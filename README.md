<div align="center">
  <a href="https://opensource.org/licenses/MIT"><img alt="License MIT" src="https://img.shields.io/badge/license-MIT-brightgreen"></a>
</div>

<p align="center">
  <a href="#sistema-de-gestão-de-processo-seletivo-para-concessão-de-bolsas-institucionais-de-mestrado-e-doutorado-do-pgcompufba">Sobre</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="https://posgress.netlify.app/">Demo</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#informações-gerais">Informações Gerais</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
   <a href="docs/requirements/index.md">User Stories</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#equipe">Equipe</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#documentação">Documentação</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#tecnologias-e-repositórios-de-desenvolvimento">Tecnologias</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#licença">License</a>
</p>

--- 

## Sistema de Gestão de Processos Seletivos para Concessão de Bolsas Institucionais de Mestrado e Doutorado do PGCOMP/UFBA

Este sistema possui o objetivo de organizar e gerenciar os processos seletivos para concessão de bolsas institucionais de Mestrado e Doutorado do Programa de Pós-Graduação em Ciência da Computação (PGCOMP) da Universidade Federal da Bahia (UFBA).

O PGCOMP, através da [Resolução nº 01/2022](https://pgcomp.ufba.br/sites/pgcomp.ufba.br/files/2022_resolucao_01_-_pgcomp_-concessaodebolsas_0.pdf), considera como bolsas institucionais aquelas bolsas oriundas das agências de fomento, recebidas como cotas e não vinculadas a projetos de pesquisa.

A Coordenação do PGCOMP/UFBA, no uso de suas atribuições legais, realiza, por meio de Editais próprios, a abertura de processos seletivos para concessão de Bolsas de Mestrado e Doutorado, conforme disposto na Resolução 01/2022.

## Informações Gerais

Este repositório é fruto de trabalho da **Disciplina MATE85 - Tópicos em Sistemas de Informação e Web I**, semestre **2022.2**, sob a orientação do **Professor Fred Durão**.

### Equipe

* **Gerência do Projeto:** Matheus Andrade e Rodrigo Meliande
* **Desenvolvedores Backend:** Djair Maykon (Tech Lead), Augusto Barreto, José Fernando e Matheus Andrade
* **Desenvolvedores Frontend:** Beatriz de Jesus (Tech Lead), Lucas Barreto, Beatriz Morais, Alexandre dos Santos, Kennedy Rocha e Rodrigo Meliande

## Demo

Acesse:

  https://sisbolsas.netlify.app/

## Documentação
* [Arquitetura](https://github.com/mate85-equipe03/selecao-bolsistas/blob/main/docs/design/arquitetura_time_3.png)
* [Requisitos/User Stories](docs/requirements/index.md)
* [Prototipação de Telas](https://www.figma.com/file/j2yQ8paIOmyaE0sPTv3wHC/posgress?node-id=0%3A1)
* [Modelo Lógico de Dados](docs/design/modelo_logico_dados.md)
* [Logo](https://www.canva.com/design/DAFLwlGOsJs/wcH0fLJuByu4h5xmKGiQTQ/edit?utm_content=DAFLwlGOsJs&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)
* [Kanban Backend](https://github.com/orgs/mate85-equipe03/projects/4) | [Kanban FrontEnd](https://mate85-equipe03.atlassian.net/jira/software/projects/PG/boards/3)
* [Plano de Testes](docs/test/index.md)
* [Documento de Implantação](https://docs.google.com/document/d/1fXFPbEcrWslb9WgyQiV8WR60qRF2jvIJ7VFmDgOCS8Q/edit?usp=sharing)

## Tecnologias e Repositórios de Desenvolvimento

### Backend

URLs:
- production: https://bolsa-api-prd.herokuapp.com/
- develop: https://radiant-cliffs-95153.herokuapp.com/


Repositório: [https://github.com/mate85-equipe03/backend](https://github.com/mate85-equipe03/backend)

* JavaScript
* [TypeScript](https://www.typescriptlang.org/)
* [Node.js](https://nodejs.org/)
* [NestJS](https://nestjs.com/)
* [Express](https://expressjs.com/)
* [Prisma](https://www.prisma.io/)
* [Postgres](https://www.postgresql.org/)

### Frontend

URL: https://sisbolsas.netlify.app/

Repositório: [https://github.com/mate85-equipe03/frontend](https://github.com/mate85-equipe03/frontend)

* JavaScript
* [TypeScript](https://www.typescriptlang.org/)
* [React](https://pt-br.reactjs.org/)
* [Vitest](https://vitest.dev/)
* [Material Design](https://material.io/)
* [Bootstrap](https://getbootstrap.com/)


## Licença

Este projeto está sob licença do MIT, para mais detalhes verifique em [LICENSE][license]. <br>
Fique a vontade para trazer novas funcionalidades ou corrigir problemas, será um prazer! 💜

---


[license]: LICENSE.md






