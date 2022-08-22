# Visão Geral

O sistema em questão tem a função de organizar e gerenciar os processos seletivos para concessão de bolsas de mestrado e doutorado do PGCOMP/UFBA.

Adotou-se a técnica de **User Stories** para a descrição dos principais requisitos funcionais. O objetivo principal deste modelo é produzir uma visão das necessidades do sistema, através da explicação a partir do ponto de vista do usuário, de uma forma clara, curta e objetiva (sem detalhes de implementação).

Posteriormente, critérios de aceitação (baseados em regras de negócio e/ou requisitos não funcionais) podem ser anexados aos *user stories* para a validação, conforme alinhamento com a parte interessada.

# Requisitos funcionais:

## User Stories

Abaixo seguem as *user stories*, identificadas unicamente por um código de prefixo **US**. No corpo de uma user story, em negrito, há a identificação da *persona*, também comumente conhecido como autor.


**US-01.** Como **qualquer usuário elegível do sistema**, quero poder alterar minha senha de acesso ao sistema.

**US-02.**  Como **usuário ROOT do Sistema**, quero poder gerenciar os cadastros dos professores do PGCOMP.

**US-03.** Como **usuário ROOT do Sistema**, quero poder criar um Processo Seletivo e inserir os professores da Comissão.

**US-04.** Como **professor membro da Comissão do PS**, quero gerenciar um Processo Seletivo (PS), inserindo/editando  informações básicas iniciais como nome, descrição, cronograma, upload do PDF, bolsas disponíveis para o processo conforme suas características (vagas, Mestrado/Doutorado, FAPESB/CNPQ/CAPES), etc..

**US-05.** Como **candidato**, quero fazer a inscrição em um Processo Seletivo com prazo de inscrição disponível, inserindo informações e enviando documentos.

**US-06.** Como **candidato**, quero poder alterar os dados de minha inscrição em um Processo Seletivo, durante o período disponível de inscrição.

**US-07.** Como **candidato**, quero receber um email de confirmação de inscrição em um processo seletivo ao qual me inscrevi.

**US-08.** Como **candidato**, quero ter acesso ao sistema para acompanhar o status da minha inscrição no processo seletivo.

**US-09.** Como **professor membro da Comissão do PS**, quero acompanhar a lista de candidatos inscritos em determinado edital.

**US-10.** Como **professor revisor**, quero ser capaz de analisar e classificar os documentos/informações de cada candidato inscrito com base nas informações fornecidas na candidatura.

**US-11.** Como **professor auditor**, quero ser capaz de checar/verificar as informações inseridas pelo revisor nas inscrições. 

  **US-11.1.** Como **professor auditor**, quero finalizar o resultado de uma determinada inscrição caso não sejam identificadas incoerências na revisão.

  **US-11.2.** Como **professor auditor**, quero solicitar que o revisor análise/classifique novamente uma inscrição, caso seja identificada alguma incoerência na revisão da inscrição.

  **US-11.3.** Como **professor revisor**, quero poder  alterar minha análise/classificação com base no parecer da auditoria e finalizar o resultado de uma determinada inscrição	.

**US-12.** Como **professor membro da Comissão do PS**, quero identificar as inscrições pendentes de revisão ou auditoria.

**US-13.** Como **professor membro da Comissão do PS**, quero acompanhar o ranking de candidatos inscritos em determinado PS após a validação das notas.

**US-14.** Como **professor membro da Comissão do PS**, após a computação das notas de todas as inscrições, quero liberar o resultado do processo.

**US-15.** Como **candidato**, após a liberação do resultado do processo, quero ter a oportunidade de submeter recurso ao Processo Seletivo.

**US-16.** Como **professor membro da Comissão do PS**, quero poder avaliar um recurso encaminhado e emitir parecer.

**US-17.** Como **professor membro da Comissão do PS**, quero liberar o resultado final do processo.



# Requisitos não-funcionais:
 
- [arquitetura] O sistema vai ser operado via interface Web e protocolo HTTP e HTTPS (TLS/SSL).
- [arquitetura] O sistema deve ter padrão REST conectando, ao mínimo, um backend e um frontend.
- [arquitetura] O sistema deve armazenar em banco dos dados, todas as informações necessárias
- [disponibilidade] O sistema apresentará disponibilidade máxima limitada ao fornecido pelo nível de serviço gratuito da hospedagem contratada
- [desempenho] O sistema estará limitado ao desempenho fornecido pelo nível de serviço gratuito da hospedagem contratada
- [usabilidade] O usuário deverá ser capaz de utilizar o sistema tanto no desktop quanto mobile (tablets e smartphones), através de uma interface responsiva.
- [legal] O sistema deve atender às normas legais, como a Resolução 01/2022 do PGCOMP/UFBA
