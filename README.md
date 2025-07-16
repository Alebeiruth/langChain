# README - Sistema RAG para Buscas Semânticas

## 📌 Visão Geral

Este repositório contém um sistema RAG (Retrieval-Augmented Generation) implementado em Python usando Jupyter Notebook. O sistema permite:

- Carregar documentos de diferentes formatos (PDF, TXT)
- Processar e dividir os documentos em "chunks" (pedaços de texto)
- Criar embeddings vetoriais para representação semântica
- Armazenar os dados em um banco vetorial (ChromaDB)
- Realizar buscas semânticas eficientes

## 🛠️ Tecnologias Utilizadas

- Python 3.13.3
- Jupyter Notebook
- Bibliotecas principais:
  - LangChain (para processamento de documentos)
  - ChromaDB (banco de dados vetorial)
  - Sentence Transformers (modelos de embedding)

## 📂 Estrutura do Projeto

```
/
├── data/                  # Pasta para documentos (PDFs e TXTs)
├── experimeto_rag.ipynb   # Notebook principal com toda a implementação
└── README.md              # Este arquivo
```

## 🚀 Como Usar

1. Clone o repositório
2. Crie uma pasta chamada `data` e coloque seus documentos lá (PDFs ou TXTs)
3. Execute o notebook `experimeto_rag.ipynb` célula por célula

O notebook está organizado em etapas lógicas:

1. Configuração do ambiente
2. Experimentos com embeddings
3. Processamento de documentos
4. Criação do banco vetorial
5. Sistema de buscas semânticas

## 💡 Funcionalidades Principais

- **Carregamento de Documentos**: Suporte para PDFs e arquivos TXT
- **Chunking Inteligente**: Divisão de documentos preservando contexto
- **Embeddings Eficientes**: Uso do modelo `all-MiniLM-L6-v2` para vetorização
- **Busca Semântica**: Encontre conteúdo relevante mesmo sem termos exatos
- **Análise de Resultados**: Métricas de similaridade para avaliar relevância

## 📊 Resultados Esperados

O sistema é capaz de:
- Processar centenas de documentos
- Criar milhares de chunks com embeddings
- Realizar buscas em milissegundos
- Encontrar conteúdos semanticamente relacionados

## 🛠️ Personalização

Você pode ajustar:
- Tamanho dos chunks e sobreposição
- Modelo de embeddings
- Parâmetros do banco vetorial
- Número de resultados por busca

## 📝 Notas Importantes

- O sistema foi testado com documentos em português
- Para melhores resultados, use documentos com conteúdo relacionado
- Documentos muito grandes serão automaticamente divididos

## 📈 Próximos Passos

Possíveis melhorias:
- Adicionar interface gráfica
- Implementar cache de embeddings
- Integrar com modelos generativos
- Adicionar suporte a mais formatos de arquivo

Este projeto é um excelente ponto de partida para sistemas de recuperação de informação e aplicações de IA generativa com contexto específico.
