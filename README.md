# Análise de Decisões Judiciais com Random Forest

## Sobre o Projeto
Este repositório contém o código e os materiais utilizados no Trabalho de Conclusão de Curso intitulado **"Análise de Decisões Judiciais – Determinação de Padrões e Predição de Julgamentos Usando Random Forest"**. O estudo foi conduzido como parte do curso de especialização em Data Science and Analytics, com o objetivo de explorar a aplicação de algoritmos de aprendizado de máquina na previsão de sentenças judiciais.

## Objetivo
O principal objetivo do estudo é identificar padrões em decisões judiciais e utilizar o algoritmo **Random Forest** para prever o resultado dos julgamentos. O modelo busca entender quais variáveis mais influenciam as sentenças, permitindo uma análise quantitativa e preditiva das decisões.

## Metodologia
- **Coleta de Dados**: Foram extraídos dados de decisões judiciais do portal do Tribunal de Justiça do Estado de São Paulo, totalizando 50 sentenças de diferentes juízes.
- **Pré-processamento**:
  - Codificação dos nomes dos réus para preservar anonimato.
  - Aplicado **One-Hot Encoding** nas variáveis categóricas (Juiz e Comarca).
  - Conversão da variável **Pena** para um formato categórico baseado em quartis.
- **Treinamento do Modelo**: Utilização do algoritmo **Random Forest**, dividido em 70% para treinamento e 30% para teste.
- **Avaliação**: Mede-se a acurácia do modelo e analisa-se a importância das variáveis no resultado das decisões judiciais.

## Resultados
- O modelo alcançou uma **acurácia de 44%** na previsão da classe de pena aplicada.
- As variáveis mais influentes foram **Comarca (49,45%)** e **Juiz (38,42%)**.
- Os resultados indicam que a localização (Comarca) exerce uma forte influência nas sentenças judiciais.
- Os juízes têm uma influência menor do que o esperado, sugerindo um certo padrão nas decisões dentro da mesma comarca.

## Tecnologias Utilizadas
- **Python** (Pandas, Scikit-learn, Matplotlib, PyMuPDF)
- **Random Forest** para classificação das decisões judiciais
- **Processamento de PDFs** para extração dos dados judiciais
- **GitHub** para versionamento do código

## Como Executar o Projeto
1. Clone o repositório:
   ```sh
   git clone https://github.com/tadeumesquita/tcc-data-science.git
   ```
2. Instale as dependências:
   ```sh
   pip install -r requirements.txt
   ```
3. Execute o script principal:
   ```sh
   python main.py
   ```

## Estrutura do Repositório
```
|
|-- data/                   # Dados brutos e processados
|-- notebooks/              # Notebooks Jupyter para exploração dos dados
|-- scripts/                # Códigos Python para extração, processamento e modelagem
|-- README.md               # Apresentação do projeto
|-- requirements.txt        # Dependências do projeto
```

## Contribuição
Se você deseja contribuir com melhorias no código ou na análise, sinta-se à vontade para abrir um Pull Request.

## Autor
**Antonio Tadeu Campos Mesquita** - [LinkedIn](https://www.linkedin.com/in/tadeumesquita/)

## Licença
Este projeto é distribuído sob a licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.

