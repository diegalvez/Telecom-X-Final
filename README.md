Projeto Telecom X parte 2- Previsão e Análise de Evasão de Clientes







📊 Descrição

Este projeto é a continuação da análise de evasão de clientes de uma empresa de telecomunicações (Parte 1), agora com foco na construção de modelos preditivos para identificar clientes com alta probabilidade de churn. Além da Análise Exploratória de Dados (EDA) realizada na Parte 1, este projeto incorpora técnicas de machine learning, como Regressão Logística e Random Forest, para prever a evasão e identificar os principais fatores que influenciam o comportamento dos clientes. O objetivo é fornecer insights acionáveis e recomendações estratégicas para melhorar a retenção de clientes.

📌 Principais Insights





🚪 Tempo de Contrato: Clientes com menos tempo de contrato (especialmente <10 meses) têm maior probabilidade de evasão.



💸 Total Gasto: Clientes que evadem tendem a gastar menos ao longo do tempo, indicando possível insatisfação ou baixo custo-benefício.



🔁 Tipo de Contrato: Contratos mensais estão associados a maior evasão, enquanto contratos anuais ou bianuais promovem maior retenção.



💳 Método de Pagamento: Métodos menos automatizados, como cheques eletrônicos, correlacionam-se com maior evasão, enquanto pagamentos automáticos (cartão de crédito/débito) favorecem a retenção.



🔒 Serviços Adicionais: Clientes sem serviços como suporte técnico ou segurança online têm maior propensão a cancelar.



📉 Picos de Evasão: Observados no primeiro mês e no último mês do ciclo de 72 meses, sugerindo problemas na experiência inicial e no encerramento de contratos.



📊 Modelos Preditivos:





Random Forest com Threshold Ajustado: Melhor equilíbrio entre precisão e recall (F1-score de 0.622 para evasão).



Regressão Logística: Maior recall (0.79), ideal para identificar clientes que realmente evadem.



Random Forest Padrão: Maior acurácia geral (0.791), mas menor recall para evasão.

🛠 Tecnologias e Bibliotecas Utilizadas





Python 3.10+



Pandas: Manipulação e análise de dados.



NumPy: Operações numéricas.



Matplotlib: Visualização de gráficos.



Seaborn: Visualizações estatísticas avançadas.



Scikit-learn: Modelos de machine learning (Random Forest, Regressão Logística, pré-processamento, métricas).



Imbalanced-learn: Balanceamento de classes com SMOTE.



Jupyter Notebook: Desenvolvimento interativo.

🚀 Como Executar o Projeto





Clone o repositório:

```bash
git clone https://github.com/diegalvez/Telecom-X.git
cd Telecom
```

Crie um ambiente virtual:

```bash
python -m venv venv
```


Ative o ambiente virtual:
Windows:

```bash
venv\Scripts\activate
```


macOS/Linux:

```bash
source venv/bin/activate
```


Instale as dependências:

```bash
pip install -r requirements.txt
```


Execute o notebook:

```bash
jupyter notebook
```
Abra o arquivo telecomxfinal.ipynb ou telecomxfinal.py no Jupyter Notebook para explorar o projeto.

📋 Estrutura do Repositório





telecomxfinal.py: Script principal com a análise completa, incluindo EDA, pré-processamento, modelagem e avaliação.



dados_normalizados.csv: Conjunto de dados utilizado (não incluído no repositório; substitua pelo seu próprio dataset).



requirements.txt: Lista de dependências necessárias.



README.md: Este arquivo.

📈 Resultados e Recomendações





Melhor Modelo: Random Forest com threshold ajustado, devido ao equilíbrio entre precisão e recall.



Estratégias de Retenção:





Incentivar contratos de longo prazo com descontos.



Promover métodos de pagamento automáticos.



Investir em serviços adicionais (suporte técnico, segurança online).



Implementar programas de onboarding para novos clientes.



Monitorar proativamente clientes com alta probabilidade de evasão usando os modelos preditivos.



Observação: Os modelos Random Forest apresentaram sinais de overfitting (acurácia de treino ~99.88% vs. teste ~75–79%). Recomenda-se ajustar hiperparâmetros (ex.: max_depth, min_samples_leaf) e usar validação cruzada para melhorar a generalização.

👤 Autor

Diego Ribeiro Alves
https://www.linkedin.com/in/diegalvez

📜 Licença

Este projeto está licenciado sob a MIT License.
