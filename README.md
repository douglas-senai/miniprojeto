# Mini Projeto Avaliativo - Senai

Descrição:
Este projeto foi desenvolvido como parte do Mini-Projeto Avaliativo (Módulo 1). O objetivo principal é construir um pipeline de engenharia e sanitização de dados robusto utilizando apenas recursos nativos do Python (sem o uso da biblioteca Pandas). 

A equipe de Engenharia de Dados da Olist identificou inconsistências estruturais nos arquivos `olist_products_dataset.csv` e `olist_orders_dataset.csv` que inviabilizavam a execução de relatórios automatizados de BI. Este script corrige dados nulos, padroniza categorias com expressões regulares, valida regras lógicas de negócio e formata campos temporais para o padrão brasileiro.

---

## Guia de Execução

### Pré-requisitos
* Ter o Python 3.x instalado em sua máquina.
* Nenhuma biblioteca externa é necessária:** O projeto foi desenvolvido utilizando apenas recursos nativos do Python.

### Passo a Passo

1. **Clone este repositório** para a sua máquina local utilizando o terminal ou prompt de comando:
   ```bash
   git clone https://github.com/douglas-senai/miniprojeto.git
   ```

2. **Navegue até o diretório** do projeto:
   ```bash
   cd NOME_DO_REPOSITORIO
   ```
3. **Certifique-se de que os arquivos de dados** (`olist_products_dataset.csv` e `olist_orders_dataset.csv`) estão localizados na mesma pasta do seu arquivo do notebook ou script Python.

4. **Execute o arquivo:**
   * Caso esteja utilizando o arquivo `.ipynb`, abra-o através do **Jupyter Notebook**, **VS Code** ou **Google Colab** e execute todas as células (`Run All`).
   * Caso tenha convertido para script padrão Python (`.py`), execute diretamente pelo terminal:
     ```bash
     python main.py
     ```
## Reflexão Teórica: Impacto da Limpeza de Dados em Machine Learning

A aplicação de uma lógica de programação estruturada e rigorosa na fase de preparação dos dados é o pilar mais crítico para garantir a qualidade de futuros modelos de Inteligência Artificial. Quando alimentamos um algoritmo de Machine Learning com dados brutos contendo ruídos, valores inconsistentes ou categorias duplicadas por erros de digitação, o modelo tende a memorizar essas imperfeições em vez de aprender o padrão real.

Além disso, a forma como tratamos valores nulos pode introduzir um viés no sistema. Por exemplo, se optássemos por descartar todas as linhas com dimensões físicas nulas na base da Olist, poderíamos estar eliminando do mapa justamente uma categoria inteira de produtos intangíveis, forçando o modelo preditivo a concluir erroneamente que todo produto cadastrado precisa ser pesado e volumoso. Portanto, a sanitização controlada cria uma base estatisticamente sólida, permitindo que a IA generalize seus aprendizados com justiça e precisão.
