# retail-consumer-behavior-analysis-davimaia-felipe
# Sistema de Recomendação para Varejo

## Contexto

O projeto simula um cenário de varejo com 10 milhões de clientes e um orçamento de R$50.000 por mês.

A ideia é entender como um sistema de recomendação poderia funcionar nesse contexto.

---

## Problema

No varejo, principalmente online, existem muitos produtos disponíveis. Isso pode dificultar a escolha do cliente e diminuir as chances de compra.

Além disso, sem recomendação, todos os usuários acabam vendo praticamente as mesmas coisas.

---

## Objetivo

O objetivo foi analisar dados de compras e criar uma forma simples de recomendar produtos.

Não foi usado machine learning, a ideia foi simular o funcionamento de um sistema de recomendação usando regras.

---

## Dados

Foi usado um dataset com informações de compras, contendo:

- produto comprado  
- categoria  
- valor  
- frequência de compras  
- idade e gênero  

Cada linha representa uma compra.

---

## Arquitetura (simples)

Fluxo básico:

cliente → sistema → recomendação

O sistema recebe o produto comprado e retorna uma sugestão com base em regras.

----

## Análise

Durante a análise, foi possível observar que:

- a categoria "Clothing" aparece mais que as outras  
- produtos como Blouse, Pants e Jewelry aparecem com frequência  
- os clientes já têm histórico de compras (não são iniciantes)  
- o ticket médio ficou em torno de 60 dólares  

-----

## Recomendação

Como o dataset não mostra produtos comprados juntos, a recomendação foi feita com base em lógica simples.

Exemplos:

- Blouse → Jewelry  
- Pants → Belt  
- Dress → Jewelry  
- Sweater → Scarf  
- Sandals → Socks  

-------
## Custo

Orçamento: R$50.000 por mês  
Clientes: 10.000.000  

Custo por cliente ≈ R$0,005 por mês  

-------
## Conclusão

O projeto mostra que dá pra usar dados simples pra gerar recomendações.

Mesmo sem um modelo complexo, já é possível simular um sistema que ajuda na tomada de decisão no varejo.
