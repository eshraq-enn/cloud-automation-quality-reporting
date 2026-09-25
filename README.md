# Architecture Cloud-Native & Automatisation Décisionnelle (NPS / CSAT) 🚀

> Projet de Fin d'Études (PFE) – Ingénierie d'État en Informatique & Réseaux (MIAGE)

## Présentation du Projet
Ce projet formalise la conception et le déploiement d'une architecture Cloud-Native visant à automatiser l'acquisition, le contrôle d'intégrité, la validation et l'intégration analytique des retours de satisfaction client.

L'objectif principal était de supprimer les interventions manuelles, de fiabiliser les données sources et d'assurer une synchronisation continue avec les tableaux de bord décisionnels.

### 🛠️ Stack Technique
* **Automatisation & Orchestration :** Microsoft Power Automate, SharePoint Online, Microsoft Teams
* **Business Intelligence & Analytics :** Microsoft Power BI (DAX, Power Query / M)
* **Modélisation des Données :** Schéma en constellation (Faits et Dimensions)

---

## 🎯 Défis Résolus & Réalisations
* **Zéro latence :** Déclenchement automatique et acquisition sécurisée des flux dès la réception des retours bruts.
* **Intégrité & Gouvernance :** Contrôle des métadonnées, filtrage des fichiers corrompus et gestion des approbations natives dans Microsoft Teams avec traçabilité complète.
* **Résilience opérationnelle :** Gestion des délais de grâce (SLA anti-oubli), relances ciblées et bascule sur des répertoires d'archivage structurés.
* **Décisionnel en temps réel :** Connexion directe et synchronisation automatique du modèle sémantique sous Power BI dès validation du workflow.

---

## 🏗️ Architecture de la Solution
L'architecture repose sur un écosystème interconnecté assurant la traçabilité de bout en bout 


### Composants Clés :
1. **Acquisition & Déclenchement (Zéro Latence) :** Détection événementielle automatique dès la réception des flux dans le Cloud.
2. **Filtre Qualité & Intégrité :** Contrôle des métadonnées, rejet des fichiers corrompus ou vides, et routage vers un répertoire d'archivage sécurisé (`03_REJECTED_DATA`).
3. **Gouvernance & Validation :** Orchestration d'un circuit d'approbation natif via Microsoft Teams avec audit trail complet (horodatage, approbateur).
4. **Résilience Opérationnelle :** Branche parallèle de gestion des délais de grâce (SLA anti-oubli) et relances automatiques ciblées.
5. **Couche Décisionnelle :** Stockage dynamique (`01_RAW_DATA`) et déclenchement automatique de l'actualisation du modèle sémantique sous Microsoft Power BI.

---

## ⚙️ Implémentation du Workflow (Power Automate)
Le moteur d'orchestration gère les branchements conditionnels, les validations hiérarchiques et la synchronisation avec le modèle sémantique Power BI 



---

## 📊 Modélisation & Méthodologie
* **Approche Décisionnelle :** Modélisation en schéma constellation pour optimiser les performances d'agrégation analytique.
* **KPIs Clés :** Net Promoter Score (NPS), Customer Satisfaction Score (CSAT), taux de conformité des fichiers et respect des SLA de traitement.
* **Environnement Technique :** Microsoft Power Automate, Power BI Service, SharePoint Online, Microsoft Teams.

---

*Note de confidentialité : Les données d'entreprise, les identifiants techniques et les informations nominatives ont été anonymisés ou retirés conformément aux règles de confidentialité.*
