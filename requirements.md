# 📘 Spécifications des Exigences - Site Web Asso 404

Ce document formalise les exigences du projet selon la méthodologie **PEGS** (Project, Environment, Goals, System). Il sert de référence pour le développement et la validation du site web de l'Association 404 (MIASHS - UT2J).

---

## 1. P - Project (Contexte & Acteurs)

### Contexte
L'association 404 regroupe les étudiants de Mathématiques et d'Informatique (MIASHS) de l'Université Toulouse - Jean Jaurès. Actuellement, l'association ne dispose pas d'un site web officiel, ce qui limite sa visibilité et la centralisation des informations.

### Parties Prenantes (Stakeholders)
* **Client / Product Owner :** Le Bureau de l'association (Mathis Dugue).
* **Utilisateurs Finaux :**
    * *Étudiants (L1-M2) :* Pour s'informer sur la vie étudiante et les événements.
    * *Entreprises & Recruteurs :* Pour consulter les projets étudiants.
    * *Futurs étudiants :* Pour découvrir la filière et l'ambiance.
* **Administrateurs :** Membres du bureau (besoin de gestion sans compétences techniques).

---

## 2. E - Environment (Environnement Opérationnel)

### Contraintes Techniques
* **Front-end :** React / TypeScript.
* **Back-end / Base de données :** Firebase (Google).
* **Hébergement & Déploiement :** Vercel.
* **Responsive Design :** Le site doit être parfaitement consultable sur mobile, tablette et ordinateur.

### Contraintes de Maintenance
* Le code doit être documenté et lisible pour faciliter la reprise par les futurs bureaux.
* La gestion courante (ajout d'événements) doit se faire sans modification du code source.

---

## 3. G - Goals (Objectifs Métier)

* **G1 - Visibilité :** Créer un site vitrine centralisant les missions, valeurs et l'équipe de l'association.
* **G2 - Valorisation :** Mettre en avant les projets étudiants auprès des partenaires extérieurs.
* **G3 - Dynamisme :** Communiquer efficacement sur les événements (soirées, ventes, ateliers).
* **G4 - Autonomie :** Fournir une interface d'administration simple pour la gestion du contenu.

---

## 4. S - System (Exigences Fonctionnelles & Non-Fonctionnelles)

Les exigences sont classées selon la méthode **MoSCoW** (Must, Should, Could, Won't).

### 🚀 Functional Requirements (Fonctionnalités)

#### **MUST (Indispensable pour la V1)**
> Ces fonctionnalités doivent être présentes pour que le site soit considéré comme livrable.

- [ ] **REQ-F-01 (Landing Page) :** Affichage d'une page d'accueil présentant l'association, ses missions et ses valeurs.
- [ ] **REQ-F-02 (Agenda) :** Affichage dynamique de la liste des événements (passés et à venir) avec date et description.
- [ ] **REQ-F-03 (Admin Auth) :** Système d'authentification sécurisé pour les administrateurs via Firebase.
- [ ] **REQ-F-04 (Admin CRUD) :** Interface permettant d'ajouter, modifier et supprimer des activités sans coder.
- [ ] **REQ-F-05 (Contact) :** Formulaire de contact simple (Nom, Email, Message).

#### **SHOULD (Important)**
> Ces fonctionnalités sont attendues sauf arbitrage contraire en fin de projet.

- [ ] **REQ-F-06 (Trombinoscope) :** Page "À propos" listant les membres du bureau avec leurs rôles et photos.
- [ ] **REQ-F-07 (Projets Étudiants) :** Section dédiée à la présentation des travaux et projets réalisés par les étudiants (vitrine pour recruteurs).
- [ ] **REQ-F-08 (Présentation Filières) :** Page détaillant les parcours Licence et Master MIASHS.

#### **COULD (Confort / Bonus)**
> Fonctionnalités souhaitables si le temps le permet.

- [ ] **REQ-F-09 (Dark Mode) :** Possibilité pour l'utilisateur de basculer entre un thème clair et sombre.
- [ ] **REQ-F-10 (Détails Événement) :** Page dédiée pour chaque événement avec informations étendues (lien externe, plan, etc.).

#### **WON'T (Hors Périmètre)**
> Fonctionnalités explicitement exclues pour cette version.

- [ ] **REQ-F-11 (Paiement) :** Pas de gestion de panier ou de paiement en ligne pour les goodies/pulls (redirection vers contact).

---

### 🛡️ Non-Functional Requirements (Qualité)

- [ ] **REQ-NF-01 (UX/UI) :** Navigation intuitive et respect de la charte graphique de l'asso (Logo, couleurs).
- [ ] **REQ-NF-02 (Performance) :** Le site doit charger rapidement (optimisation des assets sur Vercel).
- [ ] **REQ-NF-03 (Code Quality) :** Code typé (TypeScript), structuré et commenté.

---

## 5. Suivi & Implémentation

Pour garantir la traçabilité, chaque exigence ci-dessus correspond à une **Issue GitHub** dans ce dépôt.

* Les commits doivent référencer les exigences (ex: `feat: add contact form (REQ-F-05)`).
* L'avancement est visible via le board "Project" associé à ce dépôt.