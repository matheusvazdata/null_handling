# Dataset com Idades Nulas

Este projeto contém um dataset fictício de 1000 registros, criado para fins de teste e prática de manipulação de dados com valores nulos. O dataset inclui informações sobre nome, idade, gênero, cidade e salário.

## Estrutura do Dataset

O dataset contém as seguintes colunas:

- **Nome**: Nome fictício de uma pessoa;
- **Idade**: Idade da pessoa, com alguns valores nulos;
- **Cidade**: Cidade fictícia onde a pessoa reside;
- **Salário**: Salário fictício da pessoa em Reais (R$).

## Exemplo de Dados

Aqui está uma amostra dos dados contidos no dataset:

| Nome    | Idade | Cidade         | Salário |
| ------- | ----- | -------------- | ------- |
| Ana     | 28    | São Paulo      | 7568.45 |
| Bruno   | 34    | Rio de Janeiro | 3298.55 |
| Carlos  | NaN   | Belo Horizonte | 5124.32 |
| Diana   | 45    | Curitiba       | 2456.89 |
| Eduardo | NaN   | Porto Alegre   | 3789.12 |

## Objetivos do Projeto

Este dataset foi criado para permitir a prática e teste de técnicas de manipulação de dados, especialmente aquelas relacionadas a:

- Tratamento de valores nulos;
- Análise exploratória de dados;
- Visualização de dados;
- Transformação e limpeza de dados.

## Como Utilizar

### Carregar o Dataset

Para carregar o dataset em Python, utilize a biblioteca `pandas`:

```python
import pandas as pd

# Carregar o dataset
df = pd.read_csv("dataset_with_null_ages")

# Exibir as primeiras linhas do dataset
print(df.head())
```

### Tratamento de Valores Nulos

Aqui estão alguns exemplos de como você pode lidar com os valores nulos na coluna `Idade`:

#### Remover Linhas com Valores Nulos

```python
df_clean = df.dropna(subset=['Idade'])
```

#### Preencher Valores Nulos com a Mediana

```python
df['Idade'].fillna(df['Idade'].median(), inplace=True)
```

## Recursos Adicionais

- [Pandas Documentation](https://pandas.pydata.org/pandas-docs/stable/)
- [Python for Data Analysis](https://www.oreilly.com/library/view/python-for-data/9781491957653/)

## Contribuição

Sinta-se à vontade para contribuir com melhorias para este projeto. Você pode fazer isso através de issues ou pull requests.

## Licença

Este projeto é livre para uso pessoal e educacional. Nenhuma licença específica é aplicada.

## Contato

Para mais informações, entre em contato através do e-mail: [matheusvaz.data@gmail.com](mailto:matheusvaz.data@gmail.com)
