# Conceitos Fundamentais de Segurança da Informação

## 1. Definição de Segurança da Informação (ISO/IEC 27000:2018)

A **Segurança da Informação** é definida pela norma ISO/IEC 27000:2018 como a proteção de ativos informacionais de uma organização, garantindo a continuidade do negócio, minimizando incidentes e maximizando o retorno sobre investimentos e oportunidades. Seu objetivo central é aplicar controles apropriados para proteger informações contra ameaças acidentais ou intencionais.

---

## 2. Atributos Principais

### Confidencialidade
Garante que a informação seja acessível **apenas** a indivíduos, entidades ou processos explicitamente autorizados. Impede que dados sensíveis sejam expostos a partes não autorizadas.

> **Exemplo prático:** Dados de cartão de crédito de clientes só devem ser acessados pelo sistema de pagamento e pela equipe financeira autorizada.

---

### Integridade
Garante a **precisão e completude** da informação. Os dados não podem ser alterados ou corrompidos indevidamente — seja por falha técnica ou ação maliciosa. Ferramentas como backup e criptografia são utilizadas para preservar a integridade.

> **Exemplo prático:** Um registro médico não pode ser modificado sem autorização e toda alteração deve ser rastreada.

---

### Disponibilidade
Garante que a informação e os sistemas estejam **sempre acessíveis** quando o usuário autorizado necessitar. Ataques como DDoS (Negação de Serviço) visam justamente comprometer este atributo.

> **Exemplo prático:** O sistema de internet banking de um banco deve funcionar 24 horas por dia, 7 dias por semana.

---

### Privacidade
Envolve a **proteção rigorosa de dados pessoais e sensíveis**, em conformidade com a Lei Geral de Proteção de Dados Pessoais (LGPD — Lei nº 13.709/2018) e a norma ISO/IEC 29100. Vai além da confidencialidade ao garantir o direito dos titulares sobre seus próprios dados.

> **Exemplo prático:** Uma empresa não pode compartilhar dados cadastrais de clientes com terceiros sem consentimento explícito, conforme exige a LGPD.

---

## 3. O Ecossistema de Segurança

A relação entre os elementos centrais da segurança pode ser resumida da seguinte forma:

| Elemento | Definição |
|---|---|
| **Ameaça** | Agente (natural ou humano, intencional ou acidental) com potencial para comprometer ativos |
| **Vulnerabilidade** | Fraqueza inerente em um ativo, sistema ou controle |
| **Risco** | O efeito da incerteza — probabilidade de uma ameaça explorar uma vulnerabilidade |
| **Controle** | Ações e mecanismos implementados para mitigar o risco, transformando-o em risco residual |

> **Fórmula:** `Ameaça + Vulnerabilidade = Risco → Controles`

---

## Referências

- [ABNT. NBR ISO/IEC 27000:2018 — Tecnologia da informação — Técnicas de segurança — Sistemas de gestão da segurança da informação](https://www.iso.org/standard/73906.html)
- [ABNT. NBR ISO/IEC 29100:2024 — Tecnologia da informação — Técnicas de segurança — Estrutura de privacidade]([https://www.iso.org/standard/45123.html](https://www.iso.org/standard/85938.html))
- [Lei nº 13.709/2018 — Lei Geral de Proteção de Dados Pessoais (LGPD)](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm)
