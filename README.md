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
- 📂[Link do projeto](https://www.kaggle.com/code/reidnersantos/an-lise-de-sentimentos-pytorch)


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
📂[Link do projeto](https://github.com/reidnersousa/Deploy)

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

### **Sexta-feira | Docker**



✅ **Nível 1: Instalação e Configuração Básica**
📌 Tarefa: Instalar o Docker e rodar o container "hello-world".
- Objetivo: Familiarizar-se com a instalação do Docker, entender sua arquitetura e executar seu primeiro container para validar a instalação.
- Ferramentas: Docker (Docker Engine), Docker Hub.
- Entrega: Um container "hello-world" em execução, demonstrado pela saída do comando.
- Desafio Extra: Configurar o Docker para iniciar automaticamente com o sistema e explorar comandos básicos (run, ps, stop).

✅ **Nível 2: Containerização de uma Aplicação Simples**
📌 Tarefa: Desenvolver uma aplicação web simples (por exemplo, usando Flask ou Node.js) e containerizá-la.

- Objetivo: Criar um Dockerfile que defina o ambiente, copie o código da aplicação e exponha a porta para acesso.
- Ferramentas: Docker, linguagem de programação escolhida (Python/Flask ou Node.js/Express), Dockerfile.
- Entrega: Uma imagem Docker construída a partir do Dockerfile e um container rodando a aplicação.
- Desafio Extra: Escrever um arquivo Docker Compose para orquestrar a aplicação e facilitar a execução com um único comando.


✅ **Nível 3: Orquestração de Aplicações Multi-Container**
📌Tarefa: Desenvolver uma aplicação composta por múltiplos serviços (por exemplo, um backend e um banco de dados) utilizando Docker Compose.
- Objetivo: Aprender a definir serviços, redes e volumes em um arquivo docker-compose.yml, integrando diferentes containers que se comunicam entre si.
- Ferramentas: Docker Compose, Docker, uma aplicação simples (ex.: Flask para o backend e PostgreSQL como banco de dados).
- Entrega: Um projeto funcional onde o comando docker-compose up levanta todos os containers e a aplicação pode ser acessada normalmente.
- Desafio Extra: Configurar variáveis de ambiente para personalizar as configurações dos serviços e explorar a escalabilidade replicando um dos serviços.


✅ **Nível 4: Deploy de Aplicações em Produção com Pipeline CI/CD**
📌Tarefa: Criar uma pipeline de deploy automatizado para uma aplicação containerizada utilizando Docker e uma ferramenta de CI/CD.
- Objetivo: Implementar um fluxo de integração contínua e entrega contínua (CI/CD) que construa, teste e faça o deploy de uma aplicação em um ambiente de produção.
- Ferramentas: Docker, Docker Compose (ou orquestração com Docker Swarm/Kubernetes), FastAPI (para criar a API se necessário), e ferramentas de CI/CD (GitHub Actions, GitLab CI ou similares).
- Entrega: Uma API ou aplicação containerizada que é atualizada automaticamente por meio do pipeline de CI/CD, com documentação do processo.
- Desafio Extra: Implementar monitoramento e logs centralizados (por exemplo, usando Prometheus/Grafana) e configurar um pipeline que também atualize a aplicação automaticamente em caso de novas alterações no repositório.

--- 
### **Sabado | Edge Computing**

✅ **Nível 1: Configuração Básica de Dispositivo Edge**
📌 Tarefa: Configurar um Raspberry Pi (ou outro dispositivo similar) para coletar e exibir dados de sensores.

- Objetivo: Implantar um script simples que leia informações (por exemplo, temperatura e umidade) de sensores conectados, processando os dados localmente.
- Ferramentas: Raspberry Pi, Python, bibliotecas de sensores (como Adafruit_GPIO ou RPi.GPIO).
- Dataset: Dados em tempo real coletados pelo sensor durante a operação.
- Entrega: Um script funcional rodando no dispositivo que exiba os dados em um dashboard simples ou via terminal.
- Desafio Extra: Integrar comunicação via MQTT para enviar os dados coletados para um servidor central ou nuvem.

✅ **Nível 2: Implantação de Modelo de Inferência em Edge**
📌 Tarefa: Converter um modelo de Machine Learning treinado (por exemplo, para detecção de objetos) para um formato otimizado para dispositivos de borda e implementá-lo.

- Objetivo: Reduzir a latência e o consumo de recursos, tornando a inferência de modelos mais eficiente em um ambiente de Edge Computing.
- Ferramentas: TensorFlow Lite, PyTorch Mobile ou ONNX Runtime; Raspberry Pi ou dispositivo similar.
- Dataset: Utilizar um modelo pré-treinado e, se necessário, ajustar com um conjunto de dados reduzido para testes.
- Entrega: Um dispositivo edge realizando inferência em tempo real, capaz de processar imagens ou dados de sensores com baixa latência.
- Desafio Extra: Comparar o desempenho (velocidade e consumo de recursos) entre a inferência local (edge) e uma solução baseada em nuvem.

✅ **Nível 3: Pipeline de Processamento e Inferência com Contêineres**
📌 Tarefa: Containerizar uma aplicação de inferência em Edge e orquestrar o deploy em múltiplos dispositivos.

- Objetivo: Criar um pipeline robusto que integre a coleta de dados, o pré-processamento e a inferência, facilitando atualizações e escalabilidade.
- Ferramentas: Docker para containerização, Kubernetes (ou uma versão leve como K3s) para orquestração, Python.
- Dataset: Dados simulados ou reais coletados de sensores ou câmeras, conforme o cenário escolhido.
- Entrega: Um pipeline containerizado que pode ser facilmente implantado e atualizado em dispositivos edge, com integração simples via repositório (GitHub, por exemplo).
- Desafio Extra: Implementar um mecanismo de autoatualização ou monitoramento centralizado (usando ferramentas como Prometheus/Grafana) para gerenciar a performance e a saúde dos dispositivos.

✅ **Nível 4: Aplicação Completa - Edge AI em Produção com Integração CI/CD**
📌 Tarefa: Desenvolver uma API que sirva inferência de modelos em dispositivos edge e integre um pipeline de CI/CD para atualização contínua.

- Objetivo: Unir a capacidade de processamento local com processos de deploy automatizados e monitoramento híbrido (edge + nuvem), garantindo alta disponibilidade e escalabilidade.
- Ferramentas: FastAPI para criar a API, Docker para containerização, GitHub Actions ou outra ferramenta de CI/CD, e ferramentas de monitoramento (como Prometheus e Grafana).
- Dataset: Utilizar dados reais oriundos de sensores ou de uma aplicação específica (ex.: monitoramento de segurança ou qualidade de produção).
- Entrega: Uma API robusta que receba dados via endpoints, retorne inferência realizada localmente e registre métricas e logs para monitoramento.
- Desafio Extra: Implementar estratégias de failover e integração com soluções na nuvem, permitindo uma abordagem híbrida que garanta redundância e escalabilidade.


## 📂 Estrutura do Repositório  

