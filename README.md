
## 🛠️ Tecnologias Utilizadas

- **Python 3.x**
- **Pandas** - Manipulação e análise de dados
- **NumPy** - Computação numérica
- **Scikit-learn** - Machine Learning
  - KMeans para clusterização
  - Métricas de avaliação (Silhouette, Davies-Bouldin, Calinski-Harabasz)
  - Normalizer para pré-processamento
- **Matplotlib** - Visualização de dados
- **Seaborn** - Gráficos estatísticos

## �� Dataset

O projeto utiliza o dataset **CC GENERAL.csv** que contém informações sobre:
- **BALANCE**: Saldo do cartão
- **PURCHASES**: Valor total de compras
- **CASH_ADVANCE**: Adiantamento em dinheiro
- **CREDIT_LIMIT**: Limite de crédito
- **PAYMENTS**: Pagamentos realizados
- **E outras variáveis comportamentais**

## 🔧 Instalação e Configuração

### Pré-requisitos
- Python 3.7 ou superior
- pip (gerenciador de pacotes Python)

### Passos para instalação

1. **Clone o repositório**
```bash
git clone [URL_DO_REPOSITORIO]
cd Clusterização
```

2. **Crie um ambiente virtual**
```bash
python -m venv venv
```

3. **Ative o ambiente virtual**
```bash
# Windows
venv\Scripts\activate

# Linux/Mac
source venv/bin/activate
```

4. **Instale as dependências**
```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```

5. **Execute o Jupyter Notebook**
```bash
jupyter notebook
```

## �� Como Usar

1. Abra o arquivo `clusterizacao.ipynb` no Jupyter Notebook
2. Execute as células sequencialmente
3. O notebook irá:
   - Carregar e limpar os dados
   - Realizar pré-processamento
   - Aplicar algoritmos de clusterização
   - Avaliar a qualidade dos clusters
   - Gerar visualizações

## 📈 Funcionalidades Principais

### 1. Pré-processamento de Dados
- Tratamento de valores ausentes
- Normalização dos dados
- Remoção de colunas desnecessárias

### 2. Clusterização com K-Means
- Implementação do algoritmo K-Means
- Configuração de parâmetros (n_clusters=5, n_init=10, max_iter=300)

### 3. Avaliação de Clusters
- **Silhouette Score**: Mede a coesão e separação dos clusters
- **Davies-Bouldin Score**: Avalia a qualidade da clusterização
- **Calinski-Harabasz Score**: Mede a razão entre dispersão entre clusters e dentro dos clusters

### 4. Análise Comparativa
- Comparação com dados aleatórios para validação
- Análise de estabilidade usando divisão de dados
- Identificação das variáveis mais importantes

### 5. Visualização
- Gráficos de dispersão coloridos por cluster
- Análise de centroides
- Pairplot para correlações entre variáveis

## 📊 Resultados Esperados

O projeto irá gerar:
- **5 clusters** de clientes com características distintas
- **Métricas de avaliação** para validar a qualidade da clusterização
- **Visualizações** que mostram a separação dos grupos
- **Análise descritiva** de cada cluster

## 🔍 Análise dos Clusters

Após a execução, você poderá identificar:
- **Cluster 1**: Clientes com alto saldo e baixo uso
- **Cluster 2**: Clientes com alto volume de compras
- **Cluster 3**: Clientes com alto uso de adiantamento
- **Cluster 4**: Clientes com baixo limite de crédito
- **Cluster 5**: Clientes com comportamento médio

## �� Observações Importantes

- O dataset contém **8.950 registros** de clientes
- Foram utilizadas **16 variáveis** para a análise
- A normalização é aplicada para garantir que todas as variáveis tenham o mesmo peso
- As métricas de avaliação ajudam a validar a qualidade da clusterização
