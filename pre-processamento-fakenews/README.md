### Visão Geral do Projeto

O conjunto de dados é composto por 7.200 arquivos de texto, divididos equitativamente entre notícias reais e falsas (3.600 cada). A análise foca em transformar esses dados não estruturados em um pipeline de dados organizado para extração de insights.
Pipeline de NLP Aplicado

O projeto segue uma arquitetura de dados "Tidy", onde cada etapa do processamento gera uma nova camada de informação:

    Carregamento: Consolidação de milhares de arquivos .txt em um único DataFrame do Pandas.

    Normalização: Conversão para minúsculas, remoção de pontuação, URLs e números.

    Tokenização: Segmentação do texto em unidades individuais.

    Remoção de Stopwords: Limpeza de ruído gramatical e termos jornalísticos recorrentes (ex: "disse", "segundo").

    Stemming/Lematização: Redução das palavras ao seu radical para normalização semântica.

Stack Utilizada:

    Linguagem: Python 3.x

    Manipulação de Dados: Pandas

    NLP: NLTK (Natural Language Toolkit)

    Visualização: Plotly Express (Gráficos interativos)

    Nuvem de Palavras: WordCloud

    Ambiente: Google Colab / Jupyter Notebook

### Principais Insights
1. Distribuição do Tamanho dos Textos

Utilizando Histogramas e Boxplots interativos com Plotly, observou-se que a maioria das notícias no corpus é curta, com uma concentração significativa abaixo de 500 tokens. As notícias mais extensas foram identificadas estatisticamente como outliers.

2. Análise de Frequência (Top 10)

A remoção de stopwords customizadas permitiu identificar que termos como "Lula", "Presidente" e "Governo" dominam o cenário das discussões no corpus analisado.

3. Comparação entre Classes

A análise revelou distinções claras:

    Notícias Verdadeiras: Vocabulário mais institucional e descritivo (ex: "federal", "ministério", "projeto").

    Notícias Falsas: Termos com maior carga apelativa ou focados em figuras centrais específicas.

(Dica: Insira aqui prints da sua Nuvem de Palavras e do Histograma comparativo)
🔧 Como Executar

    Clone o repositório:
    Bash

git clone https://github.com/seu-usuario/projeto-nlp-fake-news.git
cd projeto-nlp-fake-news

Instale as dependências:
Bash

    pip install -r requirements.txt

    Dados:
    Certifique-se de que os arquivos .txt das notícias estão organizados nas pastas verdadeiras/ e falsas/ conforme indicado no código, ou utilize o arquivo .zip para descompactação no ambiente de execução.

    Execute o Notebook:
    Abra o arquivo .ipynb no VS Code ou faça upload para o Google Colab.

✒️ Autor

    George Felipe - Estudante de Sistemas de Informação - UFC - Seu LinkedIn
