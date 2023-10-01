Langchain Ask PDF (Tutorial)

Este é um aplicativo Python que permite carregar um PDF e fazer perguntas sobre ele usando linguagem natural. O aplicativo utiliza um LLM para gerar uma resposta sobre o seu PDF. O LLM não responderá a perguntas não relacionadas ao documento.

Como funciona
O aplicativo lê o PDF e divide o texto em pedaços menores que podem ser alimentados em um LLM. Ele utiliza incorporações OpenAI para criar representações vetoriais dos pedaços. Em seguida, o aplicativo encontra os pedaços que são semanticamente similares à pergunta que o usuário fez e alimenta esses pedaços no LLM para gerar uma resposta.

O aplicativo utiliza o Streamlit para criar a interface gráfica e o Langchain para lidar com o LLM.

Instalação
Para instalar o repositório, por favor, clone este repositório e instale os requirements:

Copy code
pip install -r requirements.txt
Você também precisará adicionar sua chave de API da OpenAI ao arquivo .env.

Uso
Para usar o aplicativo, execute o arquivo main.py com a CLI do Streamlit (depois de ter instalado o Streamlit):

arduino
Copy code
streamlit run app.py
Contribuição
Este repositório é apenas para fins educacionais e não tem a intenção de receber mais contribuições. Ele deve ser usado como material de apoio para o tutorial do YouTube que mostra como construir o projeto.