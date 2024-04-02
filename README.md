# api_rails
crie a api da seguinte forma

  rails new api_rails --api

  # entrei no diretório raiz

  bundle add devise

  bundle install

  ## está linha faz o que? cria toda a esturtura do devise?
  rails generate devise:install
  
  # entrei nesse arquivo 

  config/environments/development.rb

  # e coloquei 
  ## aqui pelo que eu entendi é para abrir email no modo de desenvolvimento para testar certo?
  config.action_mailer.default_url_options = { host: 'localhost', port: 3000 }

  # depois fiz isso
  ## esse cria a estutura do User tipo modelos?
  rails generate devise User
  ## aqui pelo que entendi ele migra as novas colunas para o banco
  rails db:migrate

  # consegui adicionar usuário e realizar login com ele!
  eu estava vendo e acho que com essa estrutura já consigo fazer o que quero que é um CRUD com autenticaçãoe tal mas preciso de ajuda para entender como funciona algumas coisas

# 1 
O usuário XPTO foi criado com sucesso e agora foi da tela de login para a tela inicial. Eu perdi o
código que fizemos juntos, desculpa rs! 
Mas lembro de um tal de token. Esse token eu envio como resposta do `create`? E do `login` talvez!
      
# 2 
Estou achando um pouco confuso algumas coisas!

## 2.1  
O ciclo do Rails é o seguinte:
  - O usuário faz uma requisição (request).
  - O arquivo `routes.rb` contém as rotas para onde essa requisição vai.
  - O controller recebe essa requisição. Qual é a função do controller? Em Dart, ele é um controlador onde deixo funções que são chamadas na view e retorno valores para expor na view.
  - Caso o controller seja o mesmo que é no Dart, o model seria o modelo dos dados? A classe que representa o objeto?
  - O model busca os dados no banco e depois devolve?


