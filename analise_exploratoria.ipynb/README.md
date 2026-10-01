# 📊 Análise Exploratória de Cancelamento de Clientes (Churn)

Projeto de análise de dados para entender quais fatores mais influenciam o cancelamento de assinaturas por parte dos clientes.

## 🎯 Objetivo

Explorar uma base de clientes para identificar padrões de comportamento associados ao cancelamento (*churn*), como forma de apoiar decisões de retenção de clientes.

Este projeto é a etapa de **análise exploratória de dados (EDA)**. A etapa de **Machine Learning** (treino de um modelo preditivo) está em um projeto separado: [link do projeto de IA aqui].

## 🗂️ Sobre os dados

Os dados utilizados são **fictícios**, gerados de forma sintética para simular um cenário realista de assinatura de serviços (streaming, SaaS, etc). Isso foi necessário por não haver acesso a uma base de dados real para este estudo.

As colunas incluem:

| Coluna | Descrição |
|---|---|
| `Idade` | Idade do cliente |
| `Sexo` | Sexo do cliente |
| `Tempo_Como_Cliente_Meses` | Há quanto tempo o cliente está na base |
| `Frequencia_Uso` | Frequência de uso do serviço |
| `Ligacoes_Callcenter` | Quantidade de ligações para o suporte |
| `Dias_Atraso` | Dias de atraso em pagamentos |
| `Assinatura` | Plano contratado (Basic, Standard, Premium) |
| `Duracao_Contrato` | Periodicidade do contrato (Monthly, Quarterly, Annual) |
| `Total_Gasto` | Valor total gasto pelo cliente |
| `Meses_Ultima_Interacao` | Meses desde a última interação do cliente |
| `Cancelou` | Variável alvo: 1 = cancelou, 0 = não cancelou |

## 🛠️ Ferramentas utilizadas

- Python
- Pandas (manipulação de dados)
- Plotly Express (visualização de dados)
- Jupyter Notebook

## 🔍 O que foi feito

1. Importação e limpeza inicial dos dados
2. Remoção de colunas irrelevantes para a análise (ID do cliente)
3. Verificação de dados faltantes
4. Análise da proporção geral de cancelamento
5. Comparação visual de cada variável em relação ao cancelamento, através de histogramas

## 📈 Principais observações

- A base apresenta uma proporção de **58,7% de clientes que cancelaram** contra **41,3% que permaneceram**.
- Clientes com **mais dias de atraso no pagamento** aparentam maior tendência ao cancelamento.
- Um **maior número de ligações ao call center** também se mostrou associado a maiores taxas de cancelamento.
- Contratos do tipo **"Monthly" (mensal)** parecem ter cancelamento mais frequente que contratos "Quarterly" ou "Annual".

## 🚀 Próximos passos

Os padrões identificados aqui serão usados como base para o projeto seguinte, onde um modelo de Machine Learning será treinado para **prever a probabilidade de cancelamento de um cliente** a partir dessas características.

## ▶️ Como rodar este projeto

```bash
pip install pandas plotly nbformat ipykernel
```

Depois, abra o arquivo `.ipynb` em um ambiente como VS Code ou Jupyter Notebook e execute as células em ordem.

## 👤 Autor

Gabriel Matos Zanol
