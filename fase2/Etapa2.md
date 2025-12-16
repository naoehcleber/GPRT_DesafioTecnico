# Rodando o srsRAN em modo ZMQ
Para rodar o srsRan como ZMQ, temos que executar o seguinte comando :
`sudo gnb -c <nome do arquivo .yaml> `
[[Configu1rando o ZMQ]]
1. No docker-compose.yml da pasta '/docker" do srsRAN_Project deve-se descomentar a linha "#- "38412:38412/sctp" " para permitir a conexão.
2. Rodar o comando "gnb -c gnb_zmq.yml" dentro da pasta /configs/
3. Rodar o Comando  "sudo ./srsue ue_rf.conf" dentro da pasta "srsRAN_4G/build/srsue/src" para ativar a UE.
4. Algum erro se apresentou nessa etapa impedindo a conexão do GNB com o srsUE (investigação pendente)
