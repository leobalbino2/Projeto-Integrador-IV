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
Nos últimos anos, a forma como profissionais e empresas prestadoras de serviços se apresentam ao mercado passou por mudanças significativas. A presença digital deixou de ser um diferencial e tornou-se essencial para gerar visibilidade, credibilidade e facilitar o contato com clientes.

Entretanto, muitos profissionais autônomos e microempresas ainda dependem de processos informais, como mensagens por aplicativos e registros manuais, o que dificulta a organização de atendimentos, solicitações de orçamento e divulgação de seus serviços.

Diante desse cenário, este projeto integrador propõe o desenvolvimento de uma plataforma digital para intermediação e gestão de serviços. A solução permitirá que prestadores de serviços divulguem seus trabalhos e organizem seus atendimentos, enquanto clientes poderão localizar profissionais e solicitar orçamentos de forma centralizada.

A empresa Estrutucasa, atuante no setor de estruturas metálicas e registrada como Microempreendedor Individual (MEI), será utilizada como estudo de caso para validação das funcionalidades da plataforma em um contexto real de mercado.

## • Objetivos

### Geral 
Desenvolver uma plataforma web que facilite a conexão entre clientes e prestadores de serviços, oferecendo recursos para divulgação profissional, solicitação de orçamentos e gestão de atendimentos.

### Específicos 
• Estruturar uma plataforma digital que permita o cadastro de profissionais e a divulgação organizada de seus serviços e portfólios.

• Implementar um sistema de solicitação de orçamentos online, permitindo que clientes enviem demandas de forma padronizada e centralizada.

• Desenvolver um painel de gerenciamento para que profissionais acompanhem solicitações recebidas, status de atendimentos e histórico de serviços.

• Organizar categorias e subcategorias de serviços, facilitando a busca e a identificação de profissionais por área de atuação.

• Aplicar conceitos e tecnologias aprendidas no curso de Desenvolvimento de Software Multiplataforma na construção de uma solução funcional, responsiva e escalável.

### Metodologia
O desenvolvimento da aplicação será realizado com base nos conceitos e práticas aprendidos ao longo do curso de Desenvolvimento de Software Multiplataforma (DSM). O projeto envolve a criação de uma plataforma web que integra interface visual, lógica de funcionamento e armazenamento de dados, possibilitando o gerenciamento de usuários, serviços e solicitações de orçamento.

Inicialmente, serão levantados os requisitos do sistema e definidos os principais fluxos de uso da plataforma. Em seguida, será elaborado um protótipo das telas para validação da experiência do usuário.

### Linguagens de Programação 
Para o desenvolvimento da aplicação serão utilizadas tecnologias voltadas à construção de aplicações web modernas.

O JavaScript será utilizado tanto no front-end quanto no back-end do sistema. No lado do cliente, será utilizada a biblioteca React, responsável pela criação da interface da plataforma, permitindo o desenvolvimento de páginas dinâmicas organizadas em componentes reutilizáveis.

No lado do servidor, será utilizado o Node.js, responsável por processar requisições da aplicação e realizar a comunicação com o banco de dados.

Para o armazenamento das informações será utilizado o mySQL, um banco de dados NoSQL que permite gerenciar dados de usuários, serviços e solicitações de orçamento de forma flexível e eficiente.

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

### Viabilidade Técnica
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
