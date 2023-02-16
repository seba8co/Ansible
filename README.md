## Ansible

### Description

- Ansible = infrastructure as code + déployement de configuartions + installations
- Basé sur Python
- Orchestrateur basé sur du push <> pas d'agent = serveur distant pousse les informations.
- Connection ssh
- Différent des outils à base d'agents > pull (puppet etc ...)

Itération sur chancun des serveurs pour les mises à jours pour la méthode push, dépendant de la taille de l'infrastructure.

En pull chaque agent est indépendant.

- Ansible est plus simple par l'utilisation du ssh en mode verbose.
- Intégration facile dans les outils de CI/CD.
- Facilité d'utilisation car Yaml
- Très nombreux modules (Ansible Galaxy)
- Différentes notions et définitions : inventory + playbook + rôles.
    - Inventory : Inventaire de toutes les machines
    - Playbook  : Articulation des deux sur quelle machine (inventory) installe-t-on quelle config (rôles)
    - Rôles     : Installation spécifique

Installation :

    binaire
    apt
    pip

- Système de templating = jinja(python)
- Modules pour de nombreux outils communs :
    +- postgres
    +- vmware
    +- aws
    +- libvirt
    +- network
    +- grafana
    +- mysql
