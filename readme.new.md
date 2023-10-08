Microservice Consul Sample adapted for NudgeAPM monitoring
==

Builder le projet
--
`1.` `cd microservice-consul-demo` \
`2.` `mvn clean install -DskipTests`

Créer les applications correspondantes dans NudgeAPM
--
`1.` Créer, sur le server Nudge, les applications correspondantes aux microservices `catalog`, `customer` et `order` \
`2.` Ouvrir chaque fichier `nudge.properties` dans les dossiers suivants : \
- `microservice-consul-demo/microservice-consul-demo-catalog/nudge-agent/nudge.properties` \
- `microservice-consul-demo/microservice-consul-demo-customer/nudge-agent/nudge.properties` \
- `microservice-consul-demo/microservice-consul-demo-order/nudge-agent/nudge.properties` \

`3.` Renseigner les UUID et l'URL correspondants pour chaque service

Déployer les services
--
`1.` `cd docker` \
`2.` `docker-compose up` 