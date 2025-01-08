# analise_sentimento_bertweet-pt-sentiment
Analise de sentimentos em português usando um modelo pré treinado bertweet-pt-sentiment - huggingface
Análise de Sentimentos em Português com BERTweet (bertweet-pt-sentiment)
Este projeto realiza a análise de sentimentos em português utilizando o modelo BERTweet pré-treinado (bertweet-pt-sentiment), disponível na plataforma Hugging Face. O modelo é baseado na arquitetura BERT, otimizada para análise de sentimentos em textos em português, e é capaz de classificar as resenhas ou opiniões em categorias de sentimento como Positivo, Negativo ou Neutro.


Tecnologias Utilizadas
Python 3.x
Transformers (Hugging Face): Biblioteca para trabalhar com modelos de PLN.
Torch: Framework para deep learning utilizado pelos modelos pré-treinados.
pandas: Biblioteca para manipulação de dados.
Matplotlib/Seaborn: Bibliotecas para visualização de dados.
from pysentimiento import create_analyzer



# Carregar o pipeline de análise de sentimentos
modelo_analise_sentimento = create_analyzer(task='sentiment', lang='pt')

# Exemplo de texto para análise
texto = "A entrega foi rápida e o produto é excelente!"

# Realizar a análise de sentimento
resultado = modelo_analise_sentimento(texto)

print(resultado)

Passo 3: Processamento de Vários Textos
Se você deseja analisar múltiplos textos, pode iterar sobre uma lista de resenhas:

