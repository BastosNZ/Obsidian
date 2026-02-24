**Data:** 24/02/2026
## Subject/Assunto 
1.1 Conceito de Análise e Projeto
1.2 Conceito de Análise e Projeto Orientado a Objetos 
1.3 Linguagem de Modelagem Unificada (UML) 
1.4 Histórico 
1.5 Diagramas estáticos e dinâmicos 
1.6 Conceitos de Processo Simplificado de Desenvolvimento de Software 
1.7 Utilização de ferramenta CASE
## Source/Fonte 
#source/ceub
## Area
#area/ceub/análiseeprojetodesistemas 


## 1.1 Conceito de Análise e Projeto

#### Conceito de análise
Estudo dos problemas de negócios de requisitos. Basicamente vai focar no "o quê" o sistema deve fazer e não "como". Examina atores, processos, regras, dados e cenários de uso para criar um entendimento compartilhado entre negócio e tecnologia.

#### Objetivo da análise
Tem o objetivo de capturar requisitos funcionais e não funcionais, definir o escopo e as fronteiras do sistema, modelar o domínio (conceitos, termos, relacionamentos), reduzir ambiguidades e riscos de entendimento.

#### Conceito de projeto 
Definição de solução técnica. Tem o foco no "como" o sistema vai atender os requisitos. Detalha estrutura, componentes, interações, persistência, integrações e decisões de arquitetura.

####  Objetivo do projeto
Ele transforma requisitos em uma arquitetura implementável, minimiza acoplamento, maximizar coesão e manutenibilidade; Escolhe padrões (GRASP, GoF), camadas e tecnologias, planeja performance, segurança, escalabilidade e observabilidade.

#### Quadro resumo
![[Quadro reusmo Conceito de Análise e Projeto.png]]

#### Análise estruturada

Abordagem funcional.

Características:
- Sistema decomposto em **processos**
    
- Uso de **Fluxo de Dados (DFD)**
    
- Modelagem por funções

Ferramentas principais:

- Modelo Entidade-Relacionamento (ER)
    
- Dicionário de Dados
    
- DFD (Diagrama de Fluxo de Dados)
    

Foco: “O que o sistema faz” em termos de transformação de dados.

## 1.2 Conceito de Análise e Projeto Orientado a Objetos 

Abordagem baseada em **objetos**.

#### Características:

- Modela entidades com:
    
    - Identidade
        
    - Estado
        
    - Comportamento
        
- Requisitos mapeados para:
    
    - Casos de uso
        
    - Classes
        
    - Cenários de interação

#### Vantagens:

- Baixo acoplamento
    
- Alta coesão
    
- Melhor reutilização (herança, composição)



### Conceito de Objeto

Objeto é a unidade fundamental da orientação a objetos.

#### Um objeto:

- Representa algo do mundo real (ou abstrato)
    
- Possui **atributos** (dados)
    
- Possui **operações** (métodos)
    
- Possui **estado** (valores atuais dos atributos)
    
- Possui **identidade própria**
    

#### Estrutura do objeto:

- **Atributos →** definem o estado
    
- **Operações →** manipulam o estado
    
- **Interface →** conjunto de operações acessíveis
    


Exemplo:  

Objeto: Funcionário  
Atributos: nome, salário  
Operações: calcularSalário(), calcularIR()

## Síntese Geral até o Slide 29 (1.1 Conceito de Análise e Projeto | 1.2 Conceito de Análise e Projeto Orientado a Objetos )

A primeira parte da disciplina estabelece:

1. Diferença clara entre **Análise (problema)** e **Projeto (solução)**
    
2. Duas abordagens principais:
    
    - Estruturada (processos e dados)
        
    - Orientada a Objetos (objetos e responsabilidades)
        
3. Introdução ao conceito central da OO: **Objeto**
    
    - Estado
        
    - Comportamento
        
    - Identidade
        
    - Interface