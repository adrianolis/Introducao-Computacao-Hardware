# Protocolos de Comunicação

**Disciplina:** Introdução à Computação  
**Aula:** 12  
**Data:** 06/05/2026  
**Integrante:** Adriano Lisarb Guzman Moura Batista  
**Grupo:** Individual

---

## O que são Protocolos?

Protocolos são conjuntos de regras que definem como os dados são empacotados, enviados, recebidos e verificados na rede. Sem eles, computadores diferentes não conseguiriam se comunicar — é a "linguagem universal" da Internet.

---

## 1. TCP/IP

O **TCP/IP** é a base fundamental de toda a comunicação na Internet. Na verdade é um conjunto de dois protocolos que trabalham juntos:

**IP (Internet Protocol)** — cuida do endereçamento e roteamento. Define de onde vem e para onde vai cada pacote de dados.

**TCP (Transmission Control Protocol)** — garante que os dados cheguem íntegros e na ordem correta. Se algum pacote se perder no caminho, o TCP solicita o reenvio.

**Exemplo prático:** ao assistir uma aula no YouTube, o TCP/IP divide o vídeo em pacotes, envia cada um pelo melhor caminho disponível e os remonta na ordem certa no seu dispositivo.

---

## 2. HTTP / HTTPS

O **HTTP (HyperText Transfer Protocol)** é o protocolo da Web. Define como o navegador (cliente) solicita páginas e como o servidor as entrega.

O **HTTPS** é a versão segura — o "S" indica que a comunicação é criptografada via TLS, impedindo que terceiros interceptem os dados.

**Exemplo prático:** ao acessar `https://github.com`, o navegador envia uma requisição HTTP GET e o servidor responde com o conteúdo da página. O HTTPS garante que essa troca seja criptografada.

> Todo site que exibe um cadeado na barra do navegador está usando HTTPS.

---

## 3. DNS

O **DNS (Domain Name System)** funciona como a "agenda de contatos" da Internet. Ele traduz nomes de domínio legíveis por humanos (como `google.com`) para endereços IP numéricos que os computadores entendem (como `142.250.79.46`).

**Exemplo prático:** ao digitar `uol.com.br` no navegador, o DNS é consultado automaticamente para descobrir qual endereço IP corresponde a esse domínio — só então a requisição é enviada ao servidor correto.

---

## 4. FTP

O **FTP (File Transfer Protocol)** é especializado na transferência direta de arquivos entre cliente e servidor. É muito utilizado no gerenciamento de hospedagem de sites.

**Exemplo prático:** um desenvolvedor que precisa enviar os arquivos do seu site para o servidor de hospedagem utiliza um cliente FTP (como FileZilla) para fazer essa transferência diretamente.

> Ao contrário do HTTP, o FTP não é usado para navegação web — sua função é exclusivamente transferir arquivos.

---

## Resumo Comparativo

| Protocolo | Função | Exemplo de uso |
|---|---|---|
| TCP/IP | Base da comunicação em rede | Todo tráfego da Internet |
| HTTP/HTTPS | Transferência de páginas web | Acessar um site no navegador |
| DNS | Traduzir domínio para IP | Digitar um endereço no navegador |
| FTP | Transferência de arquivos | Enviar arquivos para hospedagem |

---

## Referências

UNIVERSIDADE FEDERAL DO RIO GRANDE DO NORTE (UFRN). Instituto Metrópole Digital. Disponível em: https://materialpublic.imd.ufrn.br/curso/disciplina/4/21/5. Acesso em: 4 maio 2026.

KUROSE, J. F.; ROSS, K. W. **Redes de computadores e a internet**. 5. ed. São Paulo: Addison Wesley, 2010.

TANENBAUM, Andrew S. **Redes de computadores**. 4. ed. Rio de Janeiro: Elsevier, 2003.

SOARES, L. F. G. **Redes de computadores das LANs, MANs e WANs às redes ATM**. 2. ed. São Paulo: Campus, 1995.

FOROUZAN, B. **Comunicação de Dados e Redes de Computadores**. 3. ed. Porto Alegre: Bookman, 2006.
