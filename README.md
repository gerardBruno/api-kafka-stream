# api-kafka-stream
Kafka  a essentiellement 4 API principales;
-Producer API: qui permet à une application de publier un flux vers un ou plusieurs topics
- Consumer API: qui permet à une application de consommer les messages des topics
- Kafka Stream API : Permet de faire des traitements en temps réels(Ce qui est contraire au batch processing lorsque on fait un traitement des données enregistrés)
- Connector API: qui permet de connecter Kafka à une source de données comme MOngoDB

  #Pour avoir un système tolérant aux pannes il faut utiliser un cluster pour démarrer plusieurs instances(Broker) et ces instances vont être coordonnées par zookeeper.
  Si un broker est KO c est Zookeeper qui va le signaler aux autres brokers
  Producer: utilise le principe du PUSH  les messages vers le topic
  Consumer  utilise le principe du PUll  les messages donc reçoit le messages quand il peut pour ne pas être surchargé[Donc kafka stocke les messages dans les topics et c est le consumer qui dit quand il doit consommer les messages] 
