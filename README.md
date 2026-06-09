# DOCUMENTO DA APLICAÇÃO

<details>
  <summary><strong> Sumário</strong></summary>

- [1. Introdução](#1-introdução)
  - [Objetivos](#-objetivos)
- [2. Requisitos](#2-requisitos)
- [3. Modelo de casos de uso](#3-modelo-de-casos-de-uso)
- [4. Banco de Dados](#4-banco-de-dados)
- [5. Diagrama de classes](#5-diagrama-de-classes)
- [6. Estudo de viabilidade](#6-estudo-de-viabilidade)
- [7. Regras de negócio (Modelo canvas)](#7-regras-de-negócio-modelo-canvas)
- [8. Design](#8-design)
- [9. Personas](#9-personas)
- [10. Protótipo](#10-protótipo)
- [11. Aplicação](#11-aplicação)
- [12. Análise de Desempenho Estatístico](#12-análise-de-desempenho-estatístico)
- [13. Considerações Finais](#13-considerações-finais)
- [14. Referências](#14-referências)

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

O documento de requisitos de uma aplicação é um fator fundamental para seu desenvolvimento, pois permite catalogar e compreender quais características são essenciais para o sistema a ser desenvolvido com base nas funcionalidades e restrições propostas pelo cliente, assim possibilitando a entrega de um produto padronizado e satisfatório conforme as especificações solicitadas.

### Histórias do usuário

• Como usuário não cadastrado, quero poder acessar a página inicial do site para que eu possa entender do que se trata.

• Como usuário não cadastrado, quero poder visualizar os profissionais e seus serviços na plataforma para que eu entenda os tipos de serviços oferecidos.

• Como usuário não cadastrado, quero poder acessar a sessão "Cadastro" do site para me cadastrar na plataforma.

• Como usuário cadastrado, quero poder fazer login na plataforma para acessar minha conta.

• Como usuário cadastrado, quero poder editar minhas informações de perfil para manter meus dados atualizados.

• Como cliente cadastrado, quero poder buscar profissionais para encontrar prestadores de serviços.

• Como cliente cadastrado, quero poder solicitar um orçamento para um profissional.

• Como cliente cadastrado, quero poder agendar um serviço com um profissional.

• Como cliente cadastrado, quero poder visualizar o histórico de serviços realizados para acompanhar meus atendimentos anteriores.

• Como profissional cadastrado, quero poder criar e gerenciar meu perfil profissional para apresentar meus serviços aos clientes.

• Como profissional cadastrado, quero poder receber solicitações de orçamento para responder aos clientes interessados.

• Como profissional cadastrado, quero poder gerenciar meus agendamentos para organizar meus serviços.

• Como profissional cadastrado, quero poder visualizar o histórico de serviços realizados para acompanhar meus atendimentos.

## • Requisitos funcionais

Os requisitos funcionais de uma aplicação são especificações definidas na etapa de elicitação do software, que ocorre durante o levantamento de requisitos. Seu propósito é fornecer à equipe de desenvolvimento as características especificas, restrições e funcionalidades que o sistema possui durante certas circunstâncias, estabelecendo assim as bases para o desenvolvimento de um produto que atende as necessidades do cliente.

### Usuários não cadastrados

#### RF 1 - Mostrar página inicial

Exibir página inicial do sistema com informações gerais e os serviços oferecidos.

#### RF 2 - Visualizar profissionais

Permitir que usuários não cadastrados possam visualizar profissionais disponíveis no sistema.

#### RF 3 - Cadastrar usuários

Permitir que usuários possam se cadastrar ao fornecer dados pessoais como nome, e-mail, telefone, e CNPJ no caso de profissionais.

### Usuários Cadastrados

#### RF 4 - Realizar login

Permitir que o usuário acesse sua conta informando e-mail e senha previamente cadastrados.

#### RF 5 - Editar perfil

Permitir que o usuário altere suas informações de perfil.

### Usuários Cadastrados(Clientes)

#### RF 6 - Buscar profissionais

Permitir que o usuário busque profissionais disponíveis no sistema.

#### RF 7 - Visualizar perfil do profissional

Permitir que o usuário visualize o perfil do profissional, incluindo descrição e serviços oferecidos.

#### RF 8 - Solicitar Orçamento

Permitir que o usuário envie uma solicitação de orçamento ao profissional informando detalhes do serviço desejado.

#### RF 9 - Agendar Serviço

Permitir que o usuário agende o serviço após a aprovação do orçamento.

#### RF 10 - Visualizar histórico de serviços

Permitir que o usuário visualize o histórico de serviços solicitados, incluindo data, valores e status do serviço.

### Usuários Cadastrados(Profissionais)

#### RF 11 - Criar perfil profissional

Permitir que o profissional configure seu perfil profissional.

#### RF 12 - Cadastrar serviços

Permitir que o usuário cadastre os serviços oferecidos na plataforma.

#### RF 13 - Gerenciar solicitações de orçamento

Permitir que o profissional visualize e responda solicitações de orçamento.

#### RF 14 - Enviar orçamento

Permitir que o usuário envie um valor estimado do serviço com base nos dados oferecidos pelo cliente na solicitação de orçamento.

#### RF 15 - Gerenciar agendamentos

Permitir que o profissional possa visualizar e gerenciar os serviços agendados.

#### RF 16 - Visualizar histórico de serviços

Permitir que o profissional visualize serviços concluídos e seus respectivos valores.

## • Requisitos não funcionais

Os requisitos não funcionais referem-se aos aspectos do sistema que garantem sua qualidade.

#### RNF 1 - Usabilidade

O sistema deve possuir uma interface simples e intuitiva, permitindo que clientes e profissionais tenham facilidade para navegar e utilizem as funcionalidades oferecidas sem dificuldades.

#### RNF 2 - Desempenho

O sistema deve apresentar respostas rápidas as ações dos usuários, como busca de profissionais, envio de orçamentos e carregamento de páginas.

#### RNF 3 - Segurança

O sistema deve garantir a proteção das informações do usuário.

#### RNF 4 - Compatibilidade

A aplicação deve funcionar em diferentes dispositivos e navegadores.

#### RNF 5 - Disponibilidade

O sistema deve estar disponível para acesso dos usuários na maior parte do tempo.

# 3. Modelo de casos de uso

O diagrama de casos de uso serve de representação visual para mostrar as funcionalidades principais de um sistema. Ele descreve as interações entre os atores (usuários) e o sistema por meio de "casos de uso", que são ações ou serviços oferecidos.

![Preview][uscs]

# 4. Banco de Dados
O banco de dados foi desenvolvido de acordo com as necessidades da aplicação, garantindo que as informações fossem organizadas de forma estruturada e consistente, respeitando os relacionamentos entre os dados.

Foi utilizado um banco de dados relacional (SQL), que permite maior controle sobre a integridade das informações por meio de tabelas, chaves e relações. Esse modelo é amplamente utilizado em aplicações que exigem dados bem definidos e organizados.

Para facilitar a comunicação entre a aplicação e o banco de dados, foi utilizado o Prisma. Essa ferramenta atua como um ORM (Object-Relational Mapping), permitindo realizar operações no banco de forma mais simples, utilizando código em vez de comandos SQL diretos. Além disso, o Prisma auxilia na definição do modelo de dados, na criação das tabelas e na manutenção da estrutura do banco, tornando o desenvolvimento mais organizado e eficiente.
![Preview][dtbs]

# 5. Diagrama de classes
![Preview][dcls]

# 6. Estudo de viabilidade

O estudo de viabilidade é uma análise realizada para determinar se um projeto é ou não viavel. Para isso, são considerados aspectos técnicos, financeiros, de mercado e operacionais, buscando identificar dificuldades antes do inicio do desenvolvimento.

### VIABILIDADE TÉCNICA

Através da viabilidade técnica é possivel identificar se um projeto pode ser desenvolvido com as tecnologias e conhecimentos disponiveis pela equipe responsável, verificando as ferramentas utilizadas, infraestrutura necessária e a capacidade técnica dos desenvolvedores.

No caso deste projeto, a equipe é formada por alunos do curso de Desenvolvimento de Software Multiplataforma, que possuem o conhecimento técnico necessário para dar suporte ao projeto, utilizando tecnologias como React, Node.js e JavaScript, além disso, serão utilizadas as plataformas GitHub para controle de versão e Figma para prototipação.

### VIABILIDADE FINANCEIRA

A viabilidade financeira analisa os custos envolvidos no desenvolvimento e na implementação e manutenção do projeto, além de considerar possíveis formas de retorno financeiro.

Os custos de desenvolvimento para este projeto são reduzidos, pois o sistema será desenvolvido por estudantes utilizando ferramentas gratuitas.
Dessa forma, considerando o baixo custo de desenvolvimento, o projeto apresenta viabilidade financeira dentro do contexto proposto.

### VIABILIDADE DE MERCADO

A viabilidade de mercado analisa se existe demanda para o projeto proposto, considerando o público alvo, diferencial da solução e as necessidades existentes no mercado.
Na área da construção civil e de serviços manuais, é comum que profissionais autônomos ou pequenas empresas tenham dificuldade em divulgar seus serviços e alcançar novos clientes, ao mesmo tempo, clientes interessados nesses serviços muitas vezes podem ter dificuldades para encontrar profissionais confiáveis e comparar diferentes opções disponíveis.

A proposta deste projeto é funcionar como um marketplace digital, intuitivo e eficiente para que profissionais apresentem seus serviços enquanto clientes podem buscar prestadores, solicitar orçamentos e agendar serviços de forma prática.
Assim, é entendido que existe uma oportunidade de mercado para este sistema.

### VIABILIDADE OPERACIONAL

A viabilidade operacional identifica se o sistema pode ser utilizado de forma prática pelos usuários finais, considerando a facilidade de uso do sistema e adaptação ao contexto que sera aplicado.

A plataforma foi idealizada para ser acessível por meio de navegadores web, podendo ser utilizada tanto em computadores como em dispositivos móveis. A interface tem como objetivo a simplicidade e clareza nas informações, permitindo que tanto profissionais e clientes possam usar o sistema sem grandes dificuldades.
Essas características tornam o sistema operacionalmente viável e adequado para o público alvo.

### CONCLUSÃO

Com base na análise realizada, podemos concluir que o projeto apresenta viabilidade técnica, financeira, de mercado e operacional dentro do contexto que será desenvolvido. As tecnologias necessárias para o desenvolvimento são acessíveis e dominadas pela equipe, os custos são reduzidos e existe potencial para aplicação da proposta para facilitar a conexão entre clientes e profissionais na área da construção civil.

O projeto se mostra viável para desenvolvimento e implementação como uma solução prática para intermediar a relação entre clientes e profissionais prestadores de serviços.

# 7. Regras de negócio (Modelo canvas)

![preview][mdn]

### O QUE SERÁ REALIZADO?

**Proposta de Valor**

Uma aplicação web que funciona como uma plataforma prática e acessível, conectando clientes a profissionais da área da construção civil. O sistema permite a busca, seleção e contratação de serviços como reformas, manutenção e obras, oferecendo avaliações, facilidade de uso e maior segurança na escolha de profissionais qualificados.

### COMO SERÁ REALIZADO?

**Parcerias-Chave**

Profissionais autônomos da construção civil e lojas de materiais de construção (opcional).

**Atividades-Chave**

Desenvolver uma plataforma digital que permite o cadastro de clientes e profissionais. O sistema possibilita a busca por serviços, visualização de perfis, solicitação de atendimentos e avaliação dos profissionais. Além disso, haverá manutenção contínua da aplicação para garantir desempenho, segurança e boa experiência do usuário.

**Recursos-Chave**

Tempo e dedicação da equipe, documentação do sistema, ferramentas de desenvolvimento, banco de dados e infraestrutura para hospedagem da aplicação.

### PARA QUEM SERÁ REALIZADO?

**Relacionamento com Clientes**

Contato via e-mail ou plataforma, sistema de avaliações e feedback dos usuários, além de notificações sobre solicitações e serviços.

**Canais de Distribuição**

A plataforma estará disponível via aplicação web, podendo ser acessada por dispositivos móveis, além de divulgação em redes sociais e instituições de ensino.

**Segmento de Clientes**

Pessoas que necessitam de serviços domésticos ou reformas, proprietários de imóveis, pequenos negócios e profissionais autônomos da construção civil.

### QUANTO CUSTARÁ?

**Estrutura de Custos**

Desenvolvimento e manutenção da aplicação web, hospedagem, tempo da equipe, suporte ao usuário e possíveis custos com divulgação.

**Fontes de Receita**

O projeto pode ser inicialmente sem fins lucrativos, com possibilidade futura de monetização através de comissão por serviços realizados, planos para profissionais ou destaque de perfis dentro da plataforma.

# 8. Design
### Paleta de cores
As cores do projeto foram organizadas em funções específicas dentro da interface. A cor primária é utilizada como base visual, transmitindo confiança e estabilidade. A cor secundária complementa a identidade, sendo aplicada em elementos de apoio e interação. A cor terciária é usada para destaque, direcionando a atenção do usuário para ações importantes. Já a cor neutra é aplicada em textos e elementos secundários, garantindo legibilidade e equilíbrio visual.<br>
![#1A365D](https://img.shields.io/badge/-1A365D-1A365D?style=flat-square)
![#2C7A7B](https://img.shields.io/badge/-2C7A7B-2C7A7B?style=flat-square)
![#F6AD55](https://img.shields.io/badge/-F6AD55-F6AD55?style=flat-square)
![#4A5568](https://img.shields.io/badge/-4A5568-4A5568?style=flat-square)

### Fonte
Para este projeto, foi escolhida a fonte Inter, uma tipografia sem serifa desenvolvida para interfaces digitais. Sua estrutura favorece a leitura em telas, oferecendo boa legibilidade em diferentes tamanhos e dispositivos.<br>
![Preview][fnt]

### Logo
A logo do projeto é um logotipo composto pelo nome do sistema "Contrataqui", utilizando as cores ![#1A365D](https://img.shields.io/badge/-1A365D-1A365D?style=flat-square) e ![#000000](https://img.shields.io/badge/-000000-000000?style=flat-square) com a fonte INTER.

# 9. Personas
![Preview][prsn]

![Preview][prsn2]

# 10. Protótipo
O protótipo do projeto foi criado através da plataforma de design e prototipagem Figma. O link segue logo à baixo.

[Protótipo Contrataqui](https://www.figma.com/design/nxjbL4eBC2eBWWsnFE1j9q/Prot%C3%B3tipo---PI-IV?node-id=0-1&t=GeNyzYo015Sem4jL-1 "hover text")

# 11. Aplicação
A página para o GitHub do projeto se encontra no link abaixo:

[Aplicação Contrataqui](https://github.com/leobalbino2/Projeto-Integrador-IV "hover text")

## 12. Análise de Desempenho Estatístico

A partir dos indicadores extraídos dos dashboards de gestão e do perfil profissional, foram processadas métricas quantitativas para validar a eficiência operacional e o comportamento financeiro da plataforma:

### Base de Dados de Referência
Os valores abaixo representam a amostra real coletada dos indicadores de performance utilizados para as projeções e cálculos deste capítulo:

1.  **Fluxo Mensal de Demandas (Jan-Jun)**: `[3, 4, 5, 5, 5, 8]`
2.  **Faturamento por Tipo de Serviço**: `[4200.00, 3800.00, 3500.00, 3100.00, 2800.00]`
3.  **Rentabilidade dos Profissionais de Destaque**: `[8100.00, 7700.00, 3150.00, 2600.00]`
4.  **Índices de Satisfação (Avaliações)**: `[4.3, 4.5, 4.7, 4.5]`
5.  **Status Operacional dos Contratos**: `Concluído (25), Aguardando (3), Aceito (1), Em Execução (1)`

### 12.1 Indicadores de Centralidade (Média, Mediana e Moda)

A tabela abaixo sintetiza o comportamento típico das cinco variáveis monitoradas:

| Variável | Classificação | Média | Mediana | Moda | Configuração |
| :--- | :--- | :---: | :---: | :---: | :---: |
| **Fluxo Mensal de Demandas** | Quantitativa Discreta | 5,00 | 5,00 | 5 | Unimodal |
| **Faturamento por Serviço** | Quantitativa Contínua | R$ 3.480,00 | R$ 3.500,00 | N/A | Amodal |
| **Rentabilidade de Profissionais** | Quantitativa Contínua | R$ 5.387,50 | R$ 5.425,00 | N/A | Amodal |
| **Índices de Satisfação** | Quantitativa Contínua | 4,50 | 4,50 | 4,5 | Unimodal |
| **Status Operacional** | Qualitativa Nominal | N/A | N/A | 'Concluído' | Unimodal |

#### Leitura dos Resultados
*   **Demanda Mensal**: O equilíbrio entre média e mediana em 5 unidades revela um ecossistema estável, com crescimento orgânico.
*   **Variáveis Financeiras**: A ausência de moda (amodal) no faturamento é comum em mercados de serviços, onde os orçamentos são personalizados e variados.
*   **Qualidade Percebida**: A centralidade em 4,5 estrelas posiciona a plataforma em um patamar de excelência no atendimento.
*   **Eficiência de Entrega**: A predominância do status 'Concluído' confirma que o fluxo de trabalho está sendo finalizado com sucesso na maioria dos casos.

---

### 12.2 Estudo de Dispersão e Variabilidade Relativa

Análise da oscilação dos dados em relação ao comportamento médio do sistema:

| Variável | Média | Variância | Desvio Padrão | Coef. de Variação (CV) |
| :--- | :---: | :---: | :---: | :---: |
| **Fluxo Mensal de Demandas** | 5,00 | 2,80 | 1,67 unidades | 33,47% |
| **Faturamento por Serviço** | 3.480,00 | 307.000,00 | R$ 554,08 | 15,92% |
| **Rentabilidade de Profissionais** | 5.387,50 | 8.493.958,33 | R$ 2.914,44 | **54,10%** |

#### Diagnóstico da Variabilidade
*   **Ponto de Maior Oscilação**: A **Rentabilidade de Profissionais (54,10%)** apresenta a maior flutuação, o que é natural em sistemas de marketplace onde profissionais "top-tier" tendem a escalar ganhos muito acima da média geral.
*   **Ponto de Maior Estabilidade**: O **Faturamento por Serviço (15,92%)** mostra-se o indicador mais homogêneo, sugerindo uma padronização saudável nos preços praticados por categoria.

---

### 12.3 Conclusões Baseadas em Evidências Visuais

#### Correlação Preço vs. Excelência
Através da análise de dispersão, observa-se que o valor investido no contrato não condiciona a nota final. Serviços de entrada e serviços premium mantêm o mesmo nível de satisfação, validando a integridade da rede de profissionais.

#### Evolução Temporal
Os dados apontam para uma **curva ascendente de adesão**, com o volume de novos contratos dobrando entre o início e o fim do período analisado.

#### Saúde do Portfólio de Contratos
A taxa de conclusão de 83,3% indica um baixo índice de atrito operacional, reforçando a confiabilidade do modelo de negócio.


# 13. Considerações Finais
O quarto semestre do projeto trouxe desafios que impactaram diretamente o desenvolvimento da plataforma de intermediação de serviços Contrataqui. Um dos principais pontos foi a reformulação do projeto, após o entendimento de que o escopo estava limitando uma construção mais ampla do sistema, impedindo o cumprimento completo dos requisitos propostos para este semestre. Além disso, houve a necessidade de aprofundar o conhecimento técnico da equipe nas tecnologias utilizadas, como React, Node.js, TypeScript e Tailwind CSS, especialmente na integração entre Frontend e Backend.

Apesar das dificuldades, o projeto conseguiu atingir os objetivos estabelecidos para o semestre, estabelecendo também uma base sólida para a implementação de funcionalidades futuras e para a finalização das partes restantes, visando seu funcionamento completo.

# 14. Referências

__INTER.__ Fonte tipográfica sans-serif utilizada para interfaces digitais.<br>
Disponível em: https://rsms.me/inter/.<br>
Acessado em: 24 de maio de 2026.<br><br>

__CLOUDINARY.__ Plataforma de gerenciamento de imagens e vídeos em nuvem.<br>
Disponível em: https://cloudinary.com/.<br>
Acessado em: 24 de maio de 2026.<br><br>

__TAILWIND CSS.__ Framework CSS utilitário para construção de interfaces modernas.<br>
Disponível em: https://tailwindcss.com/.<br>
Acessado em: 24 de maio de 2026.<br><br>

__DOCKER.__ Plataforma para desenvolvimento, envio e execução de aplicações em contêineres.<br>
Disponível em: https://www.docker.com/.<br>
Acessado em: 24 de maio de 2026.<br><br>

__TRIIDER.__ Plataforma online para contratação de serviços residenciais.<br>
Disponível em: https://www.triider.com.br/.<br>
Acessado em: 24 de maio de 2026.<br><br>

__THUMBTACK.__ Plataforma online para contratação de profissionais e serviços locais.<br>
Disponível em: https://www.thumbtack.com/.<br>
Acessado em: 24 de maio de 2026.<br><br>

__CRONOSHARE.__ Plataforma online para conexão entre clientes e prestadores de serviços.<br>
Disponível em: https://www.cronoshare.com.br/.<br>
Acessado em: 24 de maio de 2026.<br><br>

__TRELLO.__ Plataforma de gestão de projetos e colaboração.<br>
Disponível em: https://trello.com/home.<br>
Acessado em: 22 de maio de 2026.<br><br>

__FIGMA.__ Plataforma de design colaborativo online.<br>
Disponível em: https://www.figma.com/.<br>
Acessado em: 11 de abril de 2026.<br><br>

__GITHUB.__ Plataforma de hospedagem de código-fonte e controle de versão.<br>
Disponível em: https://github.com/.<br>
Acessado em: 22 de maio de 2026.<br><br>

__DRAW.IO.__ Plataforma online para criação de diagramas de forma simples e colaborativa.<br>
Disponível em: https://app.diagrams.net.<br>
Acessado em: 13 de abril de 2026.

[uscs]: imgs/blackusecase.jpeg
[mdn]: imgs/image.png
[prsn]: imgs/personaMarcio.jpeg
[prsn2]: imgs/personaMariana.jpeg
[plt]: imgs/paletaCores2.png
[fnt]: imgs/font.jpeg
[dcls]: imgs/diagramaClasses.png
[dtbs]: imgs/database.jpeg
