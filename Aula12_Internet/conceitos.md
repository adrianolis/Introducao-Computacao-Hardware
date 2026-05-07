# Conceitos Fundamentais

**Disciplina:** Introdução à Computação  
**Aula:** 12  
**Data:** 04/05/2026  
**Integrante:** Adriano Lisarb Guzman Moura Batista  
**Grupo:** Individual

---

## 1. Internet vs. Web

A **Internet** e a **Web** são conceitos diferentes, mas frequentemente confundidos.

A **Internet** é a infraestrutura física global — cabos de fibra óptica, roteadores, switches e enlaces de satélite que conectam bilhões de dispositivos ao redor do mundo. É a "rodovia".

A **Web** (World Wide Web) é um serviço que funciona sobre a Internet — um sistema de páginas e documentos interligados por hiperlinks, acessados via navegador usando o protocolo HTTP/HTTPS. É o "carro que trafega na rodovia".

| | Internet | Web |
|---|---|---|
| O que é | Infraestrutura física | Serviço/aplicação |
| Componentes | Cabos, roteadores, IPs | Páginas HTML, links, navegadores |
| Protocolo principal | TCP/IP | HTTP/HTTPS |
| Exemplo | Wi-Fi, cabo, fibra óptica | Sites, blogs, portais |

> Outros serviços também usam a Internet sem ser a Web: e-mail, WhatsApp, streaming, jogos online.

---

## 2. Arquitetura Cliente-Servidor

A arquitetura **cliente-servidor** é o modelo base de comunicação da Internet. Nele, dois papéis se complementam:

**Cliente** — é quem solicita a informação. Exemplo: seu navegador ao digitar um endereço.

**Servidor** — é quem armazena e entrega a informação solicitada. Exemplo: o computador do Google que guarda as páginas de busca.

O fluxo funciona assim:

1. O cliente envia uma **requisição (Request)** ao servidor
2. O servidor processa e devolve uma **resposta (Response)**
3. O cliente exibe o resultado ao usuário

Esse modelo é usado em praticamente todos os serviços da Internet: sites, e-mails, aplicativos e streaming.

---

## 3. Endereço IP

O **IP (Internet Protocol)** é o endereço único que identifica cada dispositivo conectado à Internet — funciona como o "CEP digital" de cada máquina.

Para que os dados encontrem o caminho de ida e volta entre cliente e servidor, cada dispositivo precisa de um endereço IP. Existem dois formatos:

**IPv4** — formato mais antigo, composto por 4 números separados por ponto.  
Exemplo: `192.168.0.1`

**IPv6** — formato mais novo, criado para suportar o crescimento da Internet.  
Exemplo: `2001:0db8:85a3:0000:0000:8a2e:0370:7334`

O endereço IP garante que o pacote de dados enviado pelo cliente chegue exatamente ao servidor correto, e que a resposta volte para o dispositivo certo.

---

## Referências

UNIVERSIDADE FEDERAL DO RIO GRANDE DO NORTE (UFRN). Instituto Metrópole Digital. Disponível em: https://materialpublic.imd.ufrn.br/curso/disciplina/4/21/5. Acesso em: 4 maio 2026.

KUROSE, J. F.; ROSS, K. W. **Redes de computadores e a internet**. 5. ed. São Paulo: Addison Wesley, 2010.

TANENBAUM, Andrew S. **Redes de computadores**. 4. ed. Rio de Janeiro: Elsevier, 2003.

FOROUZAN, B. **Comunicação de Dados e Redes de Computadores**. 3. ed. Porto Alegre: Bookman, 2006.
