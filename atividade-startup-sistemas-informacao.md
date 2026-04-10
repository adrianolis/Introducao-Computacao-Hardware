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

## Problema e Dados (A Escolha do Caos)

### Problema real identificado
> Pequenos varejistas perdem faturamento por falta de produto (ruptura) e por excesso de estoque encalhado. Eles não têm ferramentas acessíveis para prever demanda.

### Dados brutos coletados

| Dado | Exemplo | Formato |
|------|---------|---------|
| Histórico de transações | "Produto X vendeu 30 unidades na última semana" | CSV |
| Comportamento do usuário | "Cliente olhou produto Y por 2 minutos" | Logs |
| Localização | "Loja no bairro Z, região Sul" | GeoJSON |
| Preferências | "Cliente busca ofertas de eletrônicos" | JSON |
| Clima | "Chuva prevista para sábado" | API aberta |
| Feriados locais | "Dia das Mães - 10/05" | CSV público |

### Mapa conceitual – Dados (Entrada)

| Propriedade | Resposta |
|-------------|----------|
| **Entrada (input)** | Arquivos CSV + API de clima + web scraping de feriados |
| **Origem dos dados** | PDV (ponto de venda), ERP da loja, Google Maps API, INMET |
| **Tipo (estruturado/não estruturado)** | Predominantemente estruturado (90%); logs de navegação são não estruturados (10%) |

---

## Processamento (O Sistema)

### Fluxo completo: Coleta → Armazenamento → Processamento → Análise

```mermaid
graph LR
    A[PDV / ERP] -->|API| B[Apache Kafka]
    C[API Clima] --> B
    D[Web Scraping] --> B
    B --> E[Data Lake AWS S3]
    E --> F[Spark - limpeza e agregação]
    F --> G[Modelo Random Forest]
    G --> H[Dashboard Metabase]
