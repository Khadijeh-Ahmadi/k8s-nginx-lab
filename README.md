Exécution d'un serveur web NGINX sur Kubernetes avec Ingress et MetalLB

--- Résumé du projet

Dans ce projet, un serveur web NGINX est implémenté sur un cluster Kubernetes à l'aide de :

Page HTML personnalisée via ConfigMap
Définition du déploiement pour l'exécution du pod
Mise à disposition via un service de type LoadBalancer
Utilisation du contrôleur Ingress pour router le trafic
Utilisation de MetalLB pour attribuer une adresse IP externe
Configuration du DNS local dans le fichier /etc/hosts
Entièrement accessible via un navigateur ou Curl.

--Outils et configuration requise

Kubernetes (Minikube)
MetalLB
Contrôleur Ingress-NGINX
Exécution d'un tunnel Minikube pour l'accès externe
Configuration du fichier /etc/hosts pour le domaine local

----Étapes de mise en œuvre

Créez une ConfigMap contenant du contenu HTML.
Définissez un déploiement et montez la ConfigMap.
Créez un service LoadBalancer.
Installez et configurez un contrôleur d'entrée.
Créez une ressource d'entrée pour le routage.
Exécutez un tunnel Minikube.
Ajoutez une adresse IP à /etc/hosts avec le nom nginx.local.
