cd # Passos:
- [x] [[Cmake]]
- [x] [libfftw]
- [x] [libsctp]
- [x] [yaml-cpp]
- [x] [mbedTLS]
- [x] GoogleTest

# Tarefa 1:
![[Pasted image 20251203223312.png]]
# Tarefa 1.2:
![[Pasted image 20251203235201.png]]

# Configurando Open5Gs Dockerizado
- Comando para rodar : 
```
	- cd docker_open5gs
	  source .env
	  sudo ufw disable
	  sudo sysctl -w net.ipv4.ip_forward=1
	  docker compose -f 4g-volte-deploy.yaml up```
```

# Rodando o srsRAN em modo ZMQ
Para rodar o srsRan como ZMQ, temos que executar o seguinte comando :
`sudo gnb -c <nome do arquivo .yaml> `
[[Configu1rando o ZMQ]]
