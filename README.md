# Análise de Sentimentos e Impacto no NPS das Companhias Aéreas

Este projeto realiza uma análise de sentimentos em avaliações de clientes de várias companhias aéreas e investiga como fatores como **atrasos de voo** afetam o **Net Promoter Score (NPS)** das companhias aéreas.

## Estrutura do Projeto

1. **Leitura e Processamento de Dados**  
   - O conjunto de dados contém informações sobre avaliações de diferentes companhias aéreas, incluindo a **nota geral** de satisfação e várias características relacionadas ao serviço (conforto do assento, serviço de bordo, conectividade do Wi-Fi, etc.).
   - As avaliações são analisadas para entender como as diferentes características impactam a satisfação geral dos clientes.

2. **Análise de Nuvem de Palavras**  
   - Uma visualização de **nuvem de palavras** é criada para investigar as palavras mais frequentes em **reviews positivas** (nota >= 8) e **reviews negativas** (nota <= 3).
   - Essa análise qualitativa ajuda a entender os principais pontos mencionados nas avaliações.

3. **Estudo de Correlação**  
   - As correlações entre diferentes características, como "Seat Comfort", "Cabin Staff Service", "Food & Beverages", etc., são analisadas para entender os fatores que influenciam a **nota final** de satisfação do cliente.

4. **Classificação de Sentimentos**  
   - Os sentimentos das avaliações são classificados como **positivo**, **negativo** ou **neutro** com base nas notas gerais.
   - São desenvolvidos dois modelos de classificação de sentimentos:
     - O primeiro utiliza **textos das colunas "Review" e "Review_title"**.
     - O segundo utiliza **as notas das diferentes características**.
   - Os dois modelos são comparados para determinar qual abordagem é mais eficaz.

5. **Análise de Impacto no NPS**  
   - O **Net Promoter Score (NPS)** é calculado para avaliar a satisfação dos clientes em relação às companhias aéreas.
   - A análise investiga como os **atrasos de voo** afetam o NPS, com a comparação entre avaliações com e sem menção a atrasos.

## Requisitos

- Python 3.x
- Bibliotecas:
  - pandas
  - numpy
  - scikit-learn
  - matplotlib
  - seaborn
  - wordcloud

## Execução

1. **Pré-processamento de Dados**  
   O código começa com a leitura e o pré-processamento dos dados, onde são limpos e preparados para análise.
   
2. **Modelagem e Análise**  
   Após a preparação dos dados, a análise de sentimentos é realizada, utilizando tanto o texto das avaliações quanto as notas específicas de cada característica.

3. **Cálculo do NPS**  
   O NPS é calculado para cada companhia aérea, tanto considerando todas as avaliações quanto segmentando os dados em avaliações com e sem menção a atrasos.

## Resultados Esperados

O projeto resultará em uma análise detalhada de como os **atrasos de voo** impactam o **NPS** das companhias aéreas. Além disso, as visualizações de palavras e as comparações de modelos de classificação de sentimentos fornecerão insights sobre as avaliações dos clientes.
