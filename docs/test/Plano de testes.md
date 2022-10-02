Unitários
Os testes unitários visam garantir a cobertura de teste desde a menor unidade do sistema, ou seja, desde as funções e componentes presentes no código.
Com isso, buscaremos cobrir as funcionalidades primordiais do nosso sistema já com os testes unitários, que irão cobrir cada método que faça parte destas funcionalidades. 
Assim, os testes unitários estarão presentes nas funcionalidades:
Login
Cadastro de aluno
Cadastro de professor 
Inscrição em Processo seletivo
Gerenciamento de Processo 
Uma vez que estes testes são feitos no código, serão desenvolvidos pelos próprios engenheiros que desenvolveram cada uma das funcionalidades. Sendo utilizado ferramentas que auxiliam na codificação e execução dos casos de testes unitários tanto no backend, quanto no frontend. Sendo elas, Jest e Vitest, respectivamente. 
Integração
Os testes de integração estão um nível acima dos unitários, com isso, eles visam testar quando as funções e módulos estão sendo utilizadas juntas. 
Seguiremos nesse nível testando também as principais funcionalidades do sistema, assim como nos unitários. No entanto, seguindo a ideia de integração e testando os módulos interagindo entre si. 
Estes testes também são realizados pelos desenvolvedores, em nível de código. 
End to End - Fim a fim
Testes end to end buscam testar o funcionamento de todo o sistema já integrado e implantado em ambiente similar ao de produção. Esses testes são de caixa preta, ou seja, não precisam que haja conhecimento do código para que sejam executados. Eles buscam simular um usuário comum utilizando o sistema e verificar se todas as funcionalidades estão de acordo com o que foi proposto. Com isso, executaremos estes testes de forma manual seguindo os cenários propostos na sequência. E será feito por uma pessoal do time que assumirá a função de tester para executá-los. 
É um nível de teste mais custoso, por ser executado manualmente e exigir que todo o sistema já esteja funcionando em ambiente similar a produção. Logo, executaremos cenários para as funções mais importantes do sistema e considerando o cenário feliz e triste para cada uma delas. 
Na escrita dos cenários utilizamos o padrão Gherkin, bastante utilizado na escrita de cenários de testes, buscando facilitar o entendimento para todos dos cenários que estão sendo testados. 
Funcionalidade: Cadastro de Aluno
Cenário: Cadastro Válido 
Dado que um aluno seja elegível para se candidatar a uma bolsa
E esteja na página de Cadastro do sistema
Quando ele preenche todos os campos com dados válidos
E clica no botão “Enviar”
Então seu cadastro é realizado
E ele é redirecionado para a tela inicial de aluno logado

Cenário: Cadastro Inválido 
Dado que um aluno esteja na página de Cadastro do sistema
Quando ele preenche os campos com dados inválidos
E clica no botão “Enviar”
Então o cadastro NÃO é realizado.
E uma mensagem informando que os dados são inválidos é exibida. 

Cenário: Cadastro sem preencher os dados
Dado que um aluno esteja na página de Cadastro do sistema
E não preenche todos os campos
Quando clica no botão “Enviar”
Então é exibido um popover indicando que o campo deve ser preenchido.

Funcionalidade: Cadastro de Professor
Cenário: Cadastro Válido 
Dado que seja um usuário ROOT
E esteja logado no sistema na página de cadastro de professor
Quando ele preenche todos os campos com dados válidos
E clica no botão “Enviar”
Então o cadastro é realizado
E uma mensagem de cadastro realizado com sucesso é exibida. 

Cenário: Cadastro Inválido 
Dado que seja um usuário ROOT
E esteja logado no sistema na página de cadastro de professor
Quando ele preenche todos os campos com dados válidos
E clica no botão “Enviar”
Então o cadastro NÃO é realizado.
E uma mensagem informando que os dados são inválidos é exibida. 

Funcionalidade: Login
Cenário: Login Válido Aluno
Dado que um aluno possua cadastro no sistema
E esteja na página de Login
Quando ele preenche sua matrícula e senha cadastradas
E clica no botão “Login”
Então ele é redirecionado para a tela inicial de aluno logado

Cenário: Login Válido Professor
Dado que um professor possua cadastro no sistema
E esteja na página de Login
Quando ele preenche seu Siape e senha cadastradas
E clica no botão “Login”
Então ele é redirecionado para a tela inicial de professor logado

Cenário: Login com dados inválidos
Dado que um usuário esteja na página de Login
Quando ele preenche os campos com dados inválidos
E clica no botão “Login”
Então é exibido um alerta com o texto “Credenciais inválidas. Tente novamente”

Cenário: Login sem preencher os dados
Dado que um usuário esteja na página de Login
Quando clica no botão “Login”
Então é exibido um popover indicando que o campo deve ser preenchido.

Funcionalidade: Inscrição em Processo seletivo
Cenário: Inscrição Válida
Dado que um aluno possua cadastro no sistema
E esteja na página de Inscrição em processo seletivo
Quando ele anexa os arquivos, preenche e marca todos os campos.
E clica no botão “Enviar”
Então a inscrição é realizada, sendo direcionado para a tela inicial
E uma mensagem de inscrição realizada com sucesso é exibida

Cenário: Inscrição Inválida
Dado que um aluno possua cadastro no sistema
E esteja na página de Inscrição em processo seletivo
Quando ele NÃO preenche todos os campos, ou não anexa todos os arquivos.
E clica no botão “Enviar”
Então a inscrição NÃO é realizada
E uma mensagem de falha na inscrição é mostrada

Funcionalidade: Gerência de Processo seletivo
Cenário: Criação de processo seletivo
Dado que um usuário ROOT esteja logado no sistema
E na página de criar processo seletivo
Quando ele preenche todos os campos obrigatórios, adiciona professores da comissão
E clica em “Enviar”
Então o processo é criado 
E uma mensagem de processo seletivo criado com sucesso é exibida

Cenário: Criação de processo seletivo sem preencher campos
Dado que um usuário ROOT esteja logado no sistema
E na página de criar processo seletivo
Quando ele NÃO preenche todos os campos obrigatórios, adiciona professores da comissão
E clica em “Enviar”
Então o processo NÃO é criado 
E uma mensagem é exibida indicando que todos os campos obrigatórios devem ser preenchidos

Cenário: Acessar página de edição de processo seletivo
Dado que um professor esteja logado no sistema
E na página de gerenciar processo seletivo
Quando ele seleciona um processo para edição
Então é carregado uma página de edição, mostrando os dados pré cadastrados e os campos que ele pode preencher

Cenário: Edição de processo seletivo 
Dado que um professor esteja logado no sistema
E na página de edição de um processo seletivo
Quando ele preenche ou altera os campos
E clica em “Salvar”
Então as informações são salvas 
E uma mensagem de sucesso é exibida

Cenário: Visualizar novos dados do processo seletivo
Dado que um professor editou informações de um processo seletivo
Quando ele acessa a página de gerenciamento de processos
Então os dados inseridos por ele devem ser mostrados no processo em questão

Exploratórios
Os testes exploratórios são aqueles executados sem seguir um planejamento ou script de testes. A pessoa que for realizar utiliza de sua experiência com outros sistemas, e navega livremente pelo sistema, fazendo o que tiver interesse. Buscando assim encontrar algum problema que não foi reportado anteriormente pelos outros testes. 
Esses testes serão executados por todos os integrantes da equipe, e pelo professor. E qualquer problema, ou comportamento estranho, deve ser reportado aos líderes da equipe para que seja avaliado se realmente é algo que não está de acordo com os requisitos e deve ser corrigido. 
