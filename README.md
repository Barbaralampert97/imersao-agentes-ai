# Imersão Agentes AI – Projeto de Service Desk Inteligente

Este projeto foi desenvolvido como parte da Imersão de Agentes de IA da Alura, com foco em construir um Service Desk inteligente que automatiza a triagem de solicitações e responde perguntas com base em documentos internos.

## 🎯 Objetivo

Demonstrar como criar um agente de IA capaz de:

Triar solicitações (AUTO_RESOLVER, PEDIR_INFO, ABRIR_CHAMADO).

Responder com contexto, usando RAG (Retrieval-Augmented Generation) em documentos PDF.

Gerar saídas estruturadas em JSON, facilitando integrações.

Orquestrar o fluxo de decisões via LangGraph, tornando o agente dinâmico.

## Tecnologias

LangChain → framework para integração com LLMs.

LangGraph → modelagem do fluxo do agente.

Google Gemini (via API) → modelo de linguagem principal.

pymupdf → leitura e processamento de PDFs.

dotenv → gerenciamento de credenciais.

## 📂 Estrutura do Projeto

agents.ipynb → código principal (Jupyter Notebook).

pdfs/ → documentos que servem como base de conhecimento.

.env → chave da API do Google Gemini (não incluída no repositório).

## Como Rodar

### 1. Criar ambiente virtual:

python3 -m venv .venv
source .venv/bin/activate   # Linux/macOS
.venv\Scripts\activate      # Windows

### 2. pip install -r requirements.txt

### 3. Configuração da Chave da API do Google Gemini  

Este projeto utiliza o modelo **Google Gemini**. Para rodar localmente, você precisa criar sua própria chave de API:  

1. Acesse o [Google AI Studio](https://aistudio.google.com/app/apikey).  
2. Gere uma nova chave de API.  
3. Na raiz do projeto, crie um arquivo chamado `.env`.  
4. Adicione a chave no seguinte formato:  

GOOGLE_API_KEY="SUA_CHAVE_API_AQUI"

### 4. Adicionar documentos na pasta pdfs/.

### 5. Executar o notebook:


