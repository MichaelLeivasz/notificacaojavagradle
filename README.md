# Microsserviço de Notificação por E-mail

Este microsserviço, desenvolvido em Java com Spring Boot e **Gradle**, é responsável por enviar notificações por e-mail sobre tarefas agendadas. Ele utiliza o serviço de e-mail configurado para enviar notificações aos usuários.

## Tecnologias Utilizadas

* **Java:** Linguagem de programação principal.
* **Gradle:** Sistema de build automatizado.
* **Spring Boot:** Framework para desenvolvimento rápido de aplicações Java.
* **Spring Mail:** Para envio de e-mails.

## Pré-requisitos

* Java JDK 17 ou superior.
* Gradle 7 ou superior.
* Configuração de um serviço de e-mail (SMTP) no `application.properties` ou `application.yml`.

## Endpoints da API

### E-mail

* **`POST /email`**: Envia um e-mail de notificação sobre uma tarefa.
    * Corpo da requisição: `TarefasDTO` (contendo informações da tarefa e o e-mail do destinatário).
    * Retorno: `200 OK`.

## Segurança

* Este microsserviço não possui endpoints protegidos por autenticação, pois é destinado a receber requisições internas de outros microsserviços.
