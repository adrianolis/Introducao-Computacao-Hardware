# Reflexão Individual

**Disciplina:** Introdução à Computação  
**Aula:** 12  
**Data:** 06/05/2026  
**Integrante:** Adriano Lisarb Guzman Moura Batista  
**Grupo:** Individual

---

**"Qual protocolo você considera mais essencial para o funcionamento da Internet e por quê?"**

---

Dentre os protocolos estudados, considero o **TCP/IP** o mais essencial para o funcionamento da Internet. Enquanto protocolos como HTTP, DNS e FTP são responsáveis por serviços específicos, o TCP/IP é a base que torna possível qualquer comunicação em rede — sem ele, nenhum outro protocolo conseguiria operar.

O TCP/IP na prática funciona em duas camadas complementares. O **IP** cuida do endereçamento e do roteamento, garantindo que cada pacote de dados saiba de onde veio e para onde vai. Já o **TCP** assegura que esses pacotes cheguem ao destino de forma íntegra e na ordem correta, solicitando o reenvio de qualquer pacote que se perca no caminho.

Essa combinação é o que permite que um smartphone no Brasil se comunique com um servidor no Japão, passando por dezenas de roteadores diferentes, e ainda assim receba os dados corretamente. Isso ficou evidente na atividade prática da aula: ao acessar `github.com/humortadela`, todo o tráfego observado no Inspetor do Navegador — a requisição, a resposta e o próprio erro 404 — dependeu do TCP/IP para acontecer. O HTTPS criptografou a comunicação e o DNS traduziu o domínio, mas foi o TCP/IP que garantiu que os dados chegassem e voltassem.

Por ser a infraestrutura invisível que sustenta todos os outros protocolos, o TCP/IP é, na minha visão, o pilar mais essencial da Internet moderna.

---

## Referências

KUROSE, J. F.; ROSS, K. W. **Redes de computadores e a internet**. 5. ed. São Paulo: Addison Wesley, 2010.

TANENBAUM, Andrew S. **Redes de computadores**. 4. ed. Rio de Janeiro: Elsevier, 2003.
