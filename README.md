# 🩺 Saúde+ - Assistente de Triagem Médica com LLM

## 📌 Sobre o projeto

O Saúde+ é um protótipo desenvolvido para a disciplina de Projeto de Desenvolvimento 1 e pretendo integrar esse Assistente usando LLM para ajudar os usuários a procurar o médico especialista ideal para cada caso.

O objetivo da aplicação é auxiliar o usuário na identificação da especialidade médica mais adequada para avaliar os sintomas informados.

A aplicação **não realiza diagnósticos**, **não sugere medicamentos** e **não substitui uma consulta médica**. Sua função é apenas orientar o encaminhamento para um profissional adequado.

---

## 🚀 Tecnologias utilizadas

- Node.js
- Express
- HTML
- CSS
- JavaScript
- OpenRouter API
- Modelo:
  - openai/gpt-oss-120b:free

---

## 📁 Estrutura do projeto

```
SaudePlus/
│
├── public/
│   └── index.html
│
├── server.js
├── package.json
├── package-lock.json
└── .gitignore
  └── /node_modules
  └── .env
```

---

## ▶️ Como executar

### 1. Instalar as dependências

```bash
npm install
```

### 2. Criar o arquivo `.env`

```
OPENROUTER_API_KEY=sua_chave
```

### 3. Executar

```bash
npm start
```

### 4. Abrir no navegador

```
http://localhost:3000
```

---

## 🔒 Segurança

A chave da OpenRouter permanece armazenada no arquivo `.env`, impedindo que ela seja exposta ao navegador.

Toda comunicação com o modelo acontece pelo servidor Express.

---

## 💡 Diferencial do projeto

Em vez de receber apenas texto livre, a aplicação solicita que a IA responda utilizando um **JSON estruturado**.

Isso permite que o frontend saiba exatamente onde encontrar cada informação, deixando a interface organizada e facilitando futuras integrações.

---

## ⚠️ Aviso

Esta aplicação possui finalidade educacional e não substitui avaliação médica profissional.
