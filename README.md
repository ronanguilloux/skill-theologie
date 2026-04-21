# 🏛️ Skills Théologiques et Exégétiques pour IA

Ce dépôt est un recueil de **"Skills"** destinés aux agents IA et assistants virtuels. Son objectif est de doter l'intelligence artificielle d'outils, de méthodologies et de grilles de lecture rigoureuses pour l'analyse de textes bibliques et théologiques.

Ce projet s'appuie sur le standard ouvert [Agent Skills (agentskills.io)](https://agentskills.io/), un format léger permettant d'étendre les capacités d'un agent avec des connaissances spécialisées et des workflows reproductibles.

## ⚙️ Qu'est-ce qu'un "Agent Skill" ?

Un "Skill" n'est pas un simple prompt. C'est un dossier structuré qui encapsule une expertise procédurale que l'agent peut découvrir et charger à la demande. Ce système repose sur le principe de **divulgation progressive** (*progressive disclosure*) pour ne pas surcharger la mémoire de l'agent.

Un skill est typiquement utilisé au sein d'une discussion avec agent IA (Claude Code, etc.) pour être "invoqué" comme méthodologie ou outil de référence à utiliser par le modèle d'IA qu'il expose (Google Gemini, Claude Sonnet, etc.)

## 💡 Pourquoi ce projet ?

Par défaut, les Modèles de Langage (LLMs) ont tendance à fournir des analyses bibliques lissées, généralistes, ou qui mélangent de multiples traditions interprétatives sans distinction (l'approche "Wikipédia"). 

En chargeant un de ces **Skills**, l'IA est forcée d'adopter une posture herméneutique spécifique et de s'appuyer sur des concepts techniques, définis par de grands auteurs ou courants théologiques. Cela transforme l'exécution de l'agent en lui imposant un cadre méthodologique.

## 📚 Catalogue des Skills

### Disponibles
*   **[`robert-alter-analyse`](./robert-alter-analyse/)** : Analyse de la narration et de la poésie biblique (Ancien Testament) selon les principes littéraires stricts de Robert Alter (*L'Art du récit biblique*). Focalisation sur les scènes-types, les mots-guides (Leitwort), le montage composite et l'ironie dramatique.

### 🚧 À venir (Série en cours de développement)
*Ce recueil a vocation à s'enrichir d'autres cadres d'analyse. Par exemple :*
*   **Exégèse historico-critique** : Approche documentaire, identification des sources (J, E, D, P), critique des formes.
*   **Herméneutique Patristique / Allégorique** : Lecture à travers le prisme des Pères de l'Église (les quatre sens de l'Écriture).
*   **Théologie Systématique** : Analyse de concepts théologiques selon un dogme précis (ex: thomisme, théologie réformée).
*   *... d'autres à définir.*

## 🚀 Comment utiliser ces Skills ?

Pour utiliser ces compétences, vous devez disposer d'un assistant IA en local, compatible avec le standard des skills, comme ``gemini-cli`, Claude Desktop ou `claud-cli`, ou encore OpenCode, Thunderbolt, Cursor, GitHub Copilot, etc. Les deux premiers sont probablement les plus populaires.

Si vous travaillez avec Claude:

1. télécharger ce projet dans Github
2. zipper le dossier contenant le skill de votre choix
3. importer ce fichier (par exemple `robert-alter-analyse.zip`) dans Claude Desktop > Co-Work > Customize (personnaliser) > Competences > '+' (import)
3. Dans Caude, invoquer ce skill: `/robert-alter-analyse` suivi d'un passage (pas trop court) ou du nom du fichier local contenant le texte de Genèse 38

Si vous êtes à l'aise avec la ligne de commande et que vous avez déjà importé ou développé d'autres skills en local, vous pouvez aussi copier le dossier d'un skill de ce répertoire, tel quel à coté de ceux que vous avez déjà (dans `~/.claude/skills` ou `~/.gemini/skill` par exemple)

## 🤝 Contribution
Toute contribution proposant de nouvelles approches herméneutiques ou perfectionnant les skills existants est la bienvenue. L'exigence principale est de respecter le format `SKILL.md`, les droits d'auteur et de copie, et de s'assurer que chaque approche méthodologique soit sourcée, cohérente, et isolée des autres pour garantir des analyses utiles.