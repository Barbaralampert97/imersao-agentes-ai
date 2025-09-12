# Imersão Agentes AI

Este projeto é um exercício da **imersão de agentes de IA do Alura**, utilizando **LangChain** e o modelo **Google Gemini**.

## O que foi feito até agora

- Instalação e configuração do LLM (`ChatGoogleGenerativeAI`) com chave da API.
- Criação do **prompt de triagem** (`TRIAGEM_PROMPT`) para Service Desk.
- Definição do modelo **TriagemOut** com Pydantic, garantindo estrutura do JSON.
- Implementação da função **triagem** que recebe a mensagem do usuário e retorna uma resposta validada.
- Testes iniciais de mensagens para verificação do funcionamento da triagem.

## Competências trabalhadas

- Entender e configurar um **LLM** em Python
- Criar **prompts do sistema** claros e estruturados
- Validar saídas do LLM com **modelos de dados**
- Transformar respostas de IA em **JSON estruturado**
- Testar e depurar funções de interação com IA


RAG – Retrieval-Augmented Generation

É uma técnica usada em modelos de linguagem (como ChatGPT, LLaMA, etc.) para melhorar a geração de respostas.

Funciona combinando duas coisas:

Recuperação (Retrieval): o modelo procura informações em uma base de dados externa (documentos, PDFs, sites, etc.).

Geração (Generation): o modelo usa essas informações para gerar respostas precisas e contextualizadas.

Resumo simples:

O RAG ajuda o modelo a não depender só do que ele “lembra”, mas também buscar dados externos para dar respostas mais confiáveis.


Nesta aula, você vai:
Carregar e processar documentos PDF.
Dividir textos longos em chunks para otimizar a busca de informações.
Criar embeddings e armazenar em uma Vector Store com FAISS.
Construir uma chain RAG que busca contexto e gera respostas baseadas em documentos.
Formatar respostas com citações exatas das fontes consultadas.