# Kiti Browser LaçarOS Inside
Essa versão é exclusiva para rodar LaçarOS, então se for usar como navegador, não funcionará.

# Como usar:
Para usar baixe o arquivo zip nos realeases, extraia e rode o executável. Pronto!

# To-Do
Fazer ele rodar localmente para dar para usar apps da comunidade(100% feito)

# Adicionar apps, alterar papel de parede etc
Para adicionar um app, edite o apps.html adicionando: ```<p></p> <a href="nome do arquivo.html"> <img height="50px" width="50px" src="foto do app.png" alt="todo"><p></p>Nome do app</a>``` Crie um arquivo chamado: “nome do app”.html e siga o modelo: ```<!DOCTYPE html><html lang="en"> <head> <meta charset="UTF-8"> <meta name="viewport" content="width=device-width, initial-scale=1.0"> <meta http-equiv="X-UA-Compatible" content="ie=edge"> <title>LaçarOS</title> <style> a{ text-decoration: none; color: white; } .barra{ background: #000; height: 20;  width: 100%; } batata{ cursor:pointer; } body{ font-family:sans-serif; color: white; background: #000; overflow: hidden; } </style> <script src="script.js" defer></script> </head> <body> <div class="barra"> <batata> <a href="apps.html" style="text-decoration:none;background: #fff;border-radius: 5pc;color:#000;">Iniciar</a> </batata> </div> <p></p> <a style="color: red;" href="index.html">Fechar app</a> CONTEÚDO DO SEU APLICATIVO (PODE SER UM IFRAME) </body></html>```


Para colocar um papel de parede baixe um de 1920 x 1080 e salve-o na pasta do seu sistema (KitiOS) como kiti os.png Pronto!


# Compilar
Rode
npm install electron --save-dev
npm install --save-dev @electron-forge/cli
npx electron-forge import
npm run make
e o resto, encontrará em https://www.electronjs.org/pt/docs/latest/tutorial/tutorial-prerequisites
