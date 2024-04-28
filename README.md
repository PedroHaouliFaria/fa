# Design de Arquitetura

![arq.npg](https://github.com/PedroHaouliFaria/fa/blob/2b8ba722edb4e7ba6007ffee1642e4ba376bb145/mvc.drawio%20(2).png)

Link de download Draw.io: (https://drive.google.com/file/d/102zAVxQk8o2ngtVtC0O1nLK2QVSfj-hH/view?usp=sharing) 

# Template Readme para Arquitetura MVC em Markdown
- Nome da equipe: [Phoenix Learning Solutions]
- Nome do Projeto: [Ainda indefinido]
- Descrição: [Uma plataforma de apoio para os jogadores do Business Game fornecido pelo CESIM no estilo aplicação Web, visando proporcionar uma melhor sintonia entre os membros do jogo, facilitando a compreensão das necessidades e diferenças culturais e pessoais uns dos outros.]
- Arquitetura: MVC (Model-View-Controller)
- Ferramenta de Diagramação: [draw.io]

### Modelos (Models):
- No projeto nós temos como entidades o student profile, o qual reúne várias informações do bando de dados, como o ID, o nome, a foto, o país e a descrição do usuário. Além disso, temos a personal bio, com informações como ID, foto pessoal, tags, características e algumas respostas a questionários, depois temos o login information, com o email, ID e senha, a entidade member reviews também está presente, contando com atributos como ID, características, respostas, notas, observações e a foto. Por último temos a entidade de member reviews, que tem como atributos o ID, características, respostas, notas, observações e por fim a foto.
- As entidades tem relação de semelhança entre alguns dos seus atributos e a função delas se resume em se comunicar com o servidor e averiguar ou repassar informações aos controllers.

### Controladores (Controllers):
- Os controladores são três, sendo o primeiro o User, seguido pelo Rating process/reports e o task. Suas responsabilidades incluem listar, atualizar, salvar e procurar.
- O método listar é utilizado para recuperar uma lista de itens de um banco de dados ou de outra fonte de dados, o atualizar é utilizado para modificar um item existente, o salvar é utilizado para adicionar um novo item ao banco de dados ou outra fonte de dados e o procurar é utilizado para recuperar um único item com base em um critério de busca específico.

### Views (Views):
- As views do projeto são a team page, que serve como apresentação de dados, com uma interface interativa, também temos a student page, que serve como interface de usuário interativa e personalizável,, apresentando os dados inseridos, além dela, temos a login page, servindo para a validação de entrada do usuário, ademais temos a task page, que serve para apresentação de dados, feedback do usuário e uma navegação entre telas, depois temos a rating page, servindo de feedback page , apresentação de alguns dados e principalmenteuma interface interativa para o usuário e por fim temos a report page que serve de apresentação de feedback e dados.

### Infraestrutura:

- Em relação aos componentes, no quesito bancos de dados temos o PostgreSQL e  Render , APIs externas temos o node.js com o sails.js e outras dependências.
- A infraestrutura se integra à arquitetura MVC de modo que cada infraestrutura respresenta e da apoio a cada passo da arquitetura MVC, o model, o controller, o vier e os servidores, cada um tem a sua infraestrutura que é e deve se comunicar entre si para que a aplicação Web funcione.


### Justifique as escolhas feitas e como elas impactam o projeto.
#### Implicações da Arquitetura:

Os benefícios da arquitetura MVC nos quesitos citados incluem:

- Escalabilidade: Facilita a escalabilidade do sistema, permitindo que diferentes partes sejam escaladas separadamente conforme necessário.
- Manutenção: Simplifica a manutenção do código, pois cada componente tem responsabilidades bem definidas, facilitando a compreensão, modificação e correção de problemas.
- Testabilidade: Promove a testabilidade do código, permitindo a escrita de testes automatizados para verificar o comportamento dos modelos e controladores de forma isolada.
- Reutilização de código: Encoraja a reutilização de código, já que modelos e controladores podem ser reaproveitados em diferentes partes do sistema ou em projetos diferentes.
- Separação de interesses: Facilita a separação de interesses, tornando o código mais organizado e fácil de entender, além de promover a colaboração entre equipes especializadas.


