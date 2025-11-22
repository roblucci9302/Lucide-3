# Lucide

**Assistant IA Contextuel et Ultra-Personnalisé**

[![License: GPL-3.0](https://img.shields.io/badge/License-GPL%203.0-blue.svg)](LICENSE)
[![Version](https://img.shields.io/badge/version-0.2.4-green.svg)](package.json)

---

## 📖 Qu'est-ce que Lucide ?

**Lucide** est un assistant intelligent nouvelle génération qui vous connaît vraiment. Contrairement aux assistants IA classiques qui oublient tout entre chaque conversation, Lucide construit une mémoire complète de vos interactions, comprend votre contexte professionnel et s'adapte à vos besoins spécifiques.

### Le Problème des Assistants IA Classiques

Avec ChatGPT, Claude ou d'autres assistants IA, vous devez :
- ❌ Réexpliquer votre contexte à chaque nouvelle conversation
- ❌ Décrire qui vous êtes, votre entreprise, votre secteur d'activité
- ❌ Répéter vos objectifs et contraintes à chaque fois
- ❌ Adapter manuellement les réponses génériques à votre situation

### La Solution Lucide

**Lucide est votre assistant personnel qui vous connaît.**

- ✅ **Mémoire Complète** : Se souvient de toutes vos conversations, documents et interactions
- ✅ **Contextuel** : Connaît votre industrie, votre rôle, vos projets en cours
- ✅ **9 Experts Spécialisés** : Se transforme selon vos besoins (RH, CEO, IT, Marketing, etc.)
- ✅ **Offline-First** : Fonctionne sans connexion internet
- ✅ **Sécurisé** : Vos données restent sur votre machine

---

## 🎯 Fonctionnalités Principales

### 1. Système de Profils d'Experts

Lucide intègre **9 profils d'experts spécialisés** qui s'adaptent automatiquement à votre contexte :

| Profil | Spécialisation | Cas d'usage |
|--------|----------------|-------------|
| **👩‍💼 Lucy RH** | Ressources Humaines | Recrutement, offres d'emploi, plans d'onboarding, gestion de conflits |
| **🎯 Lucy CEO** | Stratégie d'entreprise | Plans stratégiques, rapports trimestriels, pitch decks, vision |
| **💻 Lucy IT** | Technologie | Architecture logicielle, debugging, code review, spécifications techniques |
| **📱 Lucy Marketing** | Marketing Digital | Stratégies de campagne, plans de contenu, analyses de marché |
| **💼 Lucy Sales** | Ventes | Scripts de prospection, propositions commerciales, négociation |
| **👥 Lucy Manager** | Management | Gestion d'équipe, feedback, motivation, résolution de problèmes |
| **💰 Lucy Finance** | Finance & Comptabilité | Budgets, prévisions, analyses financières, optimisation fiscale |
| **⚖️ Lucy Legal** | Juridique | Contrats, conformité RGPD, mentions légales, CGV |
| **📚 Lucy Formation** | Formation & Pédagogie | Programmes de formation, évaluations, supports pédagogiques |

### 2. Mémoire Augmentée Multi-Sources

Lucide indexe et mémorise automatiquement :

- **💬 Conversations** : Toutes vos interactions avec l'assistant
- **📄 Documents** : Upload et analyse de PDF, DOCX, TXT, Markdown
- **🖼️ Images** : Screenshots avec OCR automatique
- **🎤 Audio** : Transcription et indexation de vos enregistrements
- **🗄️ Bases de données externes** : Connexion à PostgreSQL, MySQL, APIs REST

**Recherche sémantique intelligente** : Lucide retrouve l'information pertinente même si vous utilisez des termes différents.

### 3. Génération de Documents Professionnels

Créez des documents prêts à l'emploi en quelques secondes :

- **📄 Export PDF** : Documents formatés professionnellement avec mise en page
- **📝 Export DOCX** : Fichiers Word éditables avec styles natifs
- **📋 Export Markdown** : Format texte structuré et portable

**Types de documents supportés** :
- CV et lettres de motivation
- Rapports d'activité
- Présentations et pitch decks
- Contrats et documents juridiques
- Plans stratégiques
- Offres d'emploi
- Propositions commerciales

### 4. Connexion aux Données Existantes

Importez votre contexte de travail existant :

- **PostgreSQL** : Bases de données d'entreprise
- **MySQL** : Systèmes de gestion
- **SQLite** : Bases de données locales
- **APIs REST** : Services tiers

### 5. Interface Moderne et Intuitive

- **Raccourcis clavier** : Accès rapide et navigation efficace
- **Mode Focus** : Interface épurée sans distractions
- **Multi-fenêtres** : Travaillez sur plusieurs conversations simultanément
- **Thèmes personnalisables** : Adaptez l'interface à vos préférences

---

## 🚀 Installation

### Prérequis

- **Node.js** version 20.x.x ([Télécharger](https://nodejs.org/))
- **Python** 3.x ([Télécharger](https://www.python.org/downloads/))
- **Windows** : Build Tools for Visual Studio ([Télécharger](https://visualstudio.microsoft.com/downloads/))

### Installation Rapide

```bash
# 1. Cloner le dépôt
git clone https://github.com/roblucci9302/Lucide-3.git
cd Lucide-3

# 2. Vérifier la version de Node.js
node --version
# Doit afficher v20.x.x

# 3. Installation automatique
npm run setup
```

La commande `npm run setup` va :
- Installer toutes les dépendances Node.js
- Configurer l'environnement
- Construire l'interface web
- Lancer l'application

### Configuration

1. **Copier le fichier d'environnement** :
```bash
cp .env.example .env.local
```

2. **Configurer vos clés API** dans `.env.local` :
```env
# OpenAI (recommandé)
OPENAI_API_KEY=votre_cle_openai

# Ou Gemini
GEMINI_API_KEY=votre_cle_gemini

# Ou Claude
ANTHROPIC_API_KEY=votre_cle_anthropic

# Firebase (optionnel - pour la synchronisation cloud)
FIREBASE_API_KEY=votre_cle_firebase
FIREBASE_AUTH_DOMAIN=votre_domaine.firebaseapp.com
FIREBASE_PROJECT_ID=votre_projet_id
```

3. **Obtenir vos clés API** :
- OpenAI : [platform.openai.com/api-keys](https://platform.openai.com/api-keys)
- Gemini : [aistudio.google.com/apikey](https://aistudio.google.com/apikey)
- Claude/Anthropic : [console.anthropic.com](https://console.anthropic.com)

---

## 🎮 Utilisation

### Démarrer Lucide

```bash
npm start
```

### Raccourcis Clavier

| Raccourci | Action |
|-----------|--------|
| `Ctrl/Cmd + \` | Afficher/Masquer la fenêtre principale |
| `Ctrl/Cmd + Enter` | Envoyer un message |
| `Ctrl/Cmd + Flèches` | Déplacer la fenêtre |
| `Ctrl/Cmd + ,` | Ouvrir les paramètres |

### Workflow Typique

1. **Définir votre contexte** :
   ```
   Je suis CEO d'une startup SaaS de 15 personnes dans le secteur FinTech.
   Nous sommes en phase de levée de fonds Série A.
   ```

2. **Choisir un profil expert** :
   - Basculer vers "Lucy CEO" pour la stratégie
   - Basculer vers "Lucy Finance" pour les budgets
   - Basculer vers "Lucy RH" pour le recrutement

3. **Uploader vos documents** :
   - Glissez-déposez vos PDF, DOCX, images
   - Lucide analyse et indexe automatiquement

4. **Poser vos questions** :
   - Lucide mobilise automatiquement le contexte pertinent
   - Répond avec des informations ultra-personnalisées

5. **Générer des documents** :
   - Demandez un pitch deck, un plan stratégique, une offre d'emploi
   - Exportez en PDF, DOCX ou Markdown

---

## 🏗️ Architecture Technique

Lucide est construit avec les technologies suivantes :

- **Frontend** : Lit Elements (Web Components), JavaScript moderne
- **Backend** : Electron (Node.js)
- **Base de données** : SQLite (local), Firebase (sync cloud optionnel)
- **IA** : OpenAI GPT-4, Google Gemini, Anthropic Claude
- **Document Processing** : pdf-parse, mammoth, tesseract.js (OCR)
- **Document Generation** : pdfkit, docx

### Dépendances Optionnelles

Certaines fonctionnalités nécessitent des modules optionnels :

```bash
# Support complet des bases de données
npm install better-sqlite3 pg mysql2

# Génération d'IDs uniques
npm install uuid
```

Sans ces modules, Lucide fonctionne en mode dégradé avec des mocks légers.

---

## 🧪 Tests

### Tests d'Intégration avec Docker

```bash
# Démarrer les bases de données de test
npm run docker:start

# Lancer tous les tests d'intégration
npm run test:integration

# Tests spécifiques
npm run test:integration:postgres    # PostgreSQL uniquement
npm run test:integration:mysql       # MySQL uniquement
npm run test:integration:sqlite      # SQLite uniquement

# Arrêter les conteneurs
npm run docker:stop
```

**Couverture** : 30 tests d'intégration (PostgreSQL: 10, MySQL: 10, SQLite: 10)

### Autres Commandes de Test

```bash
# Vérifier les dépendances installées
npm run deps:check

# Vérifier la santé des services
npm run deps:status

# Réinitialiser les bases de test
npm run docker:reset
```

---

## 🔒 Sécurité et Confidentialité

### Sécurité des Données

- **✅ Local-First** : Vos données restent sur votre machine par défaut
- **✅ Chiffrement** : Les données sensibles sont chiffrées
- **✅ Isolation utilisateur** : Chaque utilisateur a sa propre base de données
- **✅ RGPD-Compliant** : Règles Firestore strictes pour la synchronisation cloud

### Configuration Recommandée

1. **Régénérez vos clés API** si vous utilisez un fork public
2. **Ne commitez JAMAIS** votre fichier `.env.local`
3. **Activez l'authentification** Firebase pour la sync cloud
4. **Revoyez les permissions** Firestore dans `firestore.rules`

Pour plus de détails, consultez [SECURITY.md](./SECURITY.md).

---

## 📊 Fonctionnalités Avancées

### 1. Système de Workflows

Créez des workflows automatisés pour vos tâches récurrentes :

- Templates de documents pré-configurés
- Pipelines de traitement de données
- Automatisation de tâches répétitives

### 2. Knowledge Graph

Lucide construit un graphe de connaissances de vos informations :

- Relations entre projets, personnes, concepts
- Navigation sémantique
- Découverte de connexions cachées

### 3. RAG Multi-Sources

Système de Retrieval-Augmented Generation avancé :

- Récupération contextuelle intelligente
- Fusion de multiples sources de données
- Classement par pertinence

### 4. API Extensible

Intégrez Lucide avec vos outils existants :

- Endpoints REST pour automatisation
- Webhooks pour événements
- Plugins personnalisés

---

## 🛠️ Développement

### Structure du Projet

```
Lucide-3/
├── src/
│   ├── features/          # Fonctionnalités principales
│   │   ├── ask/           # Interface de conversation
│   │   ├── knowledge/     # Système de mémoire
│   │   ├── listen/        # Transcription audio
│   │   ├── memory/        # Indexation et recherche
│   │   └── settings/      # Configuration
│   ├── bridge/            # IPC Electron (Main ↔ Renderer)
│   └── ui/                # Composants d'interface
├── web/                   # Application React
├── tests/                 # Tests unitaires et d'intégration
├── docker/                # Configuration Docker pour les tests
└── docs/                  # Documentation technique
```

### Commandes de Développement

```bash
# Développement avec rechargement automatique
npm run watch:renderer

# Build de production
npm run build

# Création de l'exécutable
npm run make

# Packaging multi-plateformes
npm run build:win          # Windows
npm run package            # Toutes plateformes
```

### Contribuer

Nous accueillons toutes les contributions ! Consultez [CONTRIBUTING.md](./CONTRIBUTING.md) pour :

- Guidelines de contribution
- Standards de code
- Processus de Pull Request
- Code de conduite

---

## 📚 Documentation

### Guides Techniques

- [ARCHITECTURE_DOCUMENTS.md](./ARCHITECTURE_DOCUMENTS.md) - Architecture du système de documents
- [PHASE_2_MEMOIRE_AUGMENTEE_PLAN_DETAILLE.md](./PHASE_2_MEMOIRE_AUGMENTEE_PLAN_DETAILLE.md) - Système de mémoire
- [PHASE_3_PLAN_AND_ROADMAP.md](./PHASE_3_PLAN_AND_ROADMAP.md) - Roadmap et planification
- [DEPENDENCY_MANAGEMENT.md](./DEPENDENCY_MANAGEMENT.md) - Gestion des dépendances

### Guides d'Utilisation

- [GUIDE_WORKFLOW_DOCUMENTS.md](./GUIDE_WORKFLOW_DOCUMENTS.md) - Workflows de documents
- [GUIDE_DE_TEST_UPLOADS.md](./GUIDE_DE_TEST_UPLOADS.md) - Tests d'upload
- [FORMATAGE_AVANCE.md](./FORMATAGE_AVANCE.md) - Formatage de documents

### Rapports de Validation

- [PHASE1_VALIDATION_REPORT.md](./PHASE1_VALIDATION_REPORT.md) - Validation Phase 1
- [PHASE2_VALIDATION_REPORT.md](./PHASE2_VALIDATION_REPORT.md) - Validation Phase 2
- [PHASE3_VALIDATION_REPORT.md](./PHASE3_VALIDATION_REPORT.md) - Validation Phase 3
- [PHASE4_VALIDATION_REPORT.md](./PHASE4_VALIDATION_REPORT.md) - Validation Phase 4

---

## 🗺️ Roadmap

### Version Actuelle : 0.2.4

- ✅ Système de profils d'experts (9 profils)
- ✅ Mémoire augmentée multi-sources
- ✅ Génération de documents (PDF, DOCX, Markdown)
- ✅ Connexion bases de données externes
- ✅ Interface moderne et responsive

### Version 0.3.0 (Q1 2025)

- 🔄 Mode collaboratif multi-utilisateurs
- 🔄 Plugins et extensions
- 🔄 Support de modèles IA locaux (Ollama)
- 🔄 Mode mobile (iOS, Android)

### Version 1.0.0 (Q2 2025)

- 📋 API publique documentée
- 📋 Marketplace de workflows
- 📋 Intégrations tierces (Slack, Teams, Notion)
- 📋 Analytics et insights d'utilisation

---

## 🤝 Communauté et Support

### Obtenir de l'Aide

- **Issues GitHub** : [github.com/roblucci9302/Lucide-3/issues](https://github.com/roblucci9302/Lucide-3/issues)
- **Discussions** : [github.com/roblucci9302/Lucide-3/discussions](https://github.com/roblucci9302/Lucide-3/discussions)
- **Documentation** : Dossier `/docs` du projet

### Contribuer au Projet

Nous recherchons des contributeurs pour :

- ✨ Nouvelles fonctionnalités
- 🐛 Corrections de bugs
- 📖 Documentation
- 🌍 Traductions (i18n)
- 🧪 Tests

Consultez les [issues avec le label "help wanted"](https://github.com/roblucci9302/Lucide-3/issues?q=is%3Aissue+state%3Aopen+label%3A%22help+wanted%22) pour commencer.

---

## 📄 Licence

Ce projet est sous licence **GNU General Public License v3.0**.

Vous êtes libre de :
- ✅ Utiliser Lucide à des fins personnelles et commerciales
- ✅ Modifier le code source
- ✅ Distribuer des copies modifiées

Conditions :
- 📋 Le code source doit rester open source
- 📋 Les modifications doivent être documentées
- 📋 La même licence doit être utilisée pour les versions dérivées

Voir [LICENSE](./LICENSE) pour plus de détails.

---

## 🙏 Remerciements

Lucide est construit sur les épaules de géants :

- **Inspiration** : Projet [Glass by Pickle](https://github.com/pickle-com/glass) et [CheatingDaddy](https://github.com/sohzm/cheating-daddy)
- **Technologies** : Electron, OpenAI, Google, Anthropic, et l'écosystème open source
- **Contributeurs** : Merci à tous ceux qui ont contribué au projet

---

## 📞 Contact

**Projet** : Lucide - Assistant IA Contextuel
**Version** : 0.2.4
**Licence** : GPL-3.0
**Repository** : [github.com/roblucci9302/Lucide-3](https://github.com/roblucci9302/Lucide-3)

---

**Fait avec ❤️ pour démocratiser l'accès à l'intelligence artificielle contextuelle.**
