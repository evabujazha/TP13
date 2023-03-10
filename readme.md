Desafio 13  - Fork, Cluster, Proxy & NGINX
## Nota : el archivo .env sera enviado por separado (no incluido en el repositorio) 

----------------------------------------------------------------------------------------------

# Comandos para ejecucion modo Fork o Cluster

### Scripts
 - npm run fork (Inicia modo fork en puerto 8080)
 - npm run cluster (Inicia modo cluster en puerto 8080)

### Terminal
 - node main.js --port (numero puerto, default : 8080) --mode (modos : cluster o fork, default : fork)
- nodemon main.js --port (numero puerto, default : 8080) --mode (modos : cluster o fork, default : fork)

----------------------------------------------------------------------------------------------

# Comandos ejecucion con Forever

 - forever start ./main.js --port=8081 --watch
 - forever start ./main.js --port=8082 --watch
 - forever start ./main.js --port=8082 --watch
 - forever list
 - forever stopall

----------------------------------------------------------------------------------------------

# Comandos ejecucion pm2 

## Modo fork
 - pm2 start ./main.js --name=server --watch -- --port=8081
 - pm2 list
 - pm2 delete all
## Modo cluster 
 - pm2 start ./main.js --name=servidor --watch -i max -- --port=8081
 - pm2 list
 - pm2 delete all

----------------------------------------------------------------------------------------------






