# Começando com RAILS

Site oficial do RAILS: https://rubyonrails.org/

* instalando rvm 
  - https://rvm.io/. Link oficial do rvm
    - instalar chave GPG:
      
      $ gpg2 --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB
      
    - instalar o rvm com curl 
      
      $ \curl -sSL https://get.rvm.io | bash -s stable


* Instalando o Ruby 
  - Após a instalação do rvm:
    
    $ rvm install ruby-< VERSION >
    
    ou 
    
    $ rvm install < VERSION >
  

* Configuração do ambiente 
  - Depois de instalar o ruby, rode:
  
    $ rvm use ruby-< VERSION > 
    
    $ rvm use gemset < NAME-GEMSET > --create
    
  - Instalando o Rails
  
    $ gem install rails 
    
  - Criando o projeto 
    
    $ rails new < NAME-PROJECT >
    
  Vamos usar o nome "projeto", então fica assim:
    
    $ rails new projeto   
    
  Isso criará uma pasta com o esqueleto da sua aplicação Rails, contendo todos os diretórios que serão precisos.
  
  - Depois de criar o projeto, rode dentro da pasta do projeto:
    
    $ bundle 
    
    O bundle fará toda instalação das depêndencias (gems), contidas no GemFile do projeto.

* Criação do Banco de Dados
  - Por padrão, o rails vem com um banco de dados chamado de Sqlite3, um DB simples e bem iniciante. Certifique de ter instalado o DB.
    
    $ rails db:create 
    
  Isso retornará uma mensagem de êxito, informando que o banco foi criado.


* Estamos prontos para subir nosso projeto localmente para produzir.
  - $ rails s 
    
    ou 
    
  -  $ rails server

 ...
