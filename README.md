<h1>Fórum Alura</h1>
<p>Fórum Alura é uma aplicação de fórum de discussão usando Spring Boot. Oferece funcionalidades como criação de tópicos, atualização de cursos e validação de formulários.</p>

<h2>Requisitos</h2>
<ul>
<li>Java 17 ou superior</li>
<li>Maven 3.8.1 ou superior</li>
<li>PostgreSQL 12 ou superior</li>
</ul>

<h2>Configuração do Banco de Dados</h2>
<p>Certifique-se de ter o PostgreSQL instalado e em execução. Crie um banco de dados chamado <code>forum</code>.</p>

<h2>Configuração do Projeto</h2>
<ol>
<li>Clone o repositório:</li>
<pre><code>git clone https://github.com/sucloudflare/desafio-forum-alura.git
cd -desafio-forum-alura
</code></pre>

<p>Atualize o arquivo <code>application.properties</code> com as informações do seu banco de dados:</p>
<pre><code>spring.application.name=forum-alura
spring.datasource.url=jdbc:postgresql://localhost/forum
spring.datasource.username=seu-usuario
spring.datasource.password=sua-senha
spring.datasource.driver-class-name=org.postgresql.Driver
hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect
spring.jpa.hibernate.ddl-auto=update
</code></pre>
</ol>

<h2>Executando a Aplicação</h2>
<p>Para compilar e executar a aplicação, use o Maven:</p>
<pre><code>mvn spring-boot:run</code></pre>
<p>A aplicação estará disponível em <a href="http://localhost:8080">http://localhost:8080</a>.</p>
<h2>Estrutura do Projeto</h2>
<h3>Classes Principais</h3>
<ul>
<li><strong>ForumApplication</strong>: Classe principal que inicia a aplicação.</li>
</ul>

<h3>Validação</h3>
<ul>strong>ErroDeFormularioDto</strong>: DTO para representar erros de formulário.</li>
<li><strong>ErroDeValidacaoHandler</strong>: Handler para capturar e tratar exceções de validação.</li>
</ul>

<h3>DTOs</h3>
<ul>
<li><strong>CursoDto</strong>: DTO para representar cursos.</li>
<li><strong>DetalhesTopicoDto</strong>: DTO para representar detalhes de tópicos.</li>
<li><strong>RespostaDto</strong>: DTO para representar respostas.</li>
<li><strong>TopicoDto</strong>: DTO para representar tópicos.</li>
</ul>

<h2>Autor</h2>
<p>Projeto desenvolvido por Bruno.</p>

<h2>Licença</h2>
<p>Este projeto está licenciado sob os termos da licença MIT. Consulte o arquivo LICENSE para obter mais detalhes.</p>

<footer>
<p>Este README fornece uma visão geral do projeto, requisitos, instruções de configuração e execução, além de detalhes sobre a estrutura e funcionalidades da aplicação.</p>
<p>ChatGPT pode cometer erros. Verifique informações importantes.</p>
</footer>
