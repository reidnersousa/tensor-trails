# 🧠 Tensor Trails 🚀  
📌 **Repositório de Projetos de Deep Learning**  
Este repositório contém projetos semanais para aprimorar habilidades em **Visão Computacional**, **Processamento de Linguagem Natural (NLP)**, **IA Generativa** e **MLOps/Deploy**.  

---

## 📅 Organização dos Projetos  

Cada dia da semana é dedicado a um tema específico. Os projetos são armazenados em diretórios separados e documentados com notebooks interativos.  

| Dia da Semana | Tema Principal | Projetos |
|--------------|---------------|----------|
| **Segunda-feira** | 🖼️ [**Visão Computacional**](#segunda-feira--visão-computacional) | Classificação, Detecção e Segmentação de Imagens |
| **Terça-feira** | 📝 [**Processamento de Linguagem Natural (NLP)**](#terça-feira--processamento-de-linguagem-natural-nlp) | Fine-tuning, embeddings e LLMs |
| **Quarta-feira** | 🚀 [**MLOps & Deploy**](#quinta-feira--mlops--deploy) | Deploy, Docker, MLflow e Kubernetes |
| **Quarta-feira** | 🎨 [**IA Generativa**](#quarta-feira--ia-generativa) | Modelos generativos de texto e imagem |

---

## 📌 Projetos por Dia  

### **📅 Segunda-feira | Visão Computacional**  
📂 [Acesse os projetos](./segunda_visao_computacional/)  

✅ **Nível 1: Gender_Classification_CNN**  
📌 Tarefa: Treinar um modelo CNN (ResNet, EfficientNet) para classificar imagens  
- Objetivo: Criar um classificador de imagens usando Transfer Learning.
- Ferramentas: TensorFlow/Keras ou PyTorch, OpenCV, Matplotlib.
- Dataset: [Biggest gender/face recognition dataset.](https://www.kaggle.com/datasets/maciejgronczynski/biggest-genderface-recognition-dataset)
- Entrega: Modelo treinado e um script que recebe uma imagem e retorna a classe prevista.

- 📂[Link do projeto](https://www.kaggle.com/code/reidnersantos/gender-classification-cnn-image-dataset)

✅ **Nível 2: Detecção de Objetos com YOLO/Faster R-CNN**  
📌 Tarefa: Treinar um modelo para detectar objetos em imagens/vídeos 
- Objetivo: Detectar objetos como carros, pessoas, placas, etc.
- Ferramentas: YOLOv8, Faster R-CNN, OpenCV, TensorFlow/PyTorch.
- Dataset: COCO, Pascal VOC, ou dataset customizado.
- Entrega: Script que recebe uma imagem ou vídeo e retorna bounding boxes com classes.
- Desafio Extra: Criar um Streamlit ou Gradio para upload de imagens e exibição da detecção.

✅ **Nível 3: Segmentação de Imagens (UNet / DeepLabV3)**  
📌 Tarefa: Criar um modelo de segmentação para destacar áreas específicas em imagens  
- Objetivo: Separar objetos do fundo (ex: segmentação de tumores, carros em ruas).
- Ferramentas: UNet, DeepLabV3, TensorFlow/PyTorch, OpenCV.
- Dataset: ISIC (câncer de pele), Cityscapes (segmentação urbana), ou dataset customizado.
- Entrega: Modelo que recebe uma imagem e retorna uma máscara segmentada.
- Desafio Extra: Fazer Data Augmentation e comparar o impacto na performance

✅ **Nível 4: Visão Computacional para Produção (Edge AI / Deploy)**  
📌 Tarefa: Rodar um modelo de visão computacional em um dispositivo embarcado (ex: Raspberry Pi, Jetson Nano)  
 - Objetivo: Criar um sistema de detecção/segmentação otimizado para rodar em hardware de baixa potência.
 - Ferramentas: TensorFlow Lite, OpenVINO, PyTorch Mobile.
 - Entrega: Modelo otimizado rodando em tempo real em um dispositivo embarcado.
 - Desafio Extra: Criar um pipeline de MLOps para treinar e atualizar o modelo remotamente.

---

### **📅 Terça-feira | Processamento de Linguagem Natural (NLP)**  
📂 [Acesse os projetos](./terca_nlp/)  

✅ **Nível 1: Fundamentos + Fine-Tuning Simples (Para fixar conceitos)**  
📌 Tarefa: Classificação de sentimentos em tweets (BERT Fine-Tuning)  
- Objetivo: Treinar um modelo BERT para classificar tweets como positivos, negativos ou neutros.
- Ferramentas: Hugging Face Transformers, TensorFlow/PyTorch, Pandas.
- Dataset: Sentiment140.
- Entrega: Criar um script que baixa o dataset, pré-processa os textos, treina o BERT e avalia.
- Desafio Extra: Criar uma API com FastAPI para enviar textos e receber a predição.
📂[Link do projeto](https://www.kaggle.com/code/reidnersantos/an-lise-de-sentimentos-pytorch)
✅ **Nível 2: Embeddings + Busca Semântica**  
📌 Tarefa: Criação de um sistema de busca semântica com embeddings  
- Objetivo: Indexar documentos e usar embeddings para encontrar respostas relevantes.
- Ferramentas: FAISS, ChromaDB, SentenceTransformers (BERT embeddings).
- Dataset: Perguntas e respostas de StackOverflow (ou use seus próprios textos).
- Entrega: Criar um buscador que recebe uma pergunta e retorna os documentos mais relevantes.
- Desafio Extra: Criar um front-end simples (Streamlit ou Gradio) para interação.

✅ **Nível 3: LLMs + RAG (Retrieval-Augmented Generation)**  
📌 Tarefa: Construção de um Chatbot Inteligente com LangChain + LLMs  
- Objetivo: Criar um chatbot que responde perguntas com base em documentos personalizados.
- Ferramentas: LangChain, OpenAI API / LLaMA / Mistral, ChromaDB (para memória).
- Dataset: Artigos científicos, PDFs, notícias ou base de perguntas sobre deep learning.
- Entrega: Um chatbot que processa PDFs e responde perguntas com base neles.
- Desafio Extra: Deploy com FastAPI e hospedagem no Hugging Face Spaces.

---

### 📅 **Quarta-feira | Trabalhos Práticos de MLOps e Deploy**  
📂 [Acesse os projetos](./quarta_ia_generativa/)  


✅ **Nível 1: Deploy Simples de Modelo com FastAPI**
📌 Tarefa: Criar uma API para servir um modelo de classificação de imagens
- Objetivo: Usa a EfficientNet e disponibilizar uma API para receber imagens e retornar previsões.
- Ferramentas: TensorFlow/PyTorch, FastAPI, Uvicorn, Postman para testes.
- Entrega: Código que roda localmente e permite enviar imagens via POST request para obter a predição.
- Desafio Extra: Criar uma interface com Streamlit para facilitar o uso


✅ **Nível 2: Dockerização e Deploy na Nuvem**
📌 Tarefa: Empacotar o modelo dentro de um container Docker e hospedar na nuvem
- Objetivo: Criar um Dockerfile, rodar o modelo dentro de um container e subir para um serviço na nuvem.
- Ferramentas: Docker, FastAPI, Google Cloud Run / AWS Lambda / Render.
- Entrega: Um endpoint online que recebe uma imagem e retorna a previsão.
- Desafio Extra: Criar um pipeline CI/CD no GitHub Actions para atualizar o modelo automaticamente.


✅ **Nível 3: MLOps Completo com MLflow e Kubernetes**
📌 Tarefa: Criar um pipeline completo de ML, incluindo versionamento e escalabilidade
- Objetivo: Monitorar experimentos com MLflow, salvar modelos e servir via Kubernetes.
- Ferramentas: MLflow, Kubernetes, Terraform (infra as code), Prometheus (monitoramento).
- Entrega: Infraestrutura completa para treinamento, versionamento e deploy do modelo.
- Desafio Extra: Integrar com DVC (Data Version Control) para gerenciar datasets grandes.

---

### **📅 Quinta-feira | MLOps & Deploy**  
📂 [Acesse os projetos](./quinta_mlops_deploy/)  

✅ **Nível 1: Deploy Simples com FastAPI**
📌 Tarefa: Criar uma API para servir um modelo de classificação de imagens
- Carregar um modelo treinado (.h5 ou .pt)
- Criar um endpoint /predict para receber uma imagem e retornar a classe prevista
- Testar a API localmente com curl ou Postman
- Sugestão Extra: Adicionar um endpoint /health para verificar se a API está rodando
- Entrega: Uma API funcional rodando localmente

✅ **Nível 2: Dockerização e Deploy na Nuvem**
📌 Tarefa: Colocar a API dentro de um container Docker
- Criar um Dockerfile para empacotar a API
- Testar o container localmente com docker run
- Subir para Google Cloud Run, AWS Lambda ou Render
- Sugestão Extra: Criar um docker-compose.yml para facilitar a execução
- Entrega: API rodando em um serviço na nuvem


✅ **Nível 3: MLOps Completo com MLflow e Kubernetes**
📌 Tarefa: Implementar versionamento de modelos e automação

- Usar MLflow para registrar e versionar os modelos
- Criar um pipeline que automaticamente treina e atualiza o modelo
- Implantar o modelo em um cluster Kubernetes
- Sugestão Extra: Adicionar prometheus para monitoramento
- Entrega: Modelo versionado e em produção com controle total


✅ **Nível 4: Monitoramento e Automação**
📌 Tarefa: Criar um pipeline CI/CD para atualizar o modelo automaticamente
- Configurar GitHub Actions para treinar e fazer deploy do modelo
- Adicionar logging e monitoramento (ex: logar previsões em um banco de dados)
- Sugestão Extra: Criar um sistema de feedback loop para re-treinar o modelo com novos dados
- Entrega: Um pipeline completo de ML em produção

---

### **Sexta-feira | IA Generativa**

✅ **Nível 1: Geração de Texto com Modelos Autoregressivos**
📌 Tarefa: Fine-tuning de um modelo GPT-2/GPT-3 para gerar textos específicos
- Objetivo: Treinar um modelo para escrever em um estilo específico (ex: artigos acadêmicos, diálogos de filmes, etc.).
- Ferramentas: Hugging Face Transformers, TensorFlow/PyTorch.
- Dataset: Textos temáticos de um domínio específico (pode usar datasets do Hugging Face ou criar um corpus próprio).
- Entrega: Um modelo que recebe um prompt e gera um texto coerente.
- Desafio Extra: Criar um chatbot simples com Streamlit para testar a geração de textos.

✅ **Nível 2: Geração de Imagens com GANs/Diffusion Models**
📌 Tarefa: Treinar uma GAN (DCGAN, StyleGAN) ou um modelo de difusão (Stable Diffusion)

- Objetivo: Gerar imagens realistas com base em um dataset específico (ex: rostos, paisagens, pinturas).
- Ferramentas: TensorFlow/PyTorch, Diffusers (para modelos de difusão), Generative Adversarial Networks (GANs).
- Dataset: CelebA (rostos humanos), LSUN (cenas de interiores), ou qualquer outro de interesse.
- Entrega: Um modelo capaz de gerar imagens de alta qualidade a partir de ruído.
- Desafio Extra: Criar um Streamlit para visualizar imagens geradas dinamicamente.


✅ **Nível 3: Text-to-Image com Stable Diffusion**
📌 Tarefa: Implementar um modelo de geração de imagens a partir de texto

- Objetivo: Criar um pipeline para gerar imagens a partir de descrições textuais.
- Ferramentas: Stable Diffusion, Diffusers, OpenAI CLIP.
- Dataset: Prompt-based (não precisa de dataset próprio).
- Entrega: Um script que recebe um texto e gera uma imagem correspondente.
- Desafio Extra: Criar um frontend interativo para o modelo (ex: Streamlit ou Gradio).

📌 **Nível 4: Aplicação Completa - IA Generativa em Produção**
📌 Tarefa: Criar uma API para servir um modelo generativo

- Objetivo: Servir um modelo de geração de texto ou imagens como uma API acessível via FastAPI.-
- Ferramentas: FastAPI, Hugging Face Transformers, Docker, Render/AWS/GCP.
- Entrega: Uma API que recebe um input (texto ou ruído) e retorna uma geração (texto ou imagem).
- Desafio Extra: Criar um pipeline CI/CD para treinar e atualizar o modelo automaticamente.


## 📂 Estrutura do Repositório  

