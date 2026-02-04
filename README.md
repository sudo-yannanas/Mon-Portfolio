# Portfolio de Coudrais Trocherie Yann - BTS SIO SISR

Bienvenue sur mon portfolio professionnel. Ce document regroupe mes expériences, mes projets réalisés en formation et mes missions en entreprise.

---

## 🏢 Expériences en Entreprise (Stages)

### [Année 202X] - [Nom de l'entreprise]
**Sujet :** Modernisation de l'infrastructure et gestion de parc.
* [Consulter le rapport de stage](./docs/rapport-stage-1.md)
* [Fiche d'activité : Déploiement de postes](./docs/fiche-deploiement.md)
* **Preuves :** (Screenshots de l'AD, inventaire GLPI...)

---

## 🛠️ Projets de Spécialité (Missions SISR)

### Administration Système & Sécurisation
* **Installation ADDS (Best Practices) :** Utilisation du script *Hello-My-Directory* pour un annuaire durci.
  * [Voir la documentation technique](./docs/adds-hardened.md)
* **Supervision :** Mise en place d'un serveur Zabbix avec alertes SNMP.
  * [Voir la documentation Zabbix](./docs/zabbix.md)

### Projets Réseaux
* **Segmentation VLAN :** Isolation des flux voix et données sur commutateurs Cisco.
  * [Schéma réseau et configuration](./docs/vlan-cisco.md)

---

## 💻 Projets Personnels & Veille
* **Home Lab :** Montage d'un serveur Proxmox pour tester des solutions Open Source.
* **Veille Technologique :** La cybersécurité sur les systèmes industriels.

---

## 📂 Documents Administratifs
* [Curriculum Vitae](./docs/CV.md)
* [Tableau de synthèse des compétences (E4)](./docs/tableau-competences.xlsx)

<style>
  /* Masque les éléments inutiles de GitHub */
  header, footer, .sidebar { display: none !important; }
<style>
  /* On cache tout ce qui gêne */
  header, footer, .sidebar, . accessory { display: none !important; }

  /* On centre tout le corps de la page */
  body {
    background-color: #121212 !important;
    color: #e0e0e0 !important;
    display: flex !important;
    flex-direction: column !important;
    align-items: center !important; /* Centre horizontalement */
    text-align: center !important;  /* Centre le texte */
    margin: 0 !important;
    padding: 50px 20px !important;
    font-size: 1.3rem !important; /* Texte plus grand */
  }

  /* On s'assure que le contenu ne s'étale pas trop */
  section.main-content, .wrapper, main {
    max-width: 900px !important;
    width: 100% !important;
  }

  /* Pour que les listes restent lisibles (alignées à gauche mais centrées dans la page) */
  ul {
    display: inline-block;
    text-align: left;
  }

  h1 { font-size: 3rem !important; }
  h2 { font-size: 2rem !important; color: #4da6ff !important; }
</style>
