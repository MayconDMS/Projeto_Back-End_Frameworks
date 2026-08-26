# Projeto_Back-End_Frameworks

## Sumário

- [Início](#projeto_back-end_frameworks)
- [1. Sobre o Projeto](#1-sobre-o-projeto)
- [2. Ambiente de Desenvolvimento](#2-ambiente-de-desenvolvimento)
- [3. Front End](#3-front-end)
- [4. Back End](#4-back-end)
- [5. Arquitetura](#5-arquitetura)
- [6. Branches — GitHub Flow](#6-branches----github-flow)
- [7. Pull Requests](#7-pull-requests)
- [8. Issues](#8-issues)
- [9. Divisão de Tarefas](#9-divisao-de-tarefas)

## 1. Sobre o Projeto

Projeto desenvolvido para a disciplina de **Back-end Frameworks**, ministrada pelo professor **Cloves Rocha**, no curso de **Sistemas de Informação da UNINASSAU Olinda**.

**Objetivo do sistema:** _A definir pelo grupo._

## 2. Ambiente de Desenvolvimento

**A definir.**

Esta seção será usada depois para documentar:

- versão das linguagens utilizadas;
- versões de frameworks;
- dependências;
- ferramentas necessárias;
- instruções para configuração e execução do ambiente.

## 3. Front End

**A definir.**

Esta seção será preenchida quando as tecnologias e decisões relacionadas ao front-end forem definidas pelo grupo.

## 4. Back End

- **Linguagem:** Python
- **Framework:** Flask
- **ORM:** A definir
- **Hashing:** Argon2 — utilizado para proteção de senhas.

## 5. Arquitetura

O projeto seguirá uma **arquitetura em camadas**, separando responsabilidades para facilitar manutenção e evolução do sistema.

Fluxo esperado de responsabilidades:

**Routes → Services → Repositories → Database**

- **Routes:** recebem as requisições e devolvem as respostas da API.
- **Services:** concentram as regras de negócio.
- **Repositories:** cuidam do acesso e persistência dos dados.
- **Database:** camada de armazenamento dos dados.

## 6. Branches — GitHub Flow

> **Regra importante:** o projeto seguirá **GitHub Flow**.

1. A `main` é a branch principal.
2. Não se deve desenvolver diretamente na `main`.
3. Para trabalhar em uma tarefa, deve-se criar uma nova branch a partir da `main`.
4. O desenvolvimento deve ser feito nessa branch.
5. Após concluir a alteração, deve-se fazer `push`.
6. Em seguida, deve-se abrir um Pull Request.
7. O código deve ser revisado por outros integrantes.
8. Depois da revisão e aprovação, o PR pode ser integrado à `main`.

Exemplos de nomes de branch:

- `feature/login`
- `feature/cadastro-usuario`
- `fix/erro-login`
- `docs/readme`

**Cada alteração deve ficar isolada em uma branch apropriada.**

## 7. Pull Requests

> **Regra importante:** Pull Request não é só envio de código — é revisão e colaboração.

Os Pull Requests são parte essencial do processo de desenvolvimento. O objetivo principal de um PR é:

- resumir o que o desenvolvedor alterou;
- explicar, quando necessário, o motivo das alterações;
- indicar qual parte do projeto foi modificada;
- permitir que outros integrantes revisem o código antes do merge.

Um integrante deve conseguir abrir um PR e entender rapidamente o que foi feito e o que precisa ser revisado.

## 8. Issues

> **Regra importante:** antes de começar qualquer tarefa, consulte as **Issues**.

As Issues serão usadas para organizar:

- tarefas pendentes;
- funcionalidades;
- bugs;
- problemas encontrados;
- outras demandas relacionadas ao projeto.

Se alguém encontrar um bug ou problema que ainda esteja registrado, deve criar uma Issue com o máximo de detalhes úteis.

Exemplo:

> Bug: erro durante a validação do login.  
> Local: `app/routes/auth.py`, linha 17.  
> Descrição: a aplicação retorna `200` mesmo quando a senha fornecida está incorreta.

Informar arquivo, função, linha e comportamento observado ajuda os outros integrantes a localizar e resolver o problema mais rápido.

## 9. Divisão de Tarefas

> **Façam o que quiserem, só avisem. E peçam ajuda se precisarem.**

No início, não teremos uma divisão rígida de responsabilidades. Cada integrante pode contribuir na parte que quiser, mas deve avisar o grupo para evitar trabalho duplicado. Se travar em algum[...]
