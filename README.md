# Chalenge-1-Data-Science-ONE
Primeiro trabalho da especialização em data science do programa ONE

# Análise de Desempenho de Lojas - Projeto Data Science

## 📌 Visão Geral
Este projeto analisa o desempenho de quatro lojas de varejo (Loja 1, Loja 2, Loja 3 e Loja 4) com base em diversos indicadores-chave como faturamento, categorias de produtos, avaliações de clientes e custos de frete. O objetivo final é recomendar qual loja deveria ser vendida com base em critérios objetivos.

## 📊 Dados Analisados
Foram considerados os seguintes aspectos para cada loja:
- **Faturamento total**
- **Vendas por categoria de produto**
- **Média de avaliações dos clientes**
- **Produtos mais e menos vendidos**
- **Custo médio de frete**
- **Distribuição geográfica das vendas**

## 🔍 Principais Métricas Comparativas

### Faturamento Total (R$)
| Loja | Faturamento |
|------|-------------|
| 1    | 1,534,509.12 |
| 2    | 1,488,459.06 |
| 3    | 1,464,025.03 |
| 4    | 1,384,497.58 |

### Média de Avaliações (1-5)
| Loja | Avaliação Média |
|------|-----------------|
| 1    | 3.98            |
| 2    | 4.04            |
| 3    | 4.05            |
| 4    | 4.00            |

### Frete Médio (R$)
| Loja | Frete Médio |
|------|------------|
| 1    | 34.69      |
| 2    | 33.62      |
| 3    | 33.07      |
| 4    | 31.28      |

### Score Calculado
(Fórmula: (Faturamento - (Qtd Produtos × Frete Médio)) × Média Avaliações)

| Loja | Score       |
|------|-------------|
| 1    | 5,776,815   |
| 2    | 5,689,146   |
| 3    | 5,610,988   |
| 4    | 5,237,408   |

## 📈 Gráficos Principais
(Incluir aqui os gráficos gerados ou links para visualização)

1. **Faturamento Total por Loja** (Gráfico de barras comparativo)
2. **Top 5 Produtos Mais Vendidos por Loja** (Gráfico de barras agrupadas)
3. **Vendas por Categoria** (Heatmap e gráfico de barras)
4. **Score por Loja** (Gráfico de barras final)

## 🎯 Recomendação Final
Com base na análise completa dos dados, **recomenda-se a venda da Loja 4** pelos seguintes motivos:

1. **Menor faturamento** entre todas as lojas (R\$ 1,384,497.58)
2. **Menor score geral** (5,237,408), significativamente abaixo das demais
3. **Sobreposição geográfica** com outras lojas, especialmente em SP, MG e RJ
4. **Categorias de produtos similares** às demais lojas, sem diferencial competitivo
5. **Frete mais baixo** não compensa o menor desempenho em vendas

A redistribuição dos clientes da Loja 4 para as demais, especialmente Loja 1 e Loja 2 que têm melhor desempenho nos mesmos mercados, traria ganhos operacionais sem perda significativa de cobertura geográfica.

## 🛠 Tecnologias Utilizadas
- Python 3
- Pandas (Análise de dados)
- Matplotlib/Seaborn (Visualização)
- Jupyter Notebook (Ambiente de desenvolvimento)

## 📂 Estrutura do Projeto
/projeto
├── images/                    # Gráficos exportados
│   └── Scatterplot Estados/   # Gráficos de dispersão por estado
├── analysis.ipynb             # Notebook com análise completa
├── README.md                  # Este arquivo
└── mapa_lojas.html            # Mapa interativo de distribuição

## 🔄 Como Reproduzir a Análise
1. Clone o repositório
2. Instale as dependências: `pip install pandas matplotlib seaborn jupyter`
3. Execute o Jupyter Notebook: `jupyter notebook analysis.ipynb`
4. Os dados são carregados automaticamente via URLs dos arquivos CSV
OU
1. Abra o Google Colab
2. Clique Ctrl + O no teclado
3. Selecione a opção GitHub
4. Cole o link para este repositório


## 📝 Observações Adicionais
- Todos os gráficos são gerados automaticamente no notebook
- O cálculo do score considera tanto aspectos financeiros quanto de satisfação do cliente
- A análise geográfica mostra concentração de vendas nas capitais dos estados
