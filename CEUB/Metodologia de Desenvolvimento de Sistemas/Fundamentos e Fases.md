**Data:** 24/02/2026
## Subject/Assunto 
Evolução/definição/fases/modelos
## Source/Fonte 
#source/ceub 
## Area
#area/ceub/metodologiadedesenvolvimentodesistemas

# Metodologia de Desenvolvimento de Sistemas: Fundamentos e Fases

O desenvolvimento de sistemas computacionais é uma atividade de alta complexidade que exige a adoção de metodologias e boas práticas para assegurar a qualidade do produto final. A ausência de processos estruturados é apontada como a principal causa de falhas operacionais em produtos entregues, evidenciando que o sucesso de um projeto depende do conhecimento e da aplicação rigorosa de métodos organizados.

### Evolução: Da Abordagem Artesanal à Engenharia de Software

Historicamente, a construção de sistemas era vista como uma "obra de arte", um processo puramente artesanal baseado em tentativa e erro. Essa abordagem era caracterizada por levantamentos informais de requisitos, ausência de modelagem do problema e pouca utilização de documentação ou normas de engenharia. Em contrapartida, a **Engenharia de Software** estabelece que o desenvolvimento não pode se limitar à implementação de código, exigindo uma forma organizada de trabalho que englobe planejamento, projeto, testes e validação.

### Definições de Processo e Metodologia

Um **processo de desenvolvimento** é definido como um conjunto de regras e atividades inter-relacionadas que permitem organizar um projeto ao estabelecer o sequenciamento das tarefas. Segundo especialistas, ele funciona como um arcabouço para construir software de alta qualidade. Já a **metodologia de desenvolvimento** é uma representação abstrata e simplificada desse processo, geralmente dividida em fases ou etapas que fornecem informações sobre as atividades e sua sequência.

### Fases Básicas do Ciclo de Vida de um Sistema

Embora não exista uma representação de processo perfeita, qualquer modelo deve contemplar fases básicas adequadas à natureza do problema. As fases fundamentais incluem:

- **Planejamento:** Envolve a antecipação de problemas e a definição dos requisitos, funções e características do sistema com base no que o usuário necessita.
- **Análise:** Foca no entendimento do domínio do problema e na definição do modelo conceitual sob a ótica do usuário, deixando de lado detalhes de implementação.
- **Projeto (Design):** Define a arquitetura do sistema, a interação entre suas partes, esquemas de bancos de dados, módulos, interfaces e o uso de bibliotecas.
- **Implementação:** Consiste no desenvolvimento do código conforme a especificação, utilizando boas práticas como revisões de código, simplicidade e refatoramento.
- **Testes:** Fase de verificação e validação para garantir o funcionamento correto, aplicando testes de unidade, integração e de sistema.
- **Manutenção:** Divide-se em **corretiva** (ajustes e correções de erros) e **evolutiva** (implementação de novas funcionalidades).

### Modelos de Desenvolvimento

Os modelos não devem ser aplicados de forma literal; eles precisam ser adaptados ao problema, ao tipo de sistema e ao contexto organizacional. Os modelos genéricos amplamente utilizados na indústria são:

Os modelos listados são metodologias clássicas de desenvolvimento de software, cada um com abordagem específica para gerenciar projetos.

## Modelo em Cascata
Abordagem linear e sequencial, com fases rígidas (requisitos, projeto, implementação, verificação e manutenção) que avançam uma após a outra, sem retrocessos. Ideal para projetos com requisitos bem definidos e estáveis.

## Modelo de Prototipação
Envolve a criação rápida de um protótipo inicial baseado em requisitos preliminares para validação com o cliente, seguido de refinamentos iterativos. Útil quando requisitos são incertos, permitindo feedback precoce.

## Modelo Espiral
Combina prototipação e análise de riscos em ciclos iterativos (planejamento, análise de risco, engenharia e avaliação), progredindo em espiral até o produto final. Indicado para projetos complexos e de alto risco.

## Modelo Iterativo e Incremental
Desenvolve o software em iterações curtas, entregando versões incrementais funcionais que adicionam funcionalidades ao longo do tempo. Permite ajustes contínuos e reduz riscos por entregas parciais.

## Modelo Baseado em Componentes
Foca na reutilização de componentes de software pré-existentes, integrando-os para formar o sistema final, com ênfase em arquitetura modular. Eficiente para sistemas grandes, acelerando desenvolvimento via bibliotecas prontas.


Os modelos de desenvolvimento de software diferem principalmente na estrutura do processo, flexibilidade para mudanças e gerenciamento de riscos.

## Principais Diferenças
| Modelo                  | Fluxo Principal                    | Foco Principal              | Flexibilidade | Melhor Para                                    |
| ----------------------- | ---------------------------------- | --------------------------- | ------------- | ---------------------------------------------- |
| Em Cascata              | Linear e sequencial                | Requisitos fixos            | Baixa         | Projetos estáveis, bem definidos               |
| Prototipação            | Iterativo com protótipos rápidos   | Feedback do cliente inicial | Alta          | Requisitos incertos                            |
| Espiral                 | Ciclos com análise de risco        | Gerenciamento de riscos     | Alta          | Projetos complexos e arriscados                |
| Iterativo e Incremental | Incrementos funcionais escalonados | Entregas parciais contínuas | Média-Alta    | Desenvolvimento evolutivo com prazos apertados |
| Baseado em Componentes  | Reutilização de módulos prontos    | Arquitetura modular         | Média         | Sistemas grandes com componentes existentes    |


