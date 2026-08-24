# Analista de Dados com IA

App web que lê dados (CSV, upload por clique, arrastar e soltar, ou digitação manual item por item), gera um gráfico automaticamente e usa IA para escrever uma leitura em linguagem natural sobre o que os números mostram.

**[Ver demonstração ao vivo](#)** · *(substitua pelo link do GitHub Pages depois de publicar)*

## O que ele faz

- **Múltiplas formas de entrada de dados**: upload de arquivo `.csv`, arrastar e soltar, dois conjuntos de dados de exemplo prontos, ou formulário para digitar linha por linha
- **Visualização automática**: monta um gráfico de barras a partir dos dados, com controles para escolher qual coluna numérica exibir e por qual coluna categórica agrupar
- **Insights gerados por IA**: envia uma amostra dos dados para a API do Google Gemini e recebe de volta 3 a 5 observações concretas sobre tendências, valores que se destacam e comparações entre categorias — em português

## Tecnologias

- HTML, CSS e JavaScript puro (sem frameworks, sem build step)
- [Chart.js](https://www.chartjs.org/) para os gráficos
- [PapaParse](https://www.papaparse.com/) para leitura de CSV
- [API do Google Gemini](https://ai.google.dev/) para os insights

## Como rodar localmente

Não precisa de instalação nem servidor: é um único arquivo HTML.

1. Baixe o repositório
2. Abra o arquivo `analista-dados-ai.html` em qualquer navegador

## Como usar

1. Carregue dados de um dos quatro jeitos: upload, arrastar, exemplo pronto, ou digitação manual
2. Ajuste o gráfico escolhendo a coluna numérica e a coluna de agrupamento
3. Cole uma chave gratuita da API do Gemini (veja abaixo) e clique em **gerar insights**

### Sobre a chave da API

O app pede a chave do Gemini diretamente na interface porque **não há servidor por trás** — tudo roda no navegador de quem estiver usando. A chave:

- é gratuita, sem cartão de crédito, gerada em [aistudio.google.com/apikey](https://aistudio.google.com/apikey)
- fica apenas na memória da página enquanto ela está aberta
- nunca é enviada para nenhum lugar além da própria API do Google

## Por que este projeto

Construído para praticar leitura e transformação de dados no front-end, visualização com bibliotecas de gráficos, e integração com uma API de IA — do carregamento dos dados brutos até a geração de uma leitura automática sobre eles.
