# DOCUMENTO DA APLICAÇÃO

<details>
  <summary><strong>📑 Sumário</strong></summary>

- [1. Introdução](#1-introdução)
  - [Objetivos](#-objetivos)
- [2. Requisitos](#2-requisitos)
- [3. Modelo de casos de uso](#3-modelo-de-casos-de-uso)
- [4. Banco de Dados](#4banco-de-dados)
- [5. Diagrama de classes](#6-diagrama-de-classes)
- [6. Estudo de viabilidade](#7-estudo-de-viabilidade)
- [7. Regras de negócio (Modelo canvas)](#8-regras-de-negócio-modelo-canvas)
- [8. Design](#9-design)
- [9. Personas](#9-personas)
- [10. Protótipo](#10-protótipo)
- [11. Aplicação](#11-aplicação)
- [12. Considerações Finais](#12-considerações-finais)
- [13. Referências](#11-referências)

</details>

# 1. Introdução
Nos últimos anos, a forma como empresas do setor da construção civil se apresentam ao mercado mudou bastante. Ter um site deixou de ser algo opcional e passou a ser parte essencial de como um negócio é percebido pelos clientes, principalmente em áreas mais técnicas como a de estruturas metálicas, onde o cliente precisa confiar no trabalho antes mesmo de fechar qualquer contrato.

Pensando nisso, este projeto integrador propõe o desenvolvimento de um site para uma empresa do ramo de construção de estruturas metálicas. A ideia surgiu de uma necessidade real: a empresa não contava com uma presença digital organizada, e processos como o contato com clientes e a solicitação de orçamentos aconteciam de forma manual e sem padronização.

O site foi desenvolvido para resolver isso de forma prática. Por ele, clientes podem conhecer os serviços e obras da empresa e solicitar orçamentos diretamente pela plataforma. Já o administrador conta com uma área restrita para gerenciar as solicitações recebidas e acompanhar informações financeiras do negócio. O objetivo não é só criar uma vitrine digital, mas oferecer uma ferramenta que realmente facilite o dia a dia da empresa e melhore a experiência de quem busca seus serviços.

## • Objetivos

### Geral 
Desenvolver uma aplicação web para uma empresa do ramo de estruturas metálicas, com o objetivo de ampliar sua presença digital e otimizar o processo de solicitação e gerenciamento de orçamentos. A plataforma permitirá que clientes conheçam os serviços oferecidos pela empresa e realizem solicitações de orçamento de forma prática, enquanto o administrador poderá acompanhar e organizar essas solicitações por meio de uma área de gerenciamento.

### Específicos 
• Estruturar uma plataforma digital que apresente informações institucionais da empresa, seus serviços e projetos realizados, facilitando a comunicação com potenciais clientes.

• Implementar um sistema de solicitação de orçamentos online, permitindo que usuários enviem informações sobre seus projetos de maneira organizada e padronizada.

• Desenvolver uma área administrativa restrita para gerenciamento das solicitações recebidas, possibilitando acompanhar orçamentos aprovados, em andamento ou finalizados.

• Organizar registros de orçamentos e valores, auxiliando no controle e acompanhamento das atividades comerciais da empresa.

• Aplicar conceitos e tecnologias aprendidas no curso de Desenvolvimento de Software Multiplataforma para a criação de uma solução funcional e responsiva.

### Metodologia
O desenvolvimento da aplicação será realizado utilizando conceitos e práticas aprendidos ao longo do curso de Desenvolvimento de Software Multiplataforma (DSM). O projeto envolve a criação de uma plataforma web que integra interface visual, lógica de funcionamento e armazenamento de dados, permitindo o registro e gerenciamento de solicitações de orçamento.

### Linguagens de Programação 
Para o desenvolvimento da aplicação serão utilizadas tecnologias voltadas à construção de aplicações web modernas. O JavaScript será utilizado tanto no front-end quanto no back-end do sistema. No lado do cliente, será utilizada a biblioteca React, responsável pela criação da interface da plataforma, permitindo desenvolver páginas dinâmicas organizadas em componentes reutilizáveis. No lado do servidor, será utilizado o Node.js, responsável por processar as requisições da aplicação e realizar a comunicação com o banco de dados. Para o armazenamento das informações será utilizado o MongoDB, um banco de dados NoSQL que permite gerenciar os dados relacionados aos orçamentos e demais informações do sistema.

### Frameworks 
Para auxiliar no desenvolvimento da interface da aplicação será utilizado o Tailwind CSS, um framework de estilização que facilita a criação de layouts modernos, responsivos e visualmente consistentes. Seu uso permite maior agilidade no desenvolvimento do front-end e melhor organização dos estilos utilizados na aplicação.

### Prototipagem  
A plataforma de design e criação de interfaces Figma possibilitará a concepção de protótipos das telas do projeto permitindo visualizar modelos experimentais da aplicação web. 

### Metodologia Scrum 
Para o desenvolvimento do projeto será utilizada a metodologia ágil Scrum, que organiza o processo de desenvolvimento em ciclos curtos chamados Sprints. Cada Sprint corresponde a um período de trabalho no qual determinadas funcionalidades do sistema são planejadas, desenvolvidas e avaliadas.

# 2. Requisitos

# 3. Modelo de casos de uso

# 4. Banco de Dados

# 5. Diagrama de classes

# 6. Estudo de viabilidade
O estudo de viabilidade é uma análise realizada para determinar se um projeto é ou não viavel. Para isso, são considerados aspectos técnicos, financeiros, de mercado e operacionais, buscando identificar dificuldades antes do inicio do desenvolvimento.

### Viabilidade Tecnica
Através da viabilidade técnica é possivel identificar se um projeto pode ser desenvolvido com as tecnologias e conhecimentos disponiveis pela equipe responsável, verificando as ferramentas utilizadas, infraestrutura necessária e a capacidade técnica dos desenvolvedores.

No caso deste projeto, a equipe é formada por alunos do curso de Desenvolvimento de Software Multiplataforma, que possuem o conhecimento técnico necessário para dar suporte ao projeto, utilizando tecnologias como React, Node.js e JavaScript, além disso, serão utilizadas as plataformas GitHub para controle de versão e Figma para prototipação.

### Viabilidade Financeira
A viabilidade financeira analisa os custos envolvidos no desenvolvimento e na implementação e manutenção do projeto, além de considerar possíveis formas de retorno financeiro.
Os custos de desenvolvimento para este projeto são reduzidos, pois o sistema será desenvolvido por estudantes utilizando ferramentas gratuitas.
Dessa forma, considerando o baixo custo de desenvolvimento, o projeto apresenta viabilidade financeira dentro do contexto proposto.

### Viabilidade de Mercado
A viabilidade de mercado analisa se existe demanda para o projeto proposto, considerando o público alvo, diferencial da solução e as necessidades existentes no mercado.
Na área da construção civil e de serviços manuais, é comum que profissionais autônomos ou pequenas empresas tenham dificuldade em divulgar seus serviços e alcançar novos clientes, ao mesmo tempo, clientes interessados nesses serviços muitas vezes podem ter dificuldades para encontrar profissionais confiáveis e comparar diferentes opções disponíveis.
A proposta deste projeto é funcionar como um marketplace digital, intuitivo e eficiente para que profissionais apresentem seus serviços enquanto clientes podem buscar prestadores, solicitar orçamentos e agendar serviços de forma prática.
Assim, é entendido que existe uma oportunidade de mercado para este sistema.

### Viabilidade Operacional
A viabilidade operacional identifica se o sistema pode ser utilizado de forma prática pelos usuários finais, considerando a facilidade de uso do sistema e adaptação ao contexto que sera aplicado.
A plataforma foi idealizada para ser acessível por meio de navegadores web, podendo ser utilizada tanto em computadores como em dispositivos móveis. A interface tem como objetivo a simplicidade e clareza nas informações, permitindo que tanto profissionais e clientes possam usar o sistema sem grandes dificuldades.
Essas características tornam o sistema operacionalmente viável e adequado para o público alvo.

### Conclusão
Com base na análise realizada, podemos concluir que o projeto apresenta viabilidade técnica, financeira, de mercado e operacional dentro do contexto que será desenvolvido. As tecnologias necessárias para o desenvolvimento são acessíveis e dominadas pela equipe, os custos são reduzidos e existe potencial para aplicação da proposta para facilitar a conexão entre clientes e profissionais na área da construção civil.
O projeto se mostra viável para desenvolvimento e implementação como uma solução prática para intermediar a relação entre clientes e profissionais prestadores de serviços.

# 7. Regras de negócio (Modelo canvas)

# 8. Design

# 9. Personas

# 10. Protótipo

# 11. Aplicação

# 12. Considerações Finais

# 13. Referências
