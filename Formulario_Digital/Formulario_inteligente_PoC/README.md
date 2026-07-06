# Formulário inteligente - Prova de Conceito (PoC)

## 🎯 Objetivo do Projeto
Esta Prova de Conceito (PoC) foi desenvolvida como parte da resolução de um case técnico para a vaga de **Analista de Processos**. O objetivo central é demonstrar como a modernização da entrada de dados — saindo de e-mails não estruturados para um formulário inteligente — pode reduzir drasticamente o lead time e o retrabalho no cadastro de novos clientes.

## 🚀 O Problema
No cenário atual (AS-IS), a empresa recebe solicitações de cadastro por e-mail, gerando:
* **20% de retrabalho** devido a documentos incompletos ou dados divergentes.
* **Lead time elevado (5 dias)** devido à verificação manual e idas e vindas de informações.

## 💡 A Solução (TO-BE)
A proposta é implementar uma interface de entrada de dados que garanta a integridade da informação antes que ela chegue ao ERP.

## 🏗️ Arquitetura da PoC
Para esta Prova de Conceito, **foi adotada uma arquitetura em monolito** (HTML, CSS e JavaScript integrados na mesma estrutura). 

* **Decisão Estratégica:** Esta abordagem foi escolhida para permitir uma validação rápida da regra de negócio (Poka-Yoke e UX), priorizando a agilidade na demonstração do conceito em detrimento de uma estrutura de microserviços ou separação completa de camadas que seria aplicada em um produto de escala industrial. 
* **Escopo:** O projeto foca na experiência do usuário e na integridade dos dados na ponta (Front-end), garantindo que o objeto JSON gerado esteja pronto para futuras integrações via API.

### Principais Funcionalidades:
* **Validação em tempo real (Poka-Yoke):** Bloqueio de avanço com campos obrigatórios vazios.
* **Interface Amigável:** Feedback visual imediato para erros de preenchimento.
* **Padronização de Dados:** Geração de JSON estruturado pronto para consumo por APIs.

## 🛠️ Tecnologias Utilizadas
* **HTML5, CSS3 & JavaScript (Vanilla):** Estrutura, estilização e lógica de validação contidas no monolito para máxima portabilidade e facilidade de teste.

## 📂 Estrutura do Repositório
* `/Apresentação_Case`: Documentação estratégica e desenhos de processos.
* `/Arquivos_formato_BPMN`: Fluxos de processos em notação BPMN.
* `/Formulario_inteligente_PoC`: Código-fonte da aplicação.

## 📋 Como testar
1. Clone este repositório.
2. Abra o arquivo `formulario_inteligente_tobe.html` em qualquer navegador.
3. Teste o preenchimento para visualizar a validação em tempo real.

---
*Desenvolvido por Sandro Monteiro | Case técnico para WAP Indústria*