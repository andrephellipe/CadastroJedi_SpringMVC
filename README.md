<h1>Spring MVC - Digital Innovation One</h1>

<p> Projeto de Introdução a Criação de Aplicações Web com Spring Web MVC

O projeto foi proposto com o objetivo de apresentar a aplicação da linguagem Java na web. O projeto foi desenvolvido usando Spring Boot, Spring Web MVC, HTML puro e o Template Engine Thymeleaf com o objetivo de renderizar e apresentar informações dinâmicas no HTML. 

</p>

Professor. André Luis Gomes

- Tecnologias Utilizadas:
  - HTML 5;
  - Java 11;
  - Thymeleaf;
  - Maven;
  - Spring Boot 2.5.4;

## Instalação do Back-end

Clone o repositório `git clone https://github.com/andrephellipe/CadastroJedi_SpringMVC.`


## Ambiente Local

Execute `Run Java` na sua IDE para que o projeto suba localmente com o SPRING BOOT. <br>

## Ambiente Integrado Local

Após ter configurado o Front, navegue para `http://localhost:8080/` 

<h2> Página inicial </h2>


![jedi1](https://user-images.githubusercontent.com/78508014/133913130-c8811812-1950-486b-8374-ee02ece8ef9f.jpg)

<h2> Página de Cadastro </h2>


![jedi2](https://user-images.githubusercontent.com/78508014/133913063-6814d1c3-6024-4983-adc9-81af2e842806.jpg)

<h3> Spring</h3>

Spring é um Framework antigo em Java de inversão de controle (Inversion of Control IoC).

- IoC é um padrão, sendo uma forma diferente que temos para manipular o controle sobre um objeto. 

- Padrão de Projeto de Injeção de Controle (dependency injection DI). @Autowired
  - Delega para o Spring de dependências e do ciclo de vida dos objetos da aplicação.
  - Evita o alto nível de acoplamento de código dentro de uma aplicação. 
    - Facilita manutenção/implementação de novas funcionalidades; 
    - Habilita a utilização de mocks para realizar unit testes.
- Spring Beans: @Beans é um objeto gerenciado pelo Container IoC (Instâncias de objetos que o Spring está gerenciando).



- <h4>Spring Boot</h4>

  - É ferramenta para construção rápida de projetos usando Spring;

  - Convenção sobre configuração;

  - Auto configuração por padrão;

    

  - O Spring ajuda o controller a devolver as informações através de uma anotação chamada "Expression Language".

    - O Spring Expression Language (SpEL para abreviar) é uma linguagem de expressão poderosa que suporta a consulta e manipulação de um gráfico de objeto em tempo de execução.
    
      
    
    - *Classes do Spring*:
      - ModelAndView - Ajuda a "settar" as informações e renderizar.
      
      - @ModelAttribute - indica que o argumento deve ser recuperado do modelo.
      
        
      
    - Validações:
    
      - @Valid - no controler devesse usar a anotação @Valid para validar a requisição;
    
      - @NotBlank - na entidade (model) devesse usar a anotação @NotBlank nos atributos que não podem estar em branco.
    
        
    
    - Interfaces:
    
      - BindingResult - resultados de erro da validação.
      - RedirectAttributes - utilizado  com a mensagem que será exibida após o redirecionamento.
    

  <h4>MVC</h4>

  - É um padrão de arquitetura não muito novo, conceito / mindset de como as coisas funcionam na internet.

    - Model: trata o negócio e os dados do negócio (back-end);

    - Controller: Comunicação entre front-end e back-end (requisições);

    - View: Normalmente são as telas em que o usuário está interagindo (front-end);

      

      - ***Controller***

        - @Controller: Spring irá controlar as instâncias das classes controller, sendo responsável por todo ciclo de vida do Bean.

        - O controller obedecem os seguem os métodos do protocolo HTTP. 

        - @GetMapping: (protocolos e métodos) sempre que o usuário fizer uma requisição o Spring MVC irá renderizar o HTML que está localizando em templates.

        - @PostMapping: auxilia na criação de um novo dado;
        
        - @PutMapping / @DeleteMapping / etc.
        
          

- <h4>THYMELEAF</h4>

  - Renderiza e coloca a informações dinâmicas no HTML (Template Engine).
  - Vai ajudar a escrever os templates de forma dinâmica, possibilitando que a informação adicionada seja renderizada na tela.
    - redirect page: (return "redirect : ......") - é um redirecionamento através da tag, que atualiza a URL na janela do navegador.
    - na página HTML, tudo o que for Thymeleaf precisa ser colocado th na frente para o Template Engine saber renderizar esse template de forma correta.



- <h4>HTML5</h4>

  - As páginas seguem os métodos (ex. "method = "post"")
  - Expression Language:
    - para redirecionamento de link usasse @ (ex. "href = @{/nome do arquivo HTML5}").
    - para adicionar informações usasse $ (ex. " th:text="${nome da entidade.atributo}"").
