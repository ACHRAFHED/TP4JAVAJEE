# JEE-Activite-Pratique-4

L'objectif est donc de mettre en place une architecture de microservices sécurisée et évolutive pour le développement d'une plateforme e-commerce complète, avec une séparation claire des responsabilités entre backend (Spring Boot, Vault, Consul) et frontend (Angular).
## Travail à faire ##

Créer une application de e-commerce basée sur les micro services :
1. Consul Discovery;
2. Spring Cloud Config;
3. Spring Cloud Gateway;
4. Customer-service;
5. Inventory Service;
6. Order Service;
7. Consul Config (Billing Service);
8. Vault (Billing Service);
9. Frontend Web avec Angular.

=> Vidéos à utiliser comme ressources : 
- Part 1- https://www.youtube.com/watch?v=LPdfVmllSQo
- Part 2 : https://www.youtube.com/watch?v=L0mdrY36tpk
- Part 3 : https://www.youtube.com/watch?v=L36O1edFPJE
- Part 4 : https://www.youtube.com/watch?v=aQRgO2OxC0w
- Part 5 : https://www.youtube.com/watch?v=iMCjDRUXoeM

  ### Les dépendences utilisées ### 

- **Spring Boot Starter Actuator** : Active les fonctionnalités prêtes pour la production, telles que les vérifications de santé et les points de surveillance, pour une application Spring Boot.
- **Spring Boot Starter Web** : Fournit des composants essentiels pour la construction d'applications web avec Spring MVC.
- **Spring Cloud Starter Consul Config** : Intègre Consul en tant que source de configuration pour les applications Spring Cloud.
- **Spring Cloud Starter Consul Discovery** : Active l'enregistrement et la découverte de services à l'aide de Consul dans un environnement Spring Cloud.
- **Spring Cloud Starter Vault Config** : Intègre HashiCorp Vault en tant que source de configuration pour les applications Spring Cloud.
- **Project Lombok** : Une bibliothèque qui simplifie le code Java en fournissant des annotations pour générer du code répétitif, tel que les getters, setters et constructeurs.
- **Spring Boot Starter Test** : Inclut les dépendances pour tester les applications Spring Boot, y compris JUnit et d'autres outils de test.
- **Spring Cloud Config Server** : Fournit un serveur de configuration centralisé pour les systèmes distribués, permettant la configuration externalisée.
- **Spring Boot Starter Data JPA** : Simplifie la configuration des référentiels Spring Data JPA pour l'accès aux données.
- **Spring Boot Starter Data REST** : Permet la création rapide d'API RESTful en utilisant les référentiels Spring Data.
- **H2 Database (runtime)** : Une base de données en mémoire utilisée pendant le développement et les tests.
- **Spring Cloud Starter Gateway** : Fournit les éléments essentiels pour la construction de passerelles API dans un environnement Spring Cloud.
- **Spring Cloud Starter OpenFeign** : Simplifie l'intégration de clients REST déclaratifs dans une application Spring Cloud.

## Consul : Introduction ##
<img width="929" alt="consul2" src="https://github.com/ACHRAFHED/TP4JAVAJEE/assets/102471232/36026082-d16b-4fac-9423-f017f6962a73">
Consul est un outil et une plateforme conçus pour découvrir et configurer des services dans des environnements de centre de données modernes et dynamiques. Développé par HashiCorp, Consul offre des fonctionnalités telles que la découverte de services, la vérification de l'état de santé et le stockage de clés-valeurs. Il permet aux applications de localiser et de communiquer entre elles de manière efficace, favorisant le développement de systèmes distribués résilients et évolutifs. Consul prend en charge diverses intégrations et est fréquemment utilisé en conjonction avec des technologies telles que Spring Cloud pour améliorer la gestion des microservices.
Le lancement de consul via la commande : `consul agent -server -bootstrap-expect=1 -data-dir=consul-data -ui -bind=<Your ip address>
## Vault : Introduction ##

Vault, également créé par HashiCorp, est un outil complet et extensible pour la gestion de secrets et la protection d'informations sensibles. Il offre un moyen sécurisé de stocker et de gérer l'accès à des données confidentielles telles que des mots de passe, des clés API et d'autres informations sensibles. Vault propose des fonctionnalités avancées telles que la rotation automatique des secrets et l'intégration transparente avec différents systèmes d'authentification. C'est une solution polyvalente largement utilisée dans les environnements modernes où la sécurité des données est une préoccupation majeure.
Le lancement de Vault : 
<img width="857" alt="vault" src="https://github.com/ACHRAFHED/TP4JAVAJEE/assets/102471232/d1fcb6eb-e569-437d-8fc7-04b55171bd38">
<img width="905" alt="vault11" src="https://github.com/ACHRAFHED/TP4JAVAJEE/assets/102471232/b110ee46-44a2-4cf6-809b-676ff2f3af95">
<img width="919" alt="vault12" src="https://github.com/ACHRAFHED/TP4JAVAJEE/assets/102471232/bc3ed000-d812-4427-9ebf-40ff0f7c5ae3">
<img width="910" alt="vault13" src="https://github.com/ACHRAFHED/TP4JAVAJEE/assets/102471232/b1dedffe-830e-446d-bfb4-776eaa261344">





  



























