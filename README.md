# Chat Realtime com Node.js e WebSockets

Projeto de chat em tempo real utilizando Node.js, Express e Socket.IO, baseado no conceito de comunicação bidirecional via WebSockets. O objetivo é demonstrar como criar uma aplicação simples de chat onde múltiplos usuários podem trocar mensagens instantaneamente.

---

## Descrição

Esta aplicação permite que usuários conectados ao servidor enviem e recebam mensagens em tempo real, sem necessidade de recarregar a página. O fluxo de comunicação acontece através de WebSockets, garantindo baixa latência e atualização imediata das mensagens para todos os clientes conectados.

O projeto é ideal para fins educacionais e para compreensão dos conceitos básicos de aplicações realtime.

---

## Tecnologias Utilizadas

- Node.js
- Express
- Socket.IO
- HTML5
- CSS3
- JavaScript

---

## Estrutura do Projeto

```
chat-realtime/
  ├── public/
  │ └── index.html
  ├── server.js
  ├── package.json
  └── README.md
```

---

## Instalação e Configuração

### 1. Clonar o repositório

```bash
git clone https://github.com/seu-usuario/chat-realtime.git
```
---
### Iniciar o servidor
```bash
    npm run dev
```

### acessar por diferentes navegadores
Abra mais de uma aba ou navegador para testar o chat em tempo real.

## Funcionamento do Servidor

O servidor cria uma aplicação HTTP com Express e adiciona suporte a WebSockets utilizando Socket.IO.  
Sempre que um cliente envia uma mensagem, o servidor a retransmite para todos os usuários conectados.

Principais eventos:

- connection: disparado quando um usuário se conecta
- chat message: evento customizado para envio de mensagens
- disconnect: disparado quando um usuário sai do chat

---

## Interface do Usuário

A interface é construída com HTML e CSS puro e contém:

- Lista de mensagens recebidas
- Campo de texto para digitação
- Botão de envio
- Atualização automática das mensagens via Socket.IO

---
