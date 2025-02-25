# 📌 Consulta de Endereço via CEP

Este é um projeto simples utilizando **Node.js** com **Express** e **Axios** para buscar informações de endereço a partir de um CEP, consumindo a API do **ViaCEP**.

## 🚀 Tecnologias Utilizadas
- 🟢 Node.js
- ⚡ Express
- 🌐 Axios

## 🛠 Como Executar o Projeto

### 1️⃣ Clonar o Repositório
```bash
git clone https://github.com/jzampieri/SOA-AND-WEB-SERVICES/tree/main/api-viacep
cd SOA-AND-WEB-SERVICES/api-viacep
```

### 2️⃣ Instalar as Dependências
```bash
npm install
```

### 3️⃣ Iniciar o Servidor
```bash
node index.js
```
✅ O servidor iniciará em `http://localhost:3000`

## 📡 Como Utilizar a API

### 🔍 Buscar um endereço pelo CEP:
**Endpoint:**
```
GET /cep/{cep}
```
**Exemplo de Uso:**
```bash
http://localhost:3000/cep/01001000
```

**Resposta JSON:**
```json
{
  "cep": "01001-000",
  "logradouro": "Praça da Sé",
  "bairro": "Sé",
  "localidade": "São Paulo",
  "estado": "SP"
}
```

## ❌ Tratamento de Erros
- Se o CEP não for encontrado:
```json
{
  "mensagem": "CEP não encontrado"
}
```
- Se houver erro na requisição:
```json
{
  "mensagem": "Erro ao consultar o CEP"
}
```

