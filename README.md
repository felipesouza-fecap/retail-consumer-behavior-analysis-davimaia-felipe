FashionHub – Sistema de Recomendação para Varejo Online
Contexto

O projeto simula o funcionamento de uma loja online de moda e acessórios chamada FashionHub, que atende 10 milhões de clientes com um orçamento limitado de R$50.000 por mês para ações de recomendação.

O objetivo é analisar dados de compras e criar um sistema simples que ajude os clientes a escolher produtos relevantes, aumentando engajamento e vendas, mesmo sem usar machine learning.

Problema

No varejo online, especialmente em lojas com grande variedade de produtos, surgem três desafios principais:

Sobrecarga de opções: clientes podem se perder entre muitas opções, diminuindo a chance de compra.
Exposição limitada: sem um sistema de recomendação, todos os usuários acabam vendo basicamente os mesmos produtos, sem personalização.
Perda de oportunidade de venda: clientes com histórico de compras e diferentes perfis (idade, gênero, frequência) não recebem sugestões estratégicas que poderiam aumentar o ticket médio.

Em resumo: a loja perde vendas e engajamento por não apresentar produtos que façam sentido para cada cliente.

Dados

Para a simulação, utilizamos um dataset com informações de compras, contendo:

Produto comprado
Categoria do produto
Valor da compra
Frequência de compras
Idade e gênero do cliente

Cada linha do dataset representa uma compra individual, permitindo analisar padrões de consumo e preferências.

Arquitetura do Sistema

O fluxo da recomendação é simples e escalável:

[Cliente] → [Input: produto comprado] → [Motor de Regras: cross-sell, upsell, segmentação por perfil] → [Output: produtos recomendados] → [Cálculo de custo]
Motor de Regras: define recomendações com base em:
Categoria do produto
Produtos complementares ou upgrades
Perfil do cliente (idade, gênero, frequência de compras)

Arquitetura pensada para ser simples, mas facilmente substituível por um sistema de machine learning no futuro.

Recomendação de Produtos

A recomendação do FashionHub foi aprimorada para incluir duas estratégias principais:

1. Cross-sell (venda cruzada)

Sugerir produtos complementares ao que o cliente comprou, aumentando o valor da compra sem forçar itens irrelevantes.

Exemplos:

Pants → Belt
Dress → Jewelry
Sweater → Scarf
Sandals → Socks

A lógica identifica padrões de produtos que “andam juntos” e recomenda de forma natural.

2. Upsell (venda adicional / upgrade)

Sugerir versões premium ou produtos mais caros relacionados ao item comprado, aumentando a receita por cliente.

Exemplos:

Blouse básica → Blouse premium
Sandals simples → Sandals de couro premium
Jewelry simples → Jewelry de designer

Mesmo sem machine learning, regras simples de categoria, valor e perfil permitem simular upgrades relevantes.

Análise Observacional
Categoria mais frequente: Clothing
Produtos mais comprados: Blouse, Pants, Jewelry
Ticket médio aproximado: 60 dólares
Clientes com histórico de compras ativo, permitindo recomendações mais personalizadas.
Cálculo de Custo
Orçamento: R$50.000/mês
Clientes: 10.000.000
Custo por cliente ≈ R$0,005/mês

Mostra que mesmo ações simples de recomendação têm excelente custo-benefício.

Conclusão

O FashionHub demonstra que, mesmo com dados simples e regras básicas, é possível criar recomendações relevantes que aumentam engajamento e vendas.

Cross-sell aumenta ticket médio de forma estratégica
Upsell incentiva upgrades de produtos
Segmentação por perfil permite personalizar experiências sem complexidade técnica

Este sistema funciona como base para soluções mais avançadas no futuro, incluindo modelos de machine learning e análise preditiva.
