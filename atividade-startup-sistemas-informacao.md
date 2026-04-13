# Atividade: Criação de uma Startup baseada em Sistemas de Informação

**Disciplina:** Introdução à Computação 
**Autor:** Adriano Lisarb Guzmán Moura Batista
**Data:** Abril/2026  

---

## Resumo da Startup

| Campo | Descrição |
|-------|-----------|
| **Nome da Startup** | DataSense Retail |
| **Setor** | Varejo (pequeno e médio porte) |
| **Problema** | Ruptura de estoque e excesso de produtos parados |
| **Solução** | Sistema preditivo que recomenda níveis de estoque por produto e região |
| **Ativo estratégico** | Dados de vendas, clima, localização e comportamento do consumidor |

---

## Problema e Dados

### Problema real identificado
> Pequenos varejistas perdem faturamento por falta de produto e por excesso de estoque encalhado. Eles não têm ferramentas acessíveis para prever demanda.

### Dados brutos coletados

| Dado | Exemplo | Formato |
|------|---------|---------|
| Histórico de transações | "Produto X vendeu 30 unidades na última semana" | CSV |
| Comportamento do usuário | "Cliente olhou produto Y por 2 minutos" | Logs |
| Localização | "Loja no bairro Z, região Sul" | GeoJSON |
| Preferências | "Cliente busca ofertas de eletrônicos" | JSON |
| Clima | "Chuva prevista para sábado" | API aberta |
| Feriados locais | "Dia das Mães - 10/05" | CSV público |

### Mapa conceitual – Dados

| Propriedade | Resposta |
|-------------|----------|
| **Entrada (input)** | Arquivos CSV + API de clima + web scraping de feriados |
| **Origem dos dados** | PDV , ERP da loja, Google Maps API, INMET |
| **Tipo (estruturado/não estruturado)** | Predominantemente estruturado; logs de navegação são não estruturados |

---

## Processamento

### Fluxo: Coleta → Armazenamento → Processamento → Análise

| Etapa | O que acontece | Tecnologia (exemplo) |
|-------|----------------|----------------------|
| **Coleta** | Dados são capturados diariamente do sistema da loja | API, scripts automáticos |
| **Armazenamento** | Dados brutos são guardados em um local centralizado | Banco de dados |
| **Processamento** | Dados são limpos e agrupados | Linguagem Python com bibliotecas como Pandas |
| **Análise** | Um modelo simples identifica padrões de venda | Algoritmo de previsão |

### Relação com elementos do sistema

| Elemento | O que é na DataSense |
|----------|----------------------|
| **Sistema** | Motor de previsão de demanda |
| **Processos** | Importar dados → Limpar → Calcular previsão → Gerar alerta |
| **Banco de dados** | Onde ficam armazenados os históricos de venda |
| **Fluxo da informação** | Dados entram → são processados → viram relatórios → ajudam a decidir |

---

## Informação e Conhecimento

### O que o sistema descobre

| Tipo | Exemplo |
|------|---------|
| **Padrões** | "Produtos da categoria A vendem mais nos finais de semana" |
| **Tendências** | "A procura por produto B aumenta gradativamente ao longo do ano" |
| **Previsões** | "Na próxima semana, a demanda esperada para o produto C é alta" |

### Como isso ajuda o lojista

| Insight | O que o lojista aprende |
|---------|-------------------------|
| Padrão de fim de semana | Precisa abastecer mais às sextas-feiras |
| Tendência de crescimento | Precisa aumentar o pedido ao fornecedor gradualmente |
| Previsão para próxima semana | Pode comprar a quantidade certa, nem faltando nem sobrando |

---

## Decisão e Valor 

### Decisões que o sistema permite tomar

| Decisão | Exemplo prático |
|---------|------------------|
| Reabastecimento | Comprar mais unidades do produto X antes do fim de semana |
| Promoção | Reduzir preço do produto Y que está parado há muito tempo |
| Alocação | Transferir produto Z de uma loja para outra onde ele vende mais |
| Planejamento | Negociar com fornecedor antecipadamente para épocas de alta |

### Valor de negócio gerado

| Benefício | Como acontece |
|-----------|----------------|
| **Aumento de eficiência** | O lojista perde menos tempo decidindo o que comprar |
| **Redução de custos** | Menos dinheiro preso em produtos que não vendem |
| **Personalização** | Recomendações adaptadas para cada loja (não genéricas) |
| **Inovação** | Pequeno varejista usa tecnologia antes acessível só para grandes redes |

---

## Representação – Mapa Conceitual (versão em texto)

### Fluxo completo: Coleta → Armazenamento → Processamento → Análise


### Tabela conceitual

| Elemento do sistema | O que representa na startup |
|---------------------|-----------------------------|
| **Entrada** | Dados brutos (vendas, localização, comportamento) |
| **Processamento** | Limpeza, agregação e aplicação do modelo de previsão |
| **Saída** | Relatório de previsão de demanda + alertas |
| **Feedback** | Lojista informa se a previsão estava certa ou errada, melhorando o sistema |


