# Sistema de Locação de Quadras Esportivas

## 1. Introdução

Este projeto implementa um sistema de gerenciamento de aluguel de quadras esportivas, desenvolvido em Java com os princípios da Programação Orientada a Objetos (POO). Utiliza o framework ORMLite para persistência de dados em um banco SQLite e JavaFX para a interface gráfica, seguindo o padrão Model-View-Controller (MVC). O sistema permite que locadores cadastrem quadras e consultem reservas, enquanto locatários podem buscar quadras disponíveis, realizar agendamentos e cancelar reservas.

## 2. Funcionalidades 

- Cadastro de usuários (Locador e Locatário) com interface gráfica.
- Aute-nticação de usuários por número (CPF/telefone) e senha.
- Visualização de quadras cadastradas (Locador) e quadras disponíveis (Locatário, com dados fictícios).
- Cadastro de quadras, consulta de disponibilidade e reservas (em desenvolvimento). 

## 3. Requisitos

### 3.1 Requisitos Funcionais
- Cadastro de usuários (Locador e Locatário)com informações básicas (número, nome, senha, telefone) e, para locatários, dados de quadra (temporário).
- Autenticação de usuários via login.
- Visualização de quadras cadastradas (Locador) e disponíveis (Locatário).
- Cadastro de quadras esportivas (em desenvolvimento).
- Consulta de disponibilidade de quadras (em desenvolvimento).
- Realização e cancelamento de reservas (em desenvolvimento).

### 3.2 Requisitos Não Funcionais
- Código modular, seguindo o padrão MVC e os princípios de POO (encapsulamento, herança, polimorfismo, abstração).
- Persistência de dados com SQLite e ORMLite.
- Interface gráfica intuitiva com JavaFX.
- Código organizado, reutilizável e bem documentado.

## 4. Tecnologias Utilizadas
- **Linguagem**: Java
- **Framework de Persistência**: ORMLite
- **Banco de Dados**: SQLite
- **Ferramentas**: Maven (ou outra ferramenta de build, se aplicável), PlantUML (para diagramas UML), BlueJ (para desenvolvimento).

## 5. Conceitos de POO aplicados
- Encapsulamento: Todos os atributos das classes são privados, acessados por getters e setters.
- Herança: As classes Locador e Locatario herdam atributos e métodos da classe base Usuario.
- Polimorfismo: O repositório de usuários (UsuarioRepositorio) é capaz de lidar com diferentes subclasses usando a mesma interface de manipulação.
- Abstração: A superclasse Usuario encapsula a estrutura comum dos usuários do sistema.

## 6. Diagramas UML

### 6.1 Diagrama de Classes
![Diagrama UML](https://www.plantuml.com/plantuml/png/nLRDRjms4BxhAOYSRCGRe5V3CE8u29h2CDAiw_k87EyIfJWgIIL6VnwcwA6dFeLVh2Dff9MuD7p88K0Ga3FVp7ppSKRUjp51I5tZglYhzIq4Q5H3dlG-K8CgXGwhIZk8KVqIEmYMr1-LKXjhpfNrgJ_whi50vsgRWlMxmSAXotj4luU5uVKEqqTpSZgbU1s7k-Gy5SJja9THYy0uczTLvnYkd4M8KJYjqDkULmuNwyHP0lwQLBWX3OR2g492Xm_aCUljJinvweCZ3ymA916wN6BZ6EBixw21Vkx015WwasqBrZs5FcTyRsDBtdv16x-Tj4JUv7Jo50N4eeKytPrjotbMhhxDFFB7uoRp54NC94xXDTv3WXeYZezXv7OBwm7Nv3tgPCcVgvzChQ_d-vQwe57u7SnCwrcWTXJnX3baY_SPMues4HydDYIkS-P95t8vKnzzmXs6Im79o8uWkHH1wP1hlXw08k2ao8cf6IgNuGLqG4XuqasSXC_fVEf1THSrX4yKYdkynaANq2VB-0nsfkRrbAYQo27uWsZNO22cGAmm_-ySoig6UfRZCnXBxxgKoCyUqI3tfSTqAmpky35ziEZCPAS6ZwsoD0NFTcJ-YKb-fM1cLmiU5mJktz6ZH1os9o-lwxl5jbzJKnE7NOogN4huDF5Zx5L0w1rryY8Hi1GB5GvJTfvFdZoBzJRPdX5FQN_VWpSEvsnhezVesBPQgRYl2OAHXyXVoDLk7kiRgD69iM_rs97w0umIz2r2xV3UujVU9vDuGpkkatyZ9LNsUH3hwi_5cSe_DjBT5kogswlK3G-rDhfkzwm0yjpV9e7cQB0UWwWWm_CT1BYbB_8KotwvlFLvYwMDUc53NXvDeJ4KBCmcZQmaL5tykTae6SBSA0zJ7PTHjDbSgbS_l9e_VbNXMyEO4aMHuYLOlYBbYAeyI0LWvIcX2dQtJueU5kqfTPM2hRj4KHtzgXYUNSuA6Llu4Q7Yqp-a4ZOjXQU_U-U0x28OFhOGW9sH_obFIejERohqHlMSScRFDyv9FtHUM_9Cqe3XZ0OLJ1kd-3mi6kD-6nWBjTQ1nZqvWo6-N3TNKYhVspZMUVgtpsbmhi6DAZFq-c1rUlgF2N8PvagXwToWY3finPk7nyOft-UmJUkmGP_0hFHuoyUkSVy3)

O diagrama de classes do sistema de locação de quadras esportivas representa a estrutura estática do projeto, detalhando as classes implementadas e suas relações. Ele ilustra a herança entre Usuario, Locador e Locatario, a composição entre UsuarioRepositorio e Database, e as interações dos controladores com o modelo, refletindo o padrão MVC. O diagrama destaca atributos e métodos principais, com notas indicando que os atributos localizacaoQuadra, tipoQuadra e horariosDisponiveis em Locatario são temporários e que alguns métodos de UsuarioRepositorio estão planejados, mas não implementados, fornecendo uma visão clara da organização e funcionamento do sistema no estado atual.

### 6.2 Diagramas de caso de uso 

![Diagrama UML](https://www.plantuml.com/plantuml/png/bP51JWCn34NtEOMNi2W7G5LLgOKL6ufWRoPkQp69AoSPeTw60t2ANeoC55Lj4nQpcyZ_VN_FNuQ86fFhJVXYVq151qwyT7iLHn0raJ7OHL5uaGwjwCKheopb_SOXaaDZYWncimNSFUEHHksE_Rqv8_NicbgXnH0L5Tv3ElraeeBRagR7QqAhU3iM7r8VytX3WNJ0KAtuu92mv-FP8i2Qmq7ywNSWhlKRAkhYsCZiE-el1URg9y33k3MRsAnPALdo7MFU18ymdzDt96yN2zEu_HfTevLRg4fN45BUSeTQJkDF7ZqitU2cr3iUqivOASvHgjc_Eutn4WcKT_i8icsL2F3am58WFqW_i2CVnP2tC98rNxKypQ4kTI9VEf_0B_DdSlqV)

O diagrama de casos de uso ilustra as interações principais entre os atores (Locador, Locatário e Sistema) e o sistema de locação de quadras esportivas, destacando as funcionalidades disponíveis e planejadas:

-- Atores:

- Locador: Usuário que cadastra e gerencia quadras esportivas, consultando reservas feitas por locatários.
- Locatário: Usuário que busca quadras disponíveis, realiza reservas e pode cancelá-las.
- Sistema: Responsável por validações automáticas, como autenticação, validação de dados e verificação de disponibilidade.
  
-- Casos de Uso:

- Fazer Login: Ambos os atores (Locador e Locatário) autenticam-se no sistema usando número (CPF/telefone) e senha. Este caso de uso se estende a "Validar Credenciais", onde o Sistema verifica as credenciais no banco de dados via UsuarioRepositorio.
- Cadastrar Usuário: Locadores e Locatários podem se cadastrar, fornecendo número, nome, senha, telefone e, para locatários, informações temporárias de quadra (localização, tipo, horários). -- Este caso se estende a "Validar Dados", onde o Sistema verifica se os campos obrigatórios estão preenchidos.
- Cadastrar Quadra (em desenvolvimento): Permite ao Locador cadastrar uma quadra esportiva, incluindo localização e tipo. Esta funcionalidade está planejada, mas não implementada (ausência da classe Quadra e do formulário NovaQuadra.fxml).
- Consultar Reservas (em desenvolvimento): Permite ao Locador visualizar as reservas feitas em suas quadras. Está planejado, mas depende da implementação das classes Reserva e Horario.
- Visualizar Quadras Disponíveis: Locatários podem ver uma lista de quadras disponíveis, atualmente implementada com dados fictícios no DashboardLocatarioController.
- Realizar Reserva (em desenvolvimento): Locatários selecionam uma quadra, data e horário para reservar. Este caso se estende a "Verificar Disponibilidade", onde o Sistema valida conflitos de horário. Ainda não implementado.
- Cancelar Reserva (em desenvolvimento): Locatários podem cancelar reservas existentes. Depende da implementação da classe Reserva.

### 6.3 Diagrama De Sequencia

![Diagrama UML](https://www.plantuml.com/plantuml/png/VP6_RjH04CRxUOfFgHA9GEy2HJeeaD8G2VevxzpTYlMEcLb7l0wYeiWBqFh5M5zoXx0lxjRZxyzlTk-yi9MXI-JVOkxPk4EdMTk3QISeDWWHjqKDzzfo5KUbAYknZJtdWglcNlSnRpGNqvJ4hi2EsMpc-C1-s2fRE4VEx2k2UTON7wR_3zAhnwBrU4nOZXSCXRViSbIVFeZEXRXzFz-YmQViOe8y_kd450ANV62QwIRhihy13qLoHM2xpiCKyERPVqDBTSquKpNuAXPtrOZM94Xk8qUdqs_SljBt8FMG6IO-fC91B_PSsdDwzdSxJYx4gM3phnMFuyyK0pi1oxLN7wx1XirapmWd5M7LCIMUnmq-_eXRmVU1Wx4ZHEyrZq-F4XtNzNRA-5GH_OQaSl_77FEIUhL3p9Ga1t0gH5cBmEB-KA2xLM02Fh_WIGsQ6k7ZBqNWe8uJf4uSUx7Zi9UawCRVHOEYVRuXUqbvUuIO-edkwd7eqby0)

O diagrama de sequência detalha o fluxo da operação de reserva. Ele inclui o Locatário, as interfaces (LoginController, DashboardLocatarioController), o UsuarioRepositorio e o banco de dados (Database). O diagrama reflete o fluxo planejado, com validação de login, busca de quadras, seleção de horário e confirmação de reserva. 

## 7. Implementação das Classes

- Usuario: Classe base que representa usuários, mapeada para a tabela usuarios com atributos id, numero, nome e senha.
- Locador: Herda de Usuario, mapeada para locadores, com atributo adicional telefone.
- Locatario: Herda de Usuario, mapeada para locatarios, com atributos adicionais telefone, localizacaoQuadra, tipoQuadra e horariosDisponiveis (temporários, a serem movidos para Quadra e Horario).
- Database: Gerencia a conexão com o banco SQLite usando ORMLite.
- UsuarioRepositorio: Realiza operações CRUD (atualmente implementa create, buscarPorNumero, autenticar; métodos update, delete, loadFromId, loadAll estão planejados).
- Controladores: CadastroController, DashboardLocadorController, DashboardLocatarioController e LoginController gerenciam a lógica de interação com a interface JavaFX.

## 8. Testes e Processo de Desenvolvimento

O processo de desenvolvimento do sistema seguiu etapas bem definidas, mesmo com escopo parcial:
  
### 8.1 Modelagem
  
A modelagem do sistema foi realizada utilizando diagramas UML, com foco na representação clara das entidades, seus atributos, métodos e relações. 
Os diagramas de classes e de casos de uso foram fundamentais para validar o entendimento das funcionalidades esperadas.
  
### 8.2 Testes Realizados
  
Os testes realizados incluíram:
-	Cadastro e listagem de usuários de diferentes tipos (Locador e Locatário);
-	Verificação da persistência no banco de dados SQLite usando ORMLite;
-	Testes de carregamento por ID para assegurar o funcionamento correto do polimorfismo;
-	Testes de herança, utilizando a superclasse Usuario para manipular objetos Locador e Locatario.
  
### 8.3 Implementação Incremental
  
O desenvolvimento seguiu uma abordagem incremental:
-	Primeiramente foram criadas as entidades principais (Usuario, Locador, Locatario);
-	Em seguida, foi construída a infraestrutura de persistência (Database e UsuarioRepositorio);
-	Por fim, foram realizados testes diretos no código Java para verificar a integridade dos dados e o funcionamento da lógica de CRUD. 
Mesmo que as funcionalidades de reserva ainda não tenham sido totalmente implementadas, a estrutura construída permite sua extensão com facilidade.

## 9. Como usar

### 9.1 Login

- Abra o sistema e insira seu número (CPF ou telefone) e senha na tela de login.
- Clique em "Cadastrar-se" para criar um novo usuário.

### 9.2 Cadastro de Usuário

- Na tela de cadastro, selecione o tipo de usuário (Locador ou Locatário).
- Preencha os campos: número, nome, telefone, senha. Para locatários, informe localização, tipo de quadra (Futebol, Tênis, Vôlei, Basquete, Poliesportiva) e horários disponíveis (temporário, a ser movido para Quadra).
- Clique em "Cadastrar" para salvar. Um alerta confirma o sucesso ou exibe erros.

### 9.3 Dashboard do Locador

- Acesse a lista de quadras cadastradas.
- Botões "Atualizar Lista" e "Alugar Quadra Selecionada" estão em desenvolvimento.
- Clique em "Sair" para voltar ao login.

### 9.4 Dashboard do Locatário

- Visualize quadras disponíveis em um painel rolável.
- Use o botão "Adicionar Nova Quadra" para abrir um formulário (em desenvolvimento).
- Clique em "Sair" para voltar ao login.

## 10. Conclusão

O sistema de locação de quadras esportivas, desenvolvido em Java com o padrão MVC, ORMLite para persistência em SQLite e JavaFX para a interface gráfica, implementa com sucesso as funcionalidades de cadastro e autenticação de usuários (Locador e Locatário), além da visualização de quadras com dados fictícios. A aplicação demonstra a aplicação dos princípios de Programação Orientada a Objetos, como herança, encapsulamento, polimorfismo e abstração, e estabelece uma base sólida para futuras expansões. A estrutura modular e os diagramas UML fornecem uma visão clara do projeto, garantindo organização e facilitando a manutenção. Apesar de algumas funcionalidades, como gerenciamento de quadras e reservas, ainda estarem em desenvolvimento, o sistema atual atende aos requisitos iniciais de autenticação e gerenciamento de usuários, representando um avanço significativo no objetivo de facilitar a locação de quadras esportivas.

## 11. Proximos passos
  
