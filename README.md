# dio-desafio-projeto-bootcamp-baires-modulo8-desafio-projeto2-visao-computacional-com-ml
Desafio de Projeto 2 - Módulo 8 - Baires Bootcamp

O objetivo é criar e documentar uma API em Python com FastAPI integrada ao Azure OpenAI, capaz de:

Receber como entrada uma imagem contendo o desenho de arquitetura de uma aplicação.

Processar a imagem utilizando técnicas de Prompt Engineering.

Gerar automaticamente uma análise de ameaças baseada na metodologia STRIDE:

Spoofing

Tampering

Repudiation

Information Disclosure

Denial of Service

Elevation of Privilege

⚠️ Atenção: este desafio é flexível. É possível implementar a solução completa ou documentar os aprendizados e reflexões sobre os conceitos apresentados.

🎯 Objetivos de Aprendizagem

Ao concluir este desafio, fui capaz de:

Aplicar os conceitos aprendidos em um ambiente prático.

Documentar processos técnicos de forma clara e estruturada.

Utilizar o GitHub como ferramenta de compartilhamento de documentação técnica.

Explorar o uso de IA Generativa com Azure OpenAI e FastAPI.

🛠️ Tecnologias Utilizadas

Python 3.10+

FastAPI

Azure OpenAI

Uvicorn (servidor de execução da API)

Pydantic (validação de dados)

Requests / HTTPX (chamadas HTTP, se aplicável)

▶️ Como Executar o Projeto

Clone este repositório:

git clone https://github.com/SEU-USUARIO/dio-modulo8-desafio-projeto2-bootcamp-baires.git
cd dio-modulo8-desafio-projeto2-bootcamp-baires


Crie um ambiente virtual e instale as dependências:

python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows
pip install -r requirements.txt


Configure suas credenciais do Azure OpenAI (em variáveis de ambiente ou arquivo .env):

AZURE_OPENAI_ENDPOINT=https://seu-endpoint.openai.azure.com/
AZURE_OPENAI_KEY=sua-chave-aqui


Execute a API:

uvicorn src.main:app --reload


Acesse no navegador:

http://127.0.0.1:8000/docs

✅ Funcionalidades Implementadas

 Receber imagens de diagramas de arquitetura.

 Processar com técnicas de prompt engineering.

 Gerar relatório de ameaças usando metodologia STRIDE.

 Melhorias futuras: integração com armazenamento em nuvem e dashboards visuais.

📖 Aprendizados

Durante o desenvolvimento deste desafio, aprendi a:

Utilizar FastAPI para construir APIs modernas e performáticas.

Explorar o Azure OpenAI para análise automatizada baseada em prompts.

Compreender melhor a metodologia STRIDE para análise de ameaças.

Documentar projetos técnicos de forma clara e organizada no GitHub.

📦 requirements.txt
fastapi==0.115.0
uvicorn[standard]==0.30.6
pydantic==2.9.2
httpx==0.27.2
python-dotenv==1.0.1
azure-ai-openai==1.0.0b8

🔎 Explicação dos pacotes

fastapi → framework principal da API.

uvicorn[standard] → servidor ASGI para rodar a aplicação.

pydantic → validação e tipagem de dados.

httpx → cliente HTTP assíncrono (caso precise consumir serviços externos).

python-dotenv → para carregar variáveis de ambiente do arquivo .env.

azure-ai-openai → SDK oficial para integração com o Azure OpenAI.
