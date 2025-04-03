# Azure_Cognitive_Search
![image](https://github.com/user-attachments/assets/cb7da31a-7180-474a-9c46-5af3def2312f)



# 🔎 Azure Cognitive Search: Utilizando AI Search para Indexação e Consulta de Dados

Este projeto tem como objetivo demonstrar como configurar uma pesquisa utilizando o serviço **Azure Cognitive Search**, aproveitando os recursos de **Inteligência Artificial** para **indexar, enriquecer e consultar dados** de forma inteligente.

---

## 🚀 Etapas para Configurar o Azure Cognitive Search

### 1. Criar um Serviço de Azure Cognitive Search

- Acesse o [Portal do Azure](https://portal.azure.com)
- Clique em **"Criar um recurso"** > pesquise por **"Azure Cognitive Search"**
- Preencha os dados:
  - Nome do serviço
  - Região (ex: Brazil South)
  - Camada de preço (gratuita ou Standard)
  - Grupo de recursos
- Clique em **"Criar"**

---

### 2. Preparar a Fonte de Dados

Você pode usar diferentes fontes de dados, como:
- Banco de Dados SQL do Azure
- Blobs de Armazenamento do Azure (arquivos .pdf, .docx, .json, etc.)
- Cosmos DB
- Dados inseridos manualmente via API ou portal

---

### 3. Criar um Índice de Pesquisa

- No menu do serviço, vá em **"Indexers"**
- Clique em **"Adicionar indexador"**
- Configure:
  - Fonte de dados (ex: armazenamento blob)
  - Indexador (define a frequência de atualização e o enriquecimento com IA)
  - Habilidades cognitivas (opcional, para extrair insights como sentimento, entidades, texto-chave, etc.)
  - Campos do índice (ex: título, conteúdo, data, tags)

---

### 4. Habilitar Enriquecimento com AI

- Você pode adicionar habilidades cognitivas:
  - Extração de texto de arquivos
  - Tradução de idiomas
  - Detecção de sentimento
  - Identificação de entidades
  - OCR (Reconhecimento de texto em imagens)

---

### 5. Consultar Dados com Interface de Pesquisa

- Acesse a aba **"Search explorer"** no portal do Azure para testar buscas.
- Use queries como: GET /indexes/nome-do-indice/docs?api-version=2023-07-01&search=azure&searchFields=title,content

  
#### 🔍 Explicação da query:
indexes/nome-do-indice/docs → Caminho padrão para buscar documentos dentro de um índice específico.

search=azure → Termo que está sendo buscado. Pode ser qualquer palavra-chave.

searchFields=title,content → Campos onde a busca será feita.

api-version=2023-07-01 → Versão da API (verifique a mais atual na documentação).



## 💡 Insights Obtidos

- A integração da **busca tradicional com capacidades cognitivas** permite extrair mais valor de documentos não estruturados.
- Automatizar a **indexação de dados em larga escala** poupa tempo e melhora o acesso à informação.
- É possível criar experiências de busca muito mais relevantes ao usuário final com **filtros, facetas, destaque de termos e linguagem natural**.

---

## 🧠 Ferramentas que Podem se Beneficiar

- **Sistemas de busca interna** em portais corporativos
- **Plataformas de e-learning** com busca de conteúdos em vídeos e PDFs
- **Intranets** com documentos técnicos ou normativos
- **Portais jurídicos**, médicos ou científicos
- **Suporte ao cliente**: bots com base de conhecimento indexada

---

## 📘 Aprendizados

- Aprendi como configurar um serviço de Azure Cognitive Search do zero.
- Compreendi como usar habilidades cognitivas para enriquecer os dados e **melhorar a qualidade das buscas**.
- Descobri que posso **integrar dados de diversas fontes** e ainda aplicar filtros, facetas e ordenações nas buscas.
- Entendi a importância da **estruturação e definição do índice** para a performance das buscas.

---

## 📎 Referências

- [Documentação Oficial - Azure Cognitive Search](https://learn.microsoft.com/pt-br/azure/search/)
- [Portal do Language Studio](https://language.cognitive.azure.com/)

---
