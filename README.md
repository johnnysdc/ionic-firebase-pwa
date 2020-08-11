
## Performance Tester and Report creator 
npm install -g lighthouse

## Simple Http Server
npm install -g http-server
http-server #PATH# -p #PORT#


## Build comum ainda sem PWA
ionic serve
ionic build --prod
http-server .\www -p 8000
lighthouse http://localhost:8000/ --view

## Adding PWA features and verifying the report of lighthouse
ng add @angular/pwa
ionic build --prod
http-server .\www -p 8000
lighthouse http://localhost:8000/ --view


## Configuring the firebase SDK

### install Firebase SDK as local binary
npm install -g firebase-tools

### login in your firebase account
#### auto open an link to google oauth
firebase login


### show your account projects
firebase projects:list

### create an basic files of firebase on current directory using the default config to Firebase Hosting, Cloud Firestone and Cloud Functions
firebase init

Execute o seguinte comando pela a raiz do diretório local do seu projeto se quiser realizar alguma das seguintes tarefas:
firebase serve --only hosting

firebase serve --host 0.0.0.0  // accepts requests to any host

### open the content public of www configured on firebase.json
firebase serve

### Send the content of public 'www' to firebase hosting
firebase deploy