
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

