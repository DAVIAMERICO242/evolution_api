git clone https://github.com/DAVIAMERICO242/evolution_api

cd evolution-api

npm install

cp src/dev-env.yml src/env.yml

nano env.yml##configurar token e porta

npm start

####para produção

npm run start:prod

pm2 start 'npm run start:prod' --name ApiEvolution -- start --node-args="--max-old-space-size=4096" --max-memory-restart 4G
