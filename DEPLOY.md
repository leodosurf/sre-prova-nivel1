Guia de Deploy e Rollback
Como fazer deploy
Construa e teste localmente:
docker build -t sre-app:1.0.1 app/
docker run -p 8080:8080 sre-app:1.0.1
COPIAR CÓDIGO
Execute os testes:
cd tests && pytest -v
COPIAR CÓDIGO
Execute o deploy:
./deploy.sh 1.0.1
COPIAR CÓDIGO
Monitore a aplicação:
./monitor.sh
COPIAR CÓDIGO

