# Kiti Browser LaçarOS Inside
Essa versão é exclusiva para rodar LaçarOS, então se for usar como navegador, não funcionará.

# Como Usar
Para usar baixe o arquivo zip nos releases, extraia e abra o executável. Pronto!

# Todo
[x] Fazer ele rodar localmente para dar para usar apps da comunidade
[ ] Integração com NovaCommander (sugerido por [Aency](https://github.com/aencyproject/))

# Customização

## Adicionando Apps
Para adicionar um app, edite o apps.html adicionando: ```<p></p> <a href="nome do arquivo.html"> <img height="50px" width="50px" src="foto do app.png" alt="todo"><p></p>Nome do app</a>``` Crie um arquivo chamado: “nome do app”.html e siga o modelo: ```<!DOCTYPE html><html lang="en"> <head> <meta charset="UTF-8"> <meta name="viewport" content="width=device-width, initial-scale=1.0"> <meta http-equiv="X-UA-Compatible" content="ie=edge"> <title>LaçarOS</title> <style> a{ text-decoration: none; color: white; } .barra{ background: #000; height: 20;  width: 100%; } batata{ cursor:pointer; } body{ font-family:sans-serif; color: white; background: #000; overflow: hidden; } </style> <script src="script.js" defer></script> </head> <body> <div class="barra"> <batata> <a href="apps.html" style="text-decoration:none;background: #fff;border-radius: 5pc;color:#000;">Iniciar</a> </batata> </div> <p></p> <a style="color: red;" href="index.html">Fechar app</a> CONTEÚDO DO SEU APLICATIVO (PODE SER UM IFRAME) </body></html>```

## Trocando Papel de Parede
Para colocar um papel de parede, baixe um papel de parede de 1920 x 1080 e salve-o na pasta do seu sistema (KitiOS) como kiti os.png.

# Compilando
```npm install electron --save-dev``` <br>
```npm install --save-dev @electron-forge/cli``` <br>
```npx electron-forge import``` <br>
```npm run make``` <br>
e o resto, encontrará em https://www.electronjs.org/pt/docs/latest/tutorial/tutorial-prerequisites
