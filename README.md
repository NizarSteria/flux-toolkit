## flux-toolkit
https://fluxcd.io/flux/

Pour information, ceci est un composant de notre stack, et tout changement est à la discretion de l'équipe Kube.

# Flux ToolKit
Flux est un outil permettant de synchroniser les clusters Kubernetes avec les sources de configuration (comme les référentiels Git) et d'automatiser les mises à jour de la configuration lorsqu'il y a un nouveau code à déployer. Les composants GitOps toolkit que nous utilisons sont :

SourceController : Son rôle principal  est de fournir une interface commune pour l'acquisition d'artefacts.
KustomizerController : est un opérateur Kubernetes, spécialisé dans l'exécution de pipelines de livraison continue pour l'infrastructure et les charges de travail définies avec des manifestes Kubernetes et assemblées avec Kustomize.
HelmController : est un opérateur Kubernetes, permettant de gérer de manière déclarative les versions de chartes Helm avec des manifestes Kubernetes. 
NotificationController : est un opérateur Kubernetes, spécialisé dans la gestion des événements entrants et sortants. pouvant être utilisé pour de l'alerting.
ci dessous un schéma expliquant leur interactions :
![image](https://github.com/user-attachments/assets/c49f2566-f229-4e79-890a-2fb22a58884d)

Pour plus d'informations consultez la documentation officielle (https://fluxcd.io/flux/)

# Par clusters et par composants
   # Par composants 
   resources:
    - flux-system
    - external-secrets
    - rbac-reconciler
    - dynatrace
    - stakater
    - kube-beats
    - argo-cd
    - argo-rollouts
    - prometheus
    - ingress-nginx )
