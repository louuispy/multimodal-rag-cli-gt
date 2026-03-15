# 🧠 Multimodal RAG CLI

Idioma do README (README's language):
- [Português](https://github.com/louuispy/multimodal-rag-cli-gt/README.md)
- [English]()

---

> Chatbot com RAG multimodal via linha de comando — processa PDFs, vídeos do YouTube e imagens como base de conhecimento para responder perguntas com LLM.

---



Projeto desenvolvido e ensinado aos meus alunos durante o **Módulo 02 do curso de GenAI do Programa Geração Tech**, com foco em RAG (Retrieval-Augmented Generation) e LangChain.

---

## ✨ Funcionalidades

- **PDF** — carrega e indexa documentos PDF como contexto
- **YouTube** — extrai a transcrição de vídeos a partir de uma URL
- **Imagem** — processa imagens como fonte de informação
- **Chat via CLI** — interface de perguntas e respostas no terminal
- **RAG** — recupera trechos relevantes do material antes de gerar a resposta

---

## 🛠️ Stack

| Tecnologia | Função |
|---|---|
| Python | Linguagem principal |
| LangChain | Orquestração do pipeline RAG |
| InMemoryVectorStore | Vectorstore local |
| Gemini | LLM para geração de respostas |
| uv | Gerenciador de pacotes e ambiente virtual |

---

## 📁 Estrutura

```
multimodal-rag-cli-gt/
├── main.py           # Ponto de entrada da aplicação
├── utils/            # Funções auxiliares (loaders, chains, etc.)
├── material/         # Pasta com tutorial passo a passo do projeto
├── pyproject.toml    # Dependências do projeto
└── .python-version   # Versão do Python utilizada
```

---

## 🚀 Como usar

### Pré-requisitos

- Python 3.11+
- [uv](https://docs.astral.sh/uv/) instalado

### Instalação

```bash
# Clone o repositório
git clone https://github.com/louuispy/multimodal-rag-cli-gt.git
cd multimodal-rag-cli-gt

# Instale as dependências com uv
uv sync
```

### Configuração

Crie um arquivo `.env` na raiz do projeto com sua chave de API:

```env
GOOGLE_API_KEY=sua_chave_aqui
```

### Execução

```bash
uv run main.py
```

Siga as instruções no terminal para informar o tipo de fonte (PDF, YouTube ou imagem) e fazer suas perguntas.

---

## 📚 Contexto do curso

Este projeto faz parte do **Módulo 02 — RAG e LangChain** do curso de Inteligência Artificial Generativa do Programa Geração Tech, o qual sou professor. 
O módulo cobre embeddings, vectorstores, retrieval chains e integração com LLMs via LangChain.

---

## 📄 Licença

MIT © [louuispy](https://github.com/louuispy)
