# API-SMS
API em NodeJs para envio de mensagens por SMS bem simples.<br>
Criar a pasta e abri-la no Vs Code em seguida abra o Terminal<br>
Para rodar antes deve instalar as dependências pelos comandos no terminal:<br>
npm install express<br>
npm install nodemon -D<br>
npm install @vonage/server-sdk <br>
***(Após instalado necessita que vá ao site vonage.com e crie o login para ter os dados que serão alimentados dentro do send-sms.js)<br>
Para rodar nossa aplicação de forma dinâmica sempre que salvamos as alterações:<br>
Adicione o script abaixo no arquivo package.json:<br>
  "scripts": {<br>
    "start": "node src/server.js",<br>
    "dev": "nodemon src/server.js"<br>
Chame a aplicação pelo comando: npm run dev<br>
Com Server rodando on....<br>
Hora de testar o envio mas, antes não esqueça de colocar os dados que pegou no site da vonage e o telefone para quem irá enviar a mensagem:<br><br>
const from = "NodeJS SMS";<br>
const to = "55SEU_TELEFONE_AQUI";<br>
const text = "Mensagem enviada por YOUR_NAME_AQUI com NodeJS"<br><br>
outra coisa como este serviço de SMS praticamente é pago neste site da vonage.com você para testar terá um balance(saldo) de $2.00 <br>
sendo suficiente para você conseguir testar sua aplicação onde você poderá depois mudar para conta Premium.<br>


