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

  body { 
    background-color: #121212; 
    color: #e0e0e0; 
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; 
    line-height: 1.8; /* Espace entre les lignes */
    padding: 60px 20px;
    margin: 0;
    display: flex;
    justify-content: center; /* Centre horizontalement le bloc principal */
    font-size: 1.2rem; /* Augmente la taille globale du texte */
  }

  .wrapper { 
    max-width: 900px; /* Largeur maximale pour que ce ne soit pas trop étiré */
    width: 100%;
    text-align: center; /* Centre le texte à l'intérieur du bloc */
  }

  /* Aligne les listes à gauche pour la lisibilité, mais garde le bloc centré */
  ul { 
    display: inline-block; 
    text-align: left; 
    margin-top: 10px;
  }

  h1 { font-size: 2.5rem; color: #ffffff; border-bottom: 2px solid #333; padding-bottom: 20px; }
  h2 { font-size: 1.8rem; color: #4da6ff; margin-top: 50px; }
  h3 { font-size: 1.4rem; color: #bb86fc; }
  
  a { color: #4da6ff; text-decoration: none; font-weight: bold; }
  a:hover { text-decoration: underline; color: #82caff; }
  
  hr { border: 0; border-top: 1px solid #333; margin: 40px 0; }
</style>
