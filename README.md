# Pipeline-Simple-EDA

## Descrição do Projeto
Este projeto consiste em um pipeline simples para Análise Exploratória de Dados (Exploratory Data Analysis - EDA) usando Python. O código realiza tarefas essenciais para preparação e exploração de dados, incluindo:

- Tratamento de valores ausentes.
- Análise univariada e bivariada com visualizações.
- Cálculo de medidas descritivas, como assimetria e curtose.
- Análise de correlações e remoção de variáveis altamente correlacionadas.
- Seleção de variáveis com base em informação mútua e variância.

O objetivo é fornecer uma base rápida e eficiente para preparação de dados antes da modelagem preditiva.

## Requisitos
As bibliotecas necessárias para executar o pipeline são:

- Python 3.8 ou superior
- pandas
- numpy
- seaborn
- matplotlib
- scipy
- scikit-learn

Para instalá-las, execute o seguinte comando:
```bash
pip install pandas numpy seaborn matplotlib scipy scikit-learn
```

## Instruções de Uso
1. Certifique-se de que o arquivo de dados esteja no formato Excel (`.xlsx`).
2. Substitua o caminho do arquivo na linha:
   ```python
   data = pd.read_excel("your-dataset.xlsx")
   ```
   pelo caminho do seu arquivo de dados.
3. Caso sua variável alvo já esteja presente no conjunto de dados, substitua "your-target-variable" pela coluna correspondente.

4. Execute o script para gerar:
   - Histogramas das variáveis numéricas.
   - Boxplots das variáveis numéricas após remoção de alta correlação.
   - Matriz de correlação.
   - Gráfico de informação mútua (caso a variável alvo esteja presente).
   - Conjunto de dados final preparado para modelagem.

5. O conjunto de dados final será salvo como um arquivo Excel chamado `name-of-final-dataset.xlsx`.

## Exemplo de Saída
Exemplo de parte do conjunto de dados final:
```
   Variable1  Variable2  Variable3
0       1.23       4.56       7.89
1       2.34       5.67       8.90
2       3.45       6.78       9.01
```

## Estrutura do Repositório
Sugerimos que a estrutura do repositório seja organizada da seguinte forma:
```
root/
├── data/
│   └── your-dataset.xlsx       # Conjunto de dados de entrada (adicionar ao .gitignore se for confidencial)
├── output/
│   └── name-of-final-dataset.xlsx  # Conjunto de dados final gerado
├── src/
│   └── pipeline_simple_eda.py   # Script principal do pipeline
├── README.md                   # Documentação do projeto
└── requirements.txt            # Lista de dependências do projeto
```

## Licença
Este projeto está licenciado sob a licença MIT. Consulte o arquivo `LICENSE` para obter mais detalhes.

## Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request.

