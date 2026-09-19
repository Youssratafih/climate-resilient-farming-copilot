# 🌱 AgriCopilot — AI-Driven Climate-Resilient Farming Copilot

<p align="center">
  <img src="https://img.shields.io/badge/Status-En_Développement-orange" alt="Status">
  <img src="https://img.shields.io/badge/Python-3.11+-blue" alt="Python">
  <img src="https://img.shields.io/badge/License-MIT-green" alt="License">
  <img src="https://img.shields.io/badge/Impact-Climat%20%26%20Agriculture-red" alt="Impact">
</p>

<p align="center">
  <strong>Un système multi-agents IA qui agit comme un agronome expert 24/7 pour sauver les récoltes face au changement climatique</strong>
</p>

---

##  LA PROBLÉMATIQUE : Une Agriculture en Sursis

### Le Constat Brutal

> **Le changement climatique a brisé les règles de l'agriculture.**  
> Les modèles prédictifs utilisés depuis des décennies sont **obsolètes**.  
> Les agriculteurs prennent des décisions avec des données d'hier pour un climat de demain.

### Les 4 Crises Majeures

| 🔴 Problème | 📊 Impact Concret |  Tendance |
|------------|-------------------|-------------|
| **Micro-climats imprévisibles**<br>Sécheresses, inondations, gels hors saison | Destruction des récoltes avant réaction | +40% d'événements extrêmes |
| **Pénurie de ressources**<br>Nappes phréatiques en baisse, engrais coûteux | Impossibilité d'over-watering ou mass-spraying | -30% d'eau disponible |
| **Nouveaux ravageurs**<br>Insectes et champignons migrent vers de nouvelles zones | Cultures sans résistance naturelle | 70% des cultures menacées |
| **Fossé de connaissances**<br>Régulations et recherche évoluent trop vite | Les agriculteurs ne peuvent pas suivre | 1 étude/minute publiée |

---

## 🎬 SCÉNARIO RÉEL : La Tomate de Mohamed

### Contexte
**Mohamed**, agriculteur à Souss-Massa (Maroc), cultive 5 hectares de tomates. Saison chaude, mais pluies inhabituelles cette année.

### Le Problème
Un matin, Mohamed voit des **taches brunes** sur les feuilles de ses tomates (Secteur 4). Il s'apprête à appliquer son fongicide habituel.

**Mais il ignore que :**
- 🌧️ Le sol est déjà **saturé en eau** (pluies récentes)
- ⚠️ Le fongicide standard est **INTERDIT** (nappe phréatique vulnérable)
- 🌡️ Une vague de chaleur arrive dans **48h**
-  Les régulations imposent des **limites strictes** sur le ruissellement d'azote

### ❌ Sans AgriCopilot
```
Mohamed applique le fongicide
         ↓
Contamination de la nappe phréatique
         ↓
Amende de 15 000 MAD
         ↓
Perte de 60% de la récolte (stress eau + chaleur + produit inadapté)
         ↓
💸 PERTE TOTALE : ~50 000 MAD
```

### ✅ Avec AgriCopilot

```
 Mohamed prend une photo avec son smartphone
         ↓
👁️ AGENT VISION : "Mildiou détecté — Secteur 4 — Sévérité: Modéré"
         ↓
📊 AGENT DATA : "Alerte: Humidité sol à 87% — Irrigation à suspendre"
         ↓
📚 AGENT RAG : "Fongicide standard INTERDIT (Règlement N°2023-AG-047).
               Alternative: Fongicide organique cuivre + biocontrôle"
         ↓
🧠 AGENT SUPERVISOR génère le plan d'action
```

#### 📋 Plan d'Action Généré

> ** Recommandations — Secteur 4**
> 
> 🔴 **NE PAS irriguer** pendant 48h (sol saturé)  
> ✅ **Appliquer** [Fongicide Organique Conforme X] uniquement zone affectée (2 acres)  
> ️ **Surveiller** température — vague de chaleur dans 48h  
> 📅 **Re-inspection** dans 72h  
> ️ **Conforme** avec [Règlement N°2023-AG-047]

**Résultat :**
- ✅ 85% de la récolte sauvée
- ✅ Amende évitée (15 000 MAD)
- ✅ Conformité réglementaire 100%
- 💰 **Économie : ~45 000 MAD**

---

## 💡 LA SOLUTION : AgriCopilot

### Un Agronome IA 24/7 dans Votre Poche

AgriCopilot est un **système multi-agents intelligent** qui combine :
- 👁️ **Vision par ordinateur** (drones, smartphones, satellites)
- 📊 **Données IoT** (capteurs sol, météo, historique)
- 📚 **RAG** (régulations, recherches climatiques, pesticides)
- 🧠 **Orchestration IA** (plans d'action conformes et actionnables)

### Architecture Multi-Agents

```
┌─────────────────────────────────────────────────────────────┐
│                    AGRICOPILOT SYSTEM                        │
│                                                              │
│  ┌────────────┐  ┌────────────┐  ┌────────────────────   │
│  │ 👁️ VISION  │  │ 📊 DATA    │  │ 📚 RAG             │   │
│  │ Agent      │  │ Agent      │  │ Agent              │   │
│  │            │  │            │  │                    │   │
│  │ • Photos   │  │ • Capteurs │  │ • Régulations      │   │
│  │ • Drones   │  │ • Météo    │  │ • Pesticides       │   │
│  │ • Satellite│  │ • Historique│ │ • Recherche climat │   │
│  └─────┬──────┘  └─────┬──────┘  └─────────┬──────────┘   │
│        │               │                    │               │
│        ───────────────┼────────────────────┘               │
│                        ↓                                    │
│           ┌────────────────────────                        │
│           │ 🧠 SUPERVISOR AGENT    │                        │
│           │ (The Action Planner)   │                        │
│           └───────────┬────────────┘                        │
│                       ↓                                     │
│           ┌────────────────────────┐                        │
│           │ 📱 STREAMLIT UI        │                        │
│           │ (Farmer Dashboard)     │                        │
│           └────────────────────────┘                        │
└─────────────────────────────────────────────────────────────┘
```

### Les 4 Agents

| Agent | Rôle | Input | Output |
|-------|------|-------|--------|
| **👁️ Vision** | Les yeux sur le terrain | Photos drone/smartphone, satellite | Détection maladies, stress hydrique |
| ** Data/IoT** | Les senseurs | Capteurs sol, météo, historique | Niveaux pH, azote, humidité temps réel |
| **📚 RAG** | Le cerveau climat & conformité | Base docs (régulations, recherches) | Traitements conformes et efficaces |
| **🧠 Supervisor** | Le planificateur | Synthèse des 3 agents | Plan d'action précis et actionnable |

---

##  IMPACT MESURABLE

### Par Ferme (Estimation Annuelle)

```
┌─────────────────────────────────────────────────────┐
│  💧 Réduction consommation eau ....... -35%         │
│  🌾 Sauvegarde récoltes menacées ..... +25%         │
│  💰 Réduction coûts pesticides ....... -20%         │
│  ️ Conformité réglementaire .......... 100%        │
│  ⏱️ Temps de décision ................ -80%         │
│                                                      │
│  💵 ROI Estimé : 300-500% sur 1 an                  │
└─────────────────────────────────────────────────────┘
```

### Impact Global

| Échelle | Impact |
|---------|--------|
| **Local** | Sécurité alimentaire des petits agriculteurs |
| **Régional** | Réduction pollution nappes phréatiques |
| **Global** | Adaptation au changement climatique, réduction gaspillage |

---

## 🚀 PHASES DE RÉALISATION

### Roadmap sur 12 Semaines

```
┌─────────────────────────────────────────────────────────┐
│  SEMAINES 1-2 : FONDATION                               │
│  ████░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░ 17%  │
│  • Architecture système multi-agents                     │
│  • Setup repository & environnement                      │
│  • Choix stack technique                                 │
└─────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────┐
│  SEMAINES 3-4 : AGENT VISION                            │
│  ████████░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░ 33%  │
│  • Collecte dataset (PlantVillage, etc.)                │
│  • Fine-tuning modèle (ResNet50/EfficientNet)           │
│  • Détection maladies & stress hydrique                 │
│  • API Vision                                           │
└─────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────┐
│  SEMAINES 5-6 : AGENT DATA & IoT                        │
│  ████████████░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░ 50%  │
│  • Simulation capteurs (sol, humidité, température)     │
│  • Traitement time-series                               │
│  • Détection anomalies                                  │
│  • Intégration API météo                                │
└─────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────┐
│  SEMAINES 7-8 : AGENT RAG                               │
│  ████████████████░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░ 67%  │
│  • Collecte docs (régulations, recherches)              │
│  • Vector database (FAISS/ChromaDB)                     │
│  • Embedding & retrieval                                │
│  • Validation conformité                                │
└─────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────┐
│  SEMAINE 9 : AGENT SUPERVISOR                           │
│  ████████████████████░░░░░░░░░░░░░░░░░░░░░░░░░░░░ 75%  │
│  • Orchestration des 3 agents                           │
│  • Génération plans d'action                            │
│  • Workflow engine (triggers)                           │
│  • Intégration LLM (GPT-4/Claude)                       │
└─────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────┐
│  SEMAINES 10-11 : INTERFACE & DÉPLOIEMENT               │
│  ████████████████████████░░░░░░░░░░░░░░░░░░░░░░░░ 92%  │
│  • Dashboard Streamlit                                  │
│  • Pipeline end-to-end                                  │
│  • Tests d'intégration                                  │
│  • Docker & déploiement (Render/Railway)                │
─────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────┐
│  SEMAINE 12 : PRÉSENTATION & MARKETING                  │
│  ████████████████████████████████████████████████ 100%  │
│  • Démo vidéo (2 min)                                   │
│  • Pitch deck (10 slides)                               │
│  • Article technique (Medium/Dev.to)                    │
└─────────────────────────────────────────────────────────┘
```

### Livrables par Phase

| Phase | Livrables Clés |
|-------|----------------|
| **1-2** | Architecture documentée, repo GitHub, `requirements.txt` |
| **3-4** | Modèle Vision entraîné (accuracy >85%), API fonctionnelle |
| **5-6** | Simulateur IoT, détection anomalies, DB capteurs |
| **7-8** | Base vectorielle RAG, retrieval fonctionnel |
| **9** | Orchestrateur opérationnel, rapports générés |
| **10-11** | App Streamlit déployée, démo end-to-end |
| **12** | Vidéo démo, pitch deck, documentation |

---

## 🛠️ Démarrage Rapide

### Prérequis
```bash
Python 3.11+
Git
```

### Installation (5 minutes)

```bash
# 1. Cloner
git clone https://github.com/votre-username/agricopilot.git
cd agricopilot

# 2. Environnement
python -m venv venv
source venv/bin/activate  # Linux/Mac

# 3. Dépendances
pip install -r requirements.txt

# 4. Config
cp .env.example .env
# Éditer .env avec vos clés API

# 5. Lancer
streamlit run app/streamlit_app.py
```

---

## 📊 Stack Technique

| Composant | Technologie |
|-----------|-------------|
| **Computer Vision** | PyTorch, OpenCV, EfficientNet |
| **NLP/RAG** | LangChain, FAISS, Sentence-Transformers |
| **Data Processing** | Pandas, NumPy, Scikit-learn |
| **Backend** | FastAPI, Python 3.11+ |
| **Frontend** | Streamlit |
| **Database** | SQLite/PostgreSQL, ChromaDB |
| **Déploiement** | Docker, Render/Railway |

---

##  Contribuer

Les contributions sont bienvenues !

1. Fork le projet
2. Créer une branche feature (`git checkout -b feature/AmazingFeature`)
3. Commit (`git commit -m 'Add AmazingFeature'`)
4. Push (`git push origin feature/AmazingFeature`)
5. Ouvrir une Pull Request

---

## 📄 License

MIT License — Voir [LICENSE](LICENSE) pour plus d'informations.

---

## 📬 Contact

**Votre Nom** — [votre.email@example.com](mailto:votre.email@example.com)

**Projet :** [https://github.com/votre-username/agricopilot](https://github.com/votre-username/agricopilot)

---

<p align="center">
  <strong> Cultivons l'avenir, intelligemment.</strong><br/>
  <em>AgriCopilot — Parce que chaque récolte compte.</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Made%20with-%E2%9D%A4-red" alt="Made with love">
  <img src="https://img.shields.io/badge/Powered%20by-AI-blue" alt="Powered by AI">
</p>
```

---
