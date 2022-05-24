# Encurtador URL com banco de dados MongoDB

* Este repositório contém um projeto que visa encurtar URL's, para isso foi utilizado NodeJS e TypeScript em conjunto com o banco de dados NoSQL MongoDB.

Para o bom funcionamento deste projeto em sua máquina será necessário algumas etapas:

* MongoDB
  * Para ter acesso ao MongoDB pode ser feito um cadastro no site "www.mongodb.com/" de forma gratuita.
  * Após fazer o cadastro basta acessar a aba "Database" e criar um database com o plano gratuito disponibilizado pelo site.
  * Com o database criado você pode clicar na opção "connect" -> "connect your application", agora você pode selecionar a opção mais recente do NodeJS e   copiar a URL gerada.
  * Agora que você tem a URL do seu banco de dados, basta abrir a pasta deste repositório e seguir o seguinte caminho "src" -> "config" -> "Constants.ts", dentro do arquivo procure o campo "MONGO_CONNECTION" e substitua a URL pela URL gerada no MongoDB.
  
* Iniciando o servidor
  * Para iniciar o servidor do projeto basta abrir um terminal na pasta de origem do projeto (encurtador_url).
  * Com o terminal aberto digite os seguintes comandos:
    * # npm install
    * # npm run build:watch
    * # npm run dev
  * Feito isso nosso servidor já está aberto em "http://localhost:5000"

* Para introduzir URL's ao nosso encurtador basta utilizar o app Insomnia.
  * Com o app aberto selecione a opção "Post" e coloque o endereço "http://localhost:5000/shorten"
  * Feito isso selecione a opção de introduzir dados no formato JSON. No campo de texto coloque a URL que deseja encurtar no formato:
    * { "originURL": "***`<url-que-deseja-encutar>`***"}
  * Agora você pode clicar em "Send" para enviar a informação para o servidor.
  * O servidor irá retornar diversos campos, o que nos interessa é o campo "shortURL" que contém a URL encurtada, basta copiar essa URL e acessar em seu navegador de preferência.

OBS: Esse projeto foi criado a partir de um curso disponibilizado na plataforma DIO.

By: Giboxz


