# Sistema de Locação de Quadras Esportivas

## 1. Introdução
Este projeto consiste em um sistema de gerenciamento de aluguel de quadras esportivas, desenvolvido com os princípios da Programação Orientada a Objetos (POO) e o framework ORMLite
para persistência de dados em SQLite. O sistema permite que locadores cadastrem quadras e consultem reservas, enquanto locatários podem buscar disponibilidade e realizar agendamentos.

## 2. Requisitos

### 2.1 Requisitos Funcionais
- Cadastro de usuários (Locador e Locatário).
- Cadastro de quadras esportivas.
- Consulta de disponibilidade de quadras.
- Realização e cancelamento de reservas.

### 2.2 Requisitos Não Funcionais
- Desenvolvimento modular utilizando POO.
- Persistência de dados com SQLite e ORMLite.
- Código organizado, reutilizável e bem documentado.

## 3. Tecnologias Utilizadas
- **Linguagem**: Java
- **Framework de Persistência**: ORMLite
- **Banco de Dados**: SQLite
- **Ferramentas**: Maven (ou outra ferramenta de build, se aplicável), PlantUML (para diagramas UML)
- **Versões**: Java (confirmar versão específica), ORMLite (confirmar versão)

## 4. Conceitos de POO aplicados
-	Encapsulamento: Todos os atributos das classes são privados, acessados por getters e setters.
-	Herança: As classes Locador e Locatario herdam atributos e métodos da classe base Usuario.
-	Polimorfismo: O repositório de usuários (UsuarioRepositorio) é capaz de lidar com diferentes subclasses usando a mesma interface de manipulação.
-	Abstração: A superclasse Usuario encapsula a estrutura comum dos usuários do sistema.

## 5. Diagramas UML

### 5.1 Diagrama de Classes
![Diagrama UML](https://www.plantuml.com/plantuml/png/ZLMnSjim3Dtv5JmlLPjeoAfBSyavkNRmaCPfTrY2RVOeKY4X3qapzmlw1Htw8VwnYX9CIP6JInQ500Yyzm2Obvx0KLrgGOeqoci56mSbo0BbN8Ftw6KgbyeJTiOlwD3a2aeqP8DXONFO_zl_RG_VQYWSU24qhaas0KvjjYGBvJ0dPOqG7-JdOtzolhXQBc-MnxqY3r3aTr-3KrO-2IbFL959PKX8cHfROYQNv9JPX3DXKzwQaGrBK7fey6YsC3Ia8UiQ7j7DeG1FpYOVCxcpgWWEg0aDgHnSCafrAaU9cXihQpM22PSsI3SXE2IAXKuyqZqZJ5v2FLHy5imvo5jOrt9EqHJeCBT3sBcfVaveRBXBZXioPB9JlWQj7i5TRPg4NIVRY8NoT7w77jqEBa9etWbnI9CSHKUn9sbUhKTGnkKuyxHK59uDoKDRBkDnEfLRwqAHJ7xj_caIS6Y7qkIe8TvstJV6z3s9mED4FxrBikZZ2HmvMQJeJEhkcqas36ArylIs41mIGN14Txxe2NI6oIgGgaRJKOLnkRKk29V9mjOhZS7k2QZsmqZT3LfscBXEc0ZeMldA6hLIMXLGO580DGclWV00aNlJaW3YdY_REecnExiSbHofIxS3c84p0uriEVU4ReyYdBOjoNjLOkiR8uv3q4ycEhLM-PJRU8bNsZxKs8_Ng9qhTEmnlOj9DR202RKG0x2U4gSxIebzFRCTQElkBO5-gudCAtUgHwiF6vhrotegtx5WKO7fWhtmMhDMhWGtiBC2tFtuwyVc7v7DiLxVmePVbx4qh4Aym5h5y5wj4iaMTgABmsucuuqfuBajAsTtO0W7g9zVVxRkRXPN-z_xFw--NEBmQ9t_IjEuMoDZx8iGx9UpivbiFBDFiyEYPxAotjTAnEX1K1ocJ399mPRM6uBE1faShj5Xwb4UYulBbabZ1H-EvgdG4Peyf8cQ3WCvTwneA8HUeYdgKly7)
O diagrama de classes representa a estrutura estática do sistema, destacando atributos e relações entre entidades:
-	Usuario: classe base comum a todos os usuários.
-	Locador e Locatario: especializações de Usuario.
-	Quadra: representa os campos esportivos cadastrados por locadores.
-	Reserva: conecta locatários a quadras em horários específicos.

### 5.2 Diagramas de caso de uso 

![Diagrama UML](https://www.plantuml.com/plantuml/png/RP0zJWCn48LxdsAqVOhyX185HNGqW7A0mPui8tazn3DEWpWCP-5YE8iHoqBvdhxtnduxDSnMXkWY7GrC87F_R10uapUMv1nwamntuZ58dYZxUCyiq9n7LgC1dRlaCFMHeBk9fIyK8H2S2eQCsi6h0oXA7hK2jsSspE0b7IERN43yodI02eVzLQKFt_GU0whb6hWVsngpROqpHgfPnYSsRZdb7aWfdojscbQjVbL9qXAjCe7rHH8_SUI0WHgy_lVk_Eh6lRcs3ImMr-EVVjPhrlQljNHjyQPNCxsUwOtRKGfbY9y0)
Representa as principais ações realizadas pelos usuários do sistema:
-	O Locador pode cadastrar quadras e consultar reservas feitas nelas;
-	O Locatário pode visualizar quadras, realizar reservas e cancelá-las;
-	O Sistema realiza validações e controla a disponibilidade.

### 5.3 Diagrama De Sequencia

![Diagrama UML](https://www.plantuml.com/plantuml/png/VP8nJiGm44NxdC9ba98BRB7Q0Y4A6k04i_RixaY99ypO4U8sY8AAK-HYX2GEMGdJZjxx_b_9GGD8Y6rJW0qive4jE9QY6wzagGCVp3Dfm1QsjuaBmxiG5yNYc7gVKBCp3P_9br7Z15L6qL_WfaX0FSB9sndB_aJIml0vVB1nEDkPPEM6B0MGnmXEG6z9E_RK8scvUM2_wJXQnwWsesou-de3QO2VEY-pPjolbrc2htGa-Kl8hS46BR5FtKfo-H4z2ft8WjopJ3UTyEo0IyAM8iDNhdgMJQMlW-_W3UK95QM7Cfdvte9dqY2mAkIMtCgGcuURQgtmpoAP0zO_na7cGoGmFJs21_Gkjiqt)
Mostra o fluxo da operação de reserva:
-	O usuário faz login;
-	Solicita as quadras disponíveis;
-	Seleciona data e horário;
-	O sistema verifica conflitos;
-	Se estiver disponível, cria a reserva;
-	Confirmação é enviada ao locatário.

## 6. Implementação das Classes

### 5.1 Classe Usuario
@DatabaseTable(tableName = "usuarios")
public class Usuario {
    @DatabaseField(generatedId = true)
    private int id;

    @DatabaseField(canBeNull = false)
    private String numero;

    @DatabaseField(canBeNull = false)
    private String nome;

    @DatabaseField(canBeNull = false)
    private String senha;

    public Usuario() {}

    public Usuario(String numero, String nome, String senha) {
        this.numero = numero;
        this.nome = nome;
        this.senha = senha;
    }

    // Getters e Setters...
}
Classe genérica para representar qualquer usuário. Serve de base para Locador e Locatario.

### 5.2 Classe Locador
@DatabaseTable(tableName = "locadores")
public class Locador extends Usuario {
    @DatabaseField
    private String telefone;

    public Locador() {}

    public Locador(String numero, String nome, String senha, String telefone) {
        super(numero, nome, senha);
        this.telefone = telefone;
    }

    // Getters e Setters...
}
Especialização de Usuario, representa quem cadastra quadras.

### 5.3 Classe Database
public class Database {
    private String databaseName;
    private JdbcConnectionSource connection;

    public Database(String databaseName) {
        this.databaseName = databaseName;
    }

    public JdbcConnectionSource getConnection() throws SQLException {
        if (connection == null) {
            connection = new JdbcConnectionSource("jdbc:sqlite:" + databaseName);
        }
        return connection;
    }

    public void close() {
        if (connection != null) {
            connection.close();
            connection = null;
        }
    }
}
Gerencia a conexão com o banco SQLite usando ORMLite.

### 5.4 Classe UsuarioRepositorio
public class UsuarioRepositorio {
    private static Dao<Usuario, Integer> daoUsuario;
    private static Dao<Locador, Integer> daoLocador;
    private static Dao<Locatario, Integer> daoLocatario;

    public static void setDatabase(Database db) {
        // cria DAOs e tabelas
    }

    public Usuario create(Usuario usuario) {
        // cria usuário no banco
    }

    public void update(Usuario usuario) {
        // atualiza dados
    }

    public void delete(Usuario usuario) {
        // remove do banco
    }

    public Usuario loadFromId(int id) {
        // busca por ID
    }

    public List<Usuario> loadAll() {
        // carrega todos os usuários
    }
}
Repositório responsável por salvar, buscar, atualizar e deletar usuários usando a ORMLite.

### 5.5 Relações entre as Classes
  
-	Database fornece a conexão usada por UsuarioRepositorio;
-	UsuarioRepositorio identifica o tipo do usuário e delega operações ao DAO correto (usuário, locador ou locatário);
-	Locador e Locatario são tratados como Usuario, permitindo polimorfismo no repositório;
-	Futuramente, Locador se relacionará diretamente com Quadra, e Locatario com Reserva.

## 7. Testes e Processo de Desenvolvimento

  O processo de desenvolvimento do sistema seguiu etapas bem definidas, mesmo com escopo parcial:
  
### 6.1 Modelagem
  
A modelagem do sistema foi realizada utilizando diagramas UML, com foco na representação clara das entidades, seus atributos, métodos e relações. 
Os diagramas de classes e de casos de uso foram fundamentais para validar o entendimento das funcionalidades esperadas.
  
### 6.2 Testes Realizados
  
Os testes realizados incluíram:
-	Cadastro e listagem de usuários de diferentes tipos (Locador e Locatário);
-	Verificação da persistência no banco de dados SQLite usando ORMLite;
-	Testes de carregamento por ID para assegurar o funcionamento correto do polimorfismo;
-	Testes de herança, utilizando a superclasse Usuario para manipular objetos Locador e Locatario.
  
### 6.3 Implementação Incremental
  
O desenvolvimento seguiu uma abordagem incremental:
-	Primeiramente foram criadas as entidades principais (Usuario, Locador, Locatario);
-	Em seguida, foi construída a infraestrutura de persistência (Database e UsuarioRepositorio);
-	Por fim, foram realizados testes diretos no código Java para verificar a integridade dos dados e o funcionamento da lógica de CRUD.
  
Mesmo que as funcionalidades de reserva ainda não tenham sido totalmente implementadas, a estrutura construída permite sua extensão com facilidade.
  
Os testes realizados incluíram:
-	Cadastro e listagem de usuários de diferentes tipos;
-	Persistência em banco SQLite via ORMLite;
-	Teste de herança e funcionamento do polimorfismo no repositório.

## 8. Conclusão

## 9. Proximos passos
  
