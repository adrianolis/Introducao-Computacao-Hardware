# Exercício Prático – Análise de Protocolos

**Disciplina:** Introdução à Computação  
**Repositório:** Introducao-Computacao-Hardware  
**Aula:** 12 – Internet: História, Conceitos, Protocolos e Navegadores  
**Data:** 04/05/2026  
**Grupo:** `_______________________`  
**Integrantes:** `_______________________`

---

## Ferramenta Utilizada

- [x] Inspetor do Navegador (F12)
- [ ] Wireshark

**Navegador/Versão:** Google Chrome  
**Site analisado:** https://github.com/humortadela

> O **Humortadela** foi um dos sites de humor mais populares do Brasil, ativo de 1995 até 2016.
> A URL escolhida aponta para uma organização inexistente no GitHub, gerando um **404 Not Found** real e didático.

---

## 1. Request (Requisição do Cliente)

| Campo           | Valor encontrado                        |
|-----------------|-----------------------------------------|
| URL             | https://github.com/humortadela          |
| Método HTTP     | GET                                     |
| Protocolo       | HTTP/2 (HTTPS)                          |
| Request Headers | `accept: text/html` / `user-agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 Chrome/124.0 Safari/537.36` |

**Captura de tela da aba Network:**

> Insira aqui o print dos Request Headers (arraste a imagem ou use o botão de anexar no GitHub)

---

## 2. Response (Resposta do Servidor)

| Campo         | Valor encontrado                  |
|---------------|-----------------------------------|
| Status Code   | **404 Not Found**                 |
| Content-Type  | text/plain; charset=utf-8         |
| Server        | github.com                        |
| Cache-Control | no-cache                          |

**Captura de tela da aba Network:**

> Insira aqui o print dos Response Headers

---

## 3. Status Code Identificado

- [ ] 200 OK – Sucesso.
- [ ] 301/302 – Redirecionamento.
- [x] **404 Not Found** – Página não encontrada no servidor.
- [ ] 500 Internal Server Error – Erro interno no servidor.

**O que esse código significa na prática?**

O servidor do GitHub respondeu normalmente à requisição — o DNS funcionou, o TCP/IP estabeleceu a conexão e o HTTPS criptografou a comunicação. Porém, o recurso `/humortadela` não existe no servidor. Isso demonstra que **404 não significa "site fora do ar"**, mas sim que o servidor está ativo e acessível, porém não encontrou o recurso solicitado naquele caminho.

---

## 4. Protocolos Identificados na Análise

### TCP/IP
- Apareceu na análise? [x] Sim
- O TCP/IP foi a base de toda a comunicação. Ele dividiu os dados em pacotes, cuidou do roteamento até os servidores do GitHub e garantiu que os pacotes chegassem íntegros e na ordem correta. Toda a troca de Request e Response que aparece na aba Network passou pelo TCP/IP, mesmo que de forma invisível ao usuário.

---

### HTTP / HTTPS
- Apareceu na análise? [x] Sim
- O site utilizou **HTTPS** (HTTP/2 com criptografia TLS). Isso é confirmado pelo cadeado na barra do navegador e pelo protocolo `HTTP/2` nos headers. O "S" garante que os dados trafegaram criptografados entre o navegador e o servidor do GitHub, protegendo a comunicação mesmo que a resposta tenha sido um erro 404.

---

### DNS
- Antes de qualquer requisição aparecer na aba Network, o navegador precisou traduzir o domínio `github.com` para um endereço IP numérico. Esse processo é feito automaticamente pelo DNS, funcionando como uma "agenda de contatos" da internet. Sem o DNS, o navegador não saberia para qual servidor enviar a requisição.

---

### FTP
- Esse protocolo apareceu? [ ] Sim [x] Não
- O FTP não foi utilizado nessa comunicação. Ele seria usado em um contexto diferente, como por exemplo para um desenvolvedor transferir arquivos diretamente para um servidor de hospedagem de sites. No caso de páginas web acessadas pelo navegador, o protocolo utilizado é o HTTP/HTTPS.

---

## 5. Conclusão do Grupo

Ao acessar `https://github.com/humortadela`, o navegador seguiu o ciclo completo de comunicação da internet: o **DNS** traduziu o domínio para um IP, o **TCP/IP** estabeleceu a conexão e dividiu os dados em pacotes, e o **HTTPS** criptografou toda a troca de informações. O servidor do GitHub recebeu a requisição GET, processou normalmente, mas retornou **404 Not Found** pois a organização `/humortadela` não existe.

O protocolo que consideramos mais essencial nessa comunicação foi o **TCP/IP**, pois ele é a base invisível que sustenta todos os outros — sem ele, nenhuma requisição chegaria ao destino, independentemente do protocolo de aplicação utilizado.

---

*Arquivo gerado para o repositório `Introducao-Computacao-Hardware` — Aula12_Internet/*
