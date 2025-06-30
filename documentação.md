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
![Diagrama UML](https://www.plantuml.com/plantuml/png/nLRDRXj73BxhAOYS7CGoqAjW674S64sX6cda-ixTeQLfPuVR-N6C_ZnCqKFHGqzz1BrOTtQvFnhleeSSUj8C-P7pyOTSlVK1NOYLMVaVjQtHOGKLMouFZYk2u2AjLgL1x-5x7z5fXbzM06kjDg1jI4SRAtAyWLrmskvRIMCwlNko1vm8tkmfV51dhtiNRtnx5v-l1N7N-aseqT0FujDN1nkkABCGOUAKetU9LmuNgN3k3Nxhix3b4XMxBWk133sofIosUn7dhaT5RfWz42JHyq-iJGCn-cSiaR-Bg1nEbK7NCz83k-JJlzU-PgkVIFil9osMsvnExc86CGaXTtUlwta_9weKPcxvzSiWSnUpc3uvCzLuZm4BzDGLGydj3ayRl6HhgGoQxGQ-KKLvCznt75r9mcyK9rfBmDAmfxC91ncyJrIpru67rb38ejeqFFbIBkVmmGRQaxiIaBHi1vBBB2YCleRh29G4zXavKyLcI4zRWT8H1ZgBmgdd_Neu9L0HVOdk8xlPEJx5OWnaWsxm6UmSP3m7guBP4Dfa5MirIoFf51bQqXb6TUkuccoY0T3hhur9fTjg7_fqNus5ka65FZXkgXeS6qEo9bmnbE0JAitlOWXiHJFaFTU5vt0dKT_JSxZLP5GlvufUIcLGPpIxBbiVqVlFxDIWgj7IXC33EtuMYt5Yy-VBudwoOMwuAhWnk-mgSINc_PHrjjUEC2cAO2L5sAHYaeMnipTvjqlojTL19qPqrXRhW5OP6hoT2cr99iccO-mF1QDJKeYyGgOmmoXjiI0ZmXJgIqL81-nIa4B4mj23fiz99wsrvJqgplUokCfMaaXFFb7da2yuYMw7-YJQwn3RGfqAJTml9a3A_MKfA1jhr9QSP46Qvtz8m1q_IIccyJRFQvk5k3nHonFotwqfDDe7PtgJErPY2fU_hjSWJPWBfJ2hcNtFw_KLlFhgrR1mLpEx9c5cAEQfM83b8p9liLfkf0ouiXm8dDuV0l3Z93o0w-1q4GDxUF5FfYsxd84QxCmV5_37FnW2LJMxu-z9sI8LFL45dXnK_AHL8wtH8SGAeUq9WixjnOgiWiGkupXVts-FVmLEthhloZaeCfH-n-z5-xny7e1yIFHgWvP-mCRm72hqO1jXWz9LRQWY6v86B4Dv_4VfFGEcELwcjboTnkbjjALcYqOhLEH14M2_5e00qpP8k9-wMGKl14iwi57a_FAxI-MMbn-qxzuv_fbyAXhUY1v1jK4-wZ8S_our-ul4bLqLJLis64Vtul6vCcsEJZ8qvVMsESRA_0i0)

O diagrama de classes do sistema de locação de quadras esportivas representa a estrutura estática do projeto, detalhando as classes implementadas e suas relações. Ele ilustra a herança entre Usuario, Locador e Locatario, a composição entre UsuarioRepositorio e Database, e as interações dos controladores com o modelo, refletindo o padrão MVC. O diagrama destaca atributos e métodos principais, com notas indicando que os atributos localizacaoQuadra, tipoQuadra e horariosDisponiveis em Locatario são temporários e que alguns métodos de UsuarioRepositorio estão planejados, mas não implementados, fornecendo uma visão clara da organização e funcionamento do sistema no estado atual.

### 6.2 Diagramas de caso de uso 

![Diagrama UML](https://www.plantuml.com/plantuml/png/bP51JWCn34NtEOMNi2W7G5LLgOKL6ufWRoPkQp69AoSPeTw60t2ANemPCQhQEY1rDv7_-_wUFqyPDPVGklJ1SOUA0O94QROgWI1h8UUmoQBm90rwqPDNZxACxnTEcG8wDyfWCfd1pIFkQT1kEDww8s9dvzG2FQQigF2Qok6h9mnSbrGzdWjwnSknn5JQt8zNb4WxJ6R56wU2BU-F5WcMd7OI3zyTiTMlQ5IFZfNCiQ7sLE3EVWBS3Ljx4uyA2oLFiM7iDy4zJAVqcIdwsSpLRZz3b-Z5G2RTBqBAQsvGnzFudGSFJnUu6-iT3gbdD8fZ53FxSwTpKJA1ycQRGTQr4W4U0dXA53jfEmuKipYA7WRIyhRbAnrigTVnjlF_-Nd_LKBx0m00)

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

![Diagrama UML](https://www.plantuml.com/plantuml/png/dLMnRXin3Dtr5KIc173ItKCHm6dH0bcQeDtf4nqBrOakgNFxEq67Jls1hlwnIdVMrP5Zkyd6anwV7laetRL6bDYrtkXN5rOes4BBWPkbS4iGfIDZi8aiSCiD9h1Zas3HDMw58SBPz9OVN9XnYCBUavm1AbHhLSODwdBEA7QahDAF06gkpzhb_JjQiRh8AUmPzfVtD4ISerAFBXyLvbE7Lh17366rVqTAiXu0GrmZFh1WaRIDZHcBWiktTQUcy34e2K7O_6b960YKmX9DXSkf-pLE0Rj88Gb0EGzT9fWC-HTc7vqvIkLJ-4BY5YaH6Y5BeN7er9Hjk3nmtXsb8208QUSZMdxsdEVgpAFrPe5UoQ2FCFjtAgmtZzvPL0EmN_RHuPZ234Ne0S4Mb8636OLnN9x2knzkJl2jTrl1EbrnsFnUayjYHjnf6VVagN4SSCir0Pj0GB1asJmcy0bPX_oTTzgW3DEeDxqybzMTNnY0KnOd-jwbKfy1E6dmhTEKOAda73ZcL4FAe1IQrxloGYDIl73I8iXmGL_PzqOSolQEd-zQEicEPlXn0wexPWVdvYxFkQN_CU9cd4L_yAIjm2a4-WwLsXsTPUkfk7lqwx5DjQAHkVHpyslpatUf3iWk-xc15byxFVTTGwhyagcff8AbiJRoIayU71Vg9-V4A9886meMq4TZ0aS2SG_B2Bmugj00lEz2_p0Cpk_80ch1fZ2isQzTIo7oLSBFFAfI-GDDnePI-Q50oEMvTkKf9w55lUgrPLd6NAUmQ_rV)

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

## 11. Proximos passos
  
