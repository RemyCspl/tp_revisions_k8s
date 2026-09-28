# Réponses aux questions du TP:

## Etape 1:
1. Dans la liste kubectl get pods -A, associez chaque composant à son rôle : kube-apiserver, etcd, kube-scheduler, coredns. Lequel stocke l'état désiré du cluster ?

    - kube-apiserver : point d’entrée central du cluster, reçoit et valide toutes les requêtes API (kubectl, contrôleurs, etc.).
    - etcd : base de données clé/valeur du cluster, elle stocke l’état actuel et la configuration du cluster.
    - kube-scheduler : décide sur quel nœud un pod doit être planifié/exécuté.
    - coredns : service DNS interne du cluster, permet de résoudre les noms des services.


## Etape 2:
1. Le pod n'a pas été recréé car on a pas utilisé de deployment pour faire en sorte qu'il y ait à minima x pods qui soient toujours actifs.

2. La colonne 'READY 1/1' signifie que l'on a demandé la création d'un pod et que celui ci est bien actif
La colonne 'RESTARTS 0' signifie qu'aucun redémarrage du pod n'a été constaté jusqu'à maintenant