# Réponses aux questions du TP:

1. Dans la liste kubectl get pods -A, associez chaque composant à son rôle : kube-apiserver, etcd, kube-scheduler, coredns. Lequel stocke l'état désiré du cluster ?

    - kube-apiserver : point d’entrée central du cluster, reçoit et valide toutes les requêtes API (kubectl, contrôleurs, etc.).
    - etcd : base de données clé/valeur du cluster, elle stocke l’état actuel et la configuration du cluster.
    - kube-scheduler : décide sur quel nœud un pod doit être planifié/exécuté.
    - coredns : service DNS interne du cluster, permet de résoudre les noms des services.

2. 