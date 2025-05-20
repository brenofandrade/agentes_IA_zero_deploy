# 🧠 Projeto RAG com LLM para Atendimento ao Cliente - Loja de Relógios

Este projeto é um estudo de caso que demonstra a aplicação de **IA Generativa com RAG (Retrieval-Augmented Generation)** e **Modelos de Linguagem (LLM)** no contexto de uma **loja de relógios**.

## 📝 Descrição

Foi desenvolvido um **chat interativo** para atendimento ao cliente utilizando **documentos internos** como:

- Manuais de qualidade
- Termos de garantia
- Informações de contato

Esses documentos foram embutidos e integrados ao modelo via técnica de **RAG**, permitindo que o modelo gere respostas mais **contextualizadas e precisas** com base em informações reais da empresa.

## 🧰 Tecnologias e Ferramentas

- [Python](https://www.python.org/)
- [Streamlit](https://streamlit.io/) – interface de chat
- [Flask](https://flask.palletsprojects.com/) – API de backend
- [LangChain](https://www.langchain.com/) – integração com LLM e recuperação de contexto
- [OpenAI GPT (ChatGPT)](https://platform.openai.com/) – modelo de linguagem
- [FAISS](https://github.com/facebookresearch/faiss) – base vetorial para recuperação de documentos

## 🚀 Execução Local

1. **Clone o repositório:**

```bash
git clone https://github.com/seu-usuario/nome-do-repositorio.git
cd nome-do-repositorio
```

2. **Instale as dependências**

```bash
pip install -r requirements.txt
```

3. **Suba a API**

```bash
python app.py
```

4. **Execute a aplicação WEB**

```bash
streamlit run chat.py
```


5. Estrutura do projeto

📁 Agentes_IA_zero_deploy
├── app.py                 # API Flask para processar perguntas
├── chat.py                # Interface de chat com Streamlit
├── documents/             # Documentos da empresa (garantia, qualidade, etc.)
├── embeddings/            # Base vetorial FAISS
├── utils/                 # Funções auxiliares
├── config.yaml            # Configurações (chaves, paths, etc.)
├── requirements.txt       # Lista de dependências
└── README.md              # Este arquivo
