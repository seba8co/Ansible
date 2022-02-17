### Ansible

## Description

+- Ansible = infrastructure as code + déployement de configuartions + installations
+- Basé sur Python
+- Orchestateur basé sur du push <> pas d'agent = serveur distant pousse les informations.
+- Connection ssh
+- à différence des outils à base d'agents > pull (puppet etc ...)

Itération sur chancun des serveurs pour les mises à jours pour la méthode push, dépendant de la taille de l'infrastructure.

En pull chaque agent est indépendant.

+- Ansible est plus simple par l'utilisation du ssh en mode verbose.
+- Intégration facile dans les outils de CI/CD.
+- Facilité d'utilisation car Yaml
+- Très nombreaux modules (Ansible Galaxy)
+- Différentes notions et définitions : inventory + playbook + rôles.
    - Inventory : Inventaure de toute les machines
    - Playbook  : Articulation des deux sur quel machine(inventory) on installe quel config (Rôle)
    - Rôles     : Installation spécifique

Installation :

    binaire
    apt
    pip

+- Système de templating = jinja(python)
+- Module pour de nombreux outils communs :
    +- postgres
    +- vmware
    +- aws
    +- libvirt
    +- network
    +- grafana
    +- mysql
