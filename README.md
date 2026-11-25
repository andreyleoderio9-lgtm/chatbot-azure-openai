# 🤖 Chatbot com Azure OpenAI (Síncrono e Assíncrono)

Projeto desenvolvido em Python para integração com modelos de IA generativa do **Microsoft Azure OpenAI / Azure AI Foundry**, explorando tanto requisições tradicionais (síncronas) quanto não bloqueantes (assíncronas).

## 🚀 Funcionalidades
* **Chat Síncrono (`chat-app.py`):** Interface via terminal para interação direta com o modelo de linguagem, mantendo histórico de contexto na sessão.
* **Chat Assíncrono (`chat-async.py`):** Implementação utilizando `asyncio` e `AsyncOpenAI` para requisições não bloqueantes, ideal para escalabilidade.
* **Autenticação Segura:** Uso de `DefaultAzureCredential` (`azure-identity`) e variáveis de ambiente (`.env`) para proteger credenciais e endpoints.

## 🛠️ Tecnologias Utilizadas
* **Python 3**
* **OpenAI Python SDK** (`openai`)
* **Azure Identity** (`azure-identity`)
* **Python Dotenv** (`python-dotenv`)

## ⚙️ Como Executar o Projeto

1. **Clone o repositório:**
   ```bash
   git clone https://github.com
   cd chatbot-azure-openai
   ```

2. **Instale as dependências:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure as variáveis de ambiente:**
   Crie um arquivo `.env` na raiz do projeto com os dados do seu recurso no Azure:
   ```env
   AZURE_OPENAI_ENDPOINT="seu-endpoint-do-azure"
   MODEL_DEPLOYMENT="nome-do-seu-modelo"
   ```

4. **Execute a aplicação:**
   ```bash
   python chat-app.py
   ```
