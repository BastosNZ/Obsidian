**Data:** 24/02/2026 
## Subject/Assunto 

Este material apresenta as diretrizes acadêmicas e os fundamentos iniciais da disciplina de **Redes de Computadores** ministrada pelo professor Antônio Carlos no **CEUB**. O conteúdo estabelece um **contrato didático** detalhando critérios de avaliação, o uso da plataforma **Cisco NetAcad** e um cronograma de seminários sobre temas modernos como **Blockchain e 5G**. Além das normas, o texto explora a importância vital da **comunicação humana** e tecnológica, destacando como a infraestrutura global depende de **cabos submarinos** de fibra óptica. São explicados conceitos técnicos essenciais, como o funcionamento de **pacotes de dados** e a classificação de redes por alcance geográfico, variando de **LAN a WAN**. Por fim, a fonte diferencia conexões **cabeadas e sem fio**, enfatizando os benefícios do compartilhamento de recursos em sistemas interconectados.
## Source/Fonte 
#source/ceubu 
## Area
#area/ceub/Redesdecomputadores

# Introdução às Redes de Computadores

Este documento apresenta um resumo detalhado da disciplina de Redes de Computadores, abordando desde diretrizes acadêmicas até conceitos fundamentais de arquitetura e funcionamento de sistemas interconectados.

## Informações Gerais e Contrato Didático

A disciplina utiliza a plataforma **CISCO (NetAcad)** como base para atividades e materiais didáticos. A estrutura de avaliação é dividida em quatro módulos (M1 a M4), integrando exercícios práticos, exames individuais, participação via Kahoot e um projeto de seminário denominado PIT.

### Sistema de Avaliação

- **M1:** Exercícios na plataforma CISCO (80%) e participação (20%).
- **M2:** Avaliação individual (80%) e Exame de ponto de verificação CISCO (20%).
- **M3:** Projeto PIT (70%), Exame CISCO (20%) e Kahoot (10%).
- **M4:** Avaliação individual (80%) e Exame de ponto de verificação CISCO (20%).

### Temas de Seminários (PIT)

Os alunos devem realizar pesquisas e debates sobre tecnologias emergentes, incluindo **Blockchain**, Redes 5G, Redes Veiculares (V2V/V2X), Conexão por Satélites e **Redes Neurais** aplicadas à infraestrutura de rede.

---

## Fundamentos e Importância da Comunicação

O principal objetivo das redes de computadores é conectar dispositivos para permitir a **troca de informações rápida e eficiente**. A comunicação é vista como a base fundamental para o desenvolvimento da sociedade, permitindo a transmissão de aprendizado, a colaboração em projetos e a tomada de decisões em diversos níveis.

### Infraestrutura Global

- **Cabos Submarinos:** Constituem a espinha dorsal da comunicação mundial, sendo responsáveis por mais de **95% do tráfego de dados** entre os continentes através de fibras ópticas instaladas no leito oceânico.
- **Dependência Sistêmica:** O apagão global ocorrido em julho de 2024, causado por uma falha em uma atualização da empresa **CrowdStrike**, evidenciou a fragilidade e a interconectividade dos sistemas atuais.

---

## Tipologia e Esferas de Comunicação

As redes transformaram a interação humana em três grandes esferas:

1. **Pessoal:** Através de redes sociais, e-mails, mensagens instantâneas e VoIP (como Skype e Zoom).
2. **Governamental:** Implementação de governo eletrônico (e-Gov) e comunicação interna entre esferas municipais, estaduais e federais.
3. **Empresarial:** Uso de intranets corporativas, videoconferências, transferência segura de dados e impulsionamento do e-commerce.

---

## Requisitos e Desempenho da Rede

Para garantir a funcionalidade de sistemas distribuídos, as redes devem atender a requisitos rigorosos:

- **Desempenho:** Medido pela **Latência** (atraso de propagação) e pela **Taxa de Transmissão**. O tempo total de transferência é calculado pela soma da latência com o tamanho da mensagem dividido pela taxa.
- **Confiabilidade e Segurança:** Garantir a imunidade a falhas, proteção contra acessos externos não autorizados e controle de acesso a recursos.
- **Confidencialidade:** Garantir que a informação só esteja disponível para usuários autorizados.
- **Qualidade de Serviço (QoS):** Capacidade da rede de atender a prazos finais, exigindo largura de banda garantida e limites de latência.

---

## Arquitetura e Elementos Técnicos

### Elementos de Hardware

- **Roteadores:** Encaminham pacotes entre redes distintas.
- **Switches:** Conectam dispositivos em uma mesma rede local de forma direcionada.
- **Hubs:** Repetidores que transmitem pacotes para todos os dispositivos conectados (menos eficientes que switches).
- **Modem:** Interface de conexão entre um computador e uma rede externa (internet).

### Transmissão de Dados (Pacotes)

A internet utiliza a **comutação de pacotes**. Os dados são divididos em unidades básicas contendo:

- **Cabeçalho:** Endereços de origem/destino e controle.
- **Dados:** A carga útil real (texto, imagem, vídeo).
- **Trailer:** Informações para verificação de integridade.

O processo envolve **fragmentação**, **encapsulamento**, **roteamento** e **remontagem** (reassembly) no destino.

---

## Classificação e Abrangência Geográfica

As redes são classificadas conforme seu alcance:

- **PAN (Personal Area Network):** Redes de curtíssimo alcance (ex: Bluetooth).
- **LAN (Local Area Network):** Redes locais (ex: Ethernet, Wi-Fi).
- **MAN (Metropolitan Area Network):** Abrangência metropolitana, até 50km (ex: Wi-Max).
- **WAN (Wide Area Network):** Grande abrangência, podendo ser mundial.

### Topologias Físicas

A forma como os computadores são interconectados pode variar em configurações de **Estrela** (uso de concentrador), **Anel**, **Barra**, **Grafo (Malha)** ou modelos **Híbridos**.

---

## Aspectos de Projeto e Tecnologias de Enlace

O projeto de uma rede deve considerar a **heterogeneidade**, pois dispositivos com tecnologias diferentes (sem fio vs. fibra óptica) precisam interoperar. Para isso, define-se uma **Rede Lógica** independente (como a Internet) para compatibilização.

As tecnologias de enlace organizam os dados em quadros (frames) e podem ser:

- **Ponto-a-ponto:** Comum em redes de longa distância.
- **Multiponto:** Comum em redes locais, muitas vezes exigindo controle de acesso ao meio para evitar ou tratar **colisões**.