**Data:** 06/03/2026
## Subject/Assunto 
Este material educativo do CEUB oferece uma visão detalhada sobre os fundamentos do desenvolvimento Web, explorando desde sua criação até o funcionamento técnico das redes. O conteúdo traça a evolução histórica, diferenciando a origem da Internet via ARPANET da invenção da World Wide Web por Tim Berners-Lee no CERN. São apresentados conceitos essenciais de infraestrutura, com foco especial no sistema de endereçamento IP, detalhando as diferenças entre as versões IPv4 e IPv6. Além disso, o texto explica a distinção entre IPs públicos e privados, abordando como esses protocolos permitem a localização e comunicação de dispositivos globalmente. Por fim, a fonte estabelece objetivos de aprendizagem que incluem o estudo de arquiteturas de sistemas e protocolos de comunicação fundamentais.

## Source/Fonte 
#source/ceub  
## Area
#area/ceub/desenvolvimentoweb 


#  Fundamentos do Desenvolvimento Web

## 1. Origem e História

É fundamental distinguir entre a **Internet** (a infraestrutura) e a **Web** (o serviço de hipertexto que roda sobre ela).

- **Internet:** Nasceu como **ARPANET** em 1969, criada pelo Departamento de Defesa dos EUA. O protocolo **TCP/IP**, base da comunicação atual, foi criado em 1974 e adotado oficialmente em 1983.
- **Web (WWW):** Criada por **Tim Berners-Lee** no CERN em 1989.
    - A proposta era um sistema para compartilhar informações via **hipertexto** (textos com links para outros textos).
    - Em 1990, surgiu o primeiro navegador (**WorldWideWeb**) e o primeiro servidor (**info.cern.ch**).
    - A popularização para o público geral ocorreu entre 1993 e 1995 com navegadores como Netscape e Internet Explorer.

## 2. Modelos de Rede (TCP/IP x OSI)

A comunicação em rede é dividida em **camadas** para que dispositivos de diferentes fabricantes possam conversar entre si.

- **Modelo OSI:** Possui 7 camadas (Física até Aplicação).
- **Modelo TCP/IP:** É o modelo prático da Web, focado em 4 camadas: Acesso à Rede, Internet, Transporte e Aplicação.

## 3. Endereçamento IP e Portas

Para que um dado chegue ao destino, precisamos de um endereço (IP) e de um ponto de entrada na aplicação (Porta).

### Endereço IP (Internet Protocol)

É o número único de cada dispositivo na rede.

- **IPv4:** Formato de 4 blocos (ex: `153.51.3.10`). Limited a ~4 bilhões de endereços.
- **IPv6:** Criado para resolver a escassez do IPv4. Formato de 8 blocos hexadecimais (ex: `2001:0db8...`). Suporta $2^{128}$ endereços.
- **IP Público vs. Privado:**
    - **Público:** Único globalmente, visível na Internet e atribuído por órgãos como a IANA/LACNIC.
    - **Privado:** Usado em redes locais (LANs). Para acessar a web, o roteador usa o **NAT (Network Address Translation)** para converter o IP privado em um IP público único.

### Portas

Se o IP é o "endereço do prédio", a **porta** é o "número do apartamento".

- Garante que o pacote de dados chegue ao processo correto (ex: navegador ou e-mail).
- **Portas comuns:** HTTP (80), HTTPS (443), DNS (53), FTP (21).

## 4. Protocolos de Transporte: TCP vs. UDP

Os protocolos de transporte definem _como_ os dados são levados.

|Característica|**TCP** (Transmission Control Protocol)|**UDP** (User Datagram Protocol)|
|:--|:--|:--|
|**Foco**|Confiabilidade e integridade.|Velocidade e baixa latência.|
|**Conexão**|Estabelece conexão (Handshake de 3 vias).|Não estabelece conexão (envia e pronto).|
|**Garantia**|Confirma recebimento (ACK) e retransmite perdas.|Não confirma recebimento nem retransmite.|
|**Uso comum**|E-mail, Web (HTTP), Transferência de arquivos.|Streaming, jogos online, VoIP.|

## 5. Protocolos da Camada de Aplicação

- **DNS (Domain Name System):** O "catálogo telefônico" da web. Traduz nomes (www.google.com) em IPs numéricos.
- **FTP (File Transfer Protocol):** Específico para transferência de arquivos entre cliente e servidor.
- **Protocolos de E-mail:**
    - **SMTP:** Apenas para **enviar** e-mails.
    - **IMAP:** Para ler e gerenciar e-mails **no servidor** (sincroniza entre múltiplos dispositivos).
    - **POP3:** Baixa os e-mails para o computador e costuma removê-los do servidor (foco offline).

## 6. O Protocolo HTTP e HTTPS

É a base da comunicação navegador-servidor.

### Funcionamento e Estrutura

1. O navegador solicita uma URL.
2. Envia uma **Requisição** (Método, URL, Headers, Body).
3. O servidor processa e envia uma **Resposta** (Status Code, Headers, Body).

**Métodos Principais:** GET (buscar), POST (enviar dados/criar), PUT (atualizar), DELETE (remover).

**Códigos de Status (Categorias):**

- **2xx (Sucesso):** 200 OK, 201 Created.
- **3xx (Redirecionamento):** 301 Moved Permanently, 302 Found.
- **4xx (Erro do Cliente):** 400 Bad Request, 401 Unauthorized, 404 Not Found.
- **5xx (Erro do Servidor):** 500 Internal Server Error, 503 Service Unavailable.

### Segurança

- **HTTPS:** É o HTTP com uma camada extra de segurança (**SSL/TLS**).
- Os dados são **criptografados**, evitando a interceptação por terceiros.

## 7. Desenvolvimento com Python (Biblioteca `requests`)

Ferramenta poderosa para interagir com APIs e sites via código.

```
import requests

# Exemplo de GET
resp = requests.get("https://httpbin.org/get")
print(resp.status_code) # Verifica o sucesso (ex: 200)
print(resp.json())      # Converte resposta para dicionário Python

# Exemplo de POST com dados
payload = {"usuario": "aluno", "senha": "123"}
resposta = requests.post("https://httpbin.org/post", data=payload)
```

## 8. Arquiteturas Web

- **Cliente/Servidor:** O cliente solicita e o servidor fornece a informação. É o modelo padrão.
- **Peer-to-Peer (P2P):** Sem servidor central; todos os dispositivos são iguais (ex: BitTorrent, Blockchain).
- **REST:** Padrão para APIs que usam HTTP de forma simples e escalável, geralmente trocando dados em **JSON**.
- **Microserviços:** Divide uma aplicação grande em pequenos serviços independentes e especializados (ex: um serviço para pedidos, outro para pagamentos).