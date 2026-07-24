# 🖥️ Mise en situation dans un contexte helpdesk — Apache Guacamole

> Accès distant "sans agent" (clientless) aux postes du parc, pour simuler un scénario de prise en main à distance côté support/helpdesk.

## Statut

🚧 **Documentation à compléter** — ce volet fait partie du socle applicatif du homelab ; le déploiement d'Apache Guacamole est engagé mais la procédure détaillée reste à formaliser dans ce dépôt.

## Objectif du scénario

Apache Guacamole permet un accès RDP/VNC/SSH directement depuis un navigateur, sans installer de client sur le poste de l'opérateur. L'idée est de reproduire un cas d'usage helpdesk réaliste : un technicien support prend la main à distance sur un poste utilisateur (`Ordinateur - W11`) du parc RAID-A-PORTER pour du dépannage, sans nécessiter d'agent tiers côté poste.

## Ce qui reste à documenter

- [ ] Déploiement du serveur Guacamole (guacd + interface web) via Docker
- [ ] Connexions RDP configurées vers les postes W11 du parc
- [ ] Authentification unifiée via l'annuaire Active Directory (SSO), en cohérence avec l'intégration LDAP déjà utilisée pour GLPI et OrangeHRM
- [ ] Scénario de mise en situation helpdesk : ticket GLPI → prise en main Guacamole → résolution

## Repos liés

- [`ad-structuration-annuaire`](https://github.com/L-VSIX/ad-structuration-annuaire) — authentification prévue
- [`glpi-support-helpdesk`](https://github.com/L-VSIX/glpi-support-helpdesk) — origine du scénario de ticket

## Auteur

**Lilian Vertueux** — [LinkedIn](https://www.linkedin.com/in/lilian-vertueux/)
