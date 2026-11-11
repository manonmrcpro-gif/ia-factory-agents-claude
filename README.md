# IA Factory Agents

Plugin Claude (Cowork / Claude Code) qui regroupe les **15 agents de la Bibliothèque d'agents IA Factory** sous forme de skills, plus l'interview qui crée tes documents de référence. Chaque skill reprend le prompt de l'agent (rôle, méthode, règles, format de sortie), avec les exemples et templates dans `references/`.

## Les agents

| Pilier | Agent (skill) | Ce qu'il fait |
|---|---|---|
| Point de départ | Florence, tes Documents de référence (`florence-documents-de-reference`) | Interview en notes vocales (2 sessions) qui crée tes 3 documents de référence : ADN, méthode & économie ; Ma voix ; Mes règles IA. À lancer en premier. |
| Socle commun | Tina, ton Transcript (`tina-transcript`) | Classe un transcript (interne / formation / prospect / client), le rattache à la bonne fiche, synthétise et range les next actions. |
| Socle commun | Constance, ta Maintenance (`constance-maintenance`) | Garde ton système d'agents sans doublon, documenté et à jour, et met ton schéma d'écosystème à jour. |
| Socle commun | Aya, ta Voix du client (`aya-voix-du-client`) | Relit tes appels chaque semaine, fait remonter ce qui revient avec les mots exacts, envoie les idées de posts dans ton calendrier. |
| Pilotage | Nadia, ta Coach Process et IA (`nadia-coach-process-ia`) | Cartographie d'un process étape par étape, avant et après dessinés dans ton Miro, ou diagnostic et priorisation de tes sujets (Now / Next / Later avec ROI). Pour les indépendants comme pour les entreprises. |
| Pilotage | Joséphine, ton Cadrage offre et pricing (`josephine-cadrage-offre`) | Part de ton existant, fixe plancher et objectif, décline ton CA en offres pricées à la valeur, écrit ta promesse. |
| Acquisition Marketing | Coco, ta Stratégie édito (`coco-strategie-edito`) | Calendrier du mois sur 3 piliers (le marché, ta méthode, toi), veille avec score sur la médiane, hooks et squelettes ; tableau de bord en artefact et point hebdo (arrête / double / teste, personnes chaudes). Ne rédige jamais. |
| Acquisition Marketing | Simone, ta Coach rédaction (`simone-coach-redaction`) | Te fait raconter, relit ton post (hook, toboggan, chute, tics d'IA), propose des options, te fait lire à voix haute. N'écrit pas à ta place. |
| Acquisition Marketing | Juliette, ton Lead Magnet (`juliette-lead-magnet`) | Quiz diagnostic, page de capture et 5 emails après l'inscription. |
| Acquisition Marketing | Serena, tes Cas clients (`serena-cas-clients`) | Transforme une mission réussie en cas client Avant → Pont → Après. |
| Acquisition commerciale | Mireille, ta Veille offres de mission (`mireille-veille-missions`) | Repère les offres de mission sur LinkedIn, Malt et Welcome to the Jungle avec des mots-clés testés en direct, les trie et donne une piste d'angle pour candidater. |
| Acquisition commerciale | Berthe, ta Préparation RDV découverte (`berthe-preparation-rdv`) | Fiche stratégique + guide de call avant chaque R1. |
| Acquisition commerciale | Nicole, ton Analyse de call (`nicole-analyse-call`) | Après le RDV : analyse du call, objections, plan d'action commun, mail de suivi, closing. |
| Acquisition commerciale | Nawal, ta Propale (`nawal-propale`) | Proposition commerciale qui fait signer : diagnostic, coût de l'inaction, ROI, un seul next step. |
| Delivery | Colette, ta Cheffe de projet (`colette-cheffe-de-projet`) | Suivi de mission + récap client adapté au canal. |
| Delivery | Hortense, ton Expérience client (`hortense-experience-client`) | Designe l'expérience que tu veux vendre (storyboard en 6 cases, émotions, parcours interne), ta semaine type et le nombre de clients que tu peux suivre, puis vérifie que ton offre tient. |

## Le socle commun

Chaque agent suit le même socle : il annonce en démarrant à quoi il sert, où il lit et où il range, et s'il s'utilise tel quel ou se personnalise ; il vérifie ses sources et ne crée rien en double ; il explique chaque outil qu'il fait entrer ; il va chercher l'info dans le navigateur plutôt que de demander des captures ; il rend le process en fin de séance (gris = l'IA, rose = à la main, goulots signalés) ; il propose lui-même Claude in Chrome pour les outils sans connecteur ; il propose un créneau dans ton agenda après chaque tâche planifiée ; il indique l'adresse d'envoi en tête de ses brouillons si tu écris depuis plusieurs adresses ; il finit par « Où on en est ». Aucun agent ne rédige un message à copier-coller pour une personne réelle : il suggère une piste, tu écris.

## Les chaînes

- **Contenu** : Aya, ta Voix du client → Coco, ta Stratégie édito → Simone, ta Coach rédaction
- **Vente** : Juliette, ton Lead Magnet / Mireille, ta Veille offres de mission → Berthe, ta Préparation RDV découverte → Nicole, ton Analyse de call → Nawal, ta Propale
- **Delivery** : Tina, ton Transcript → Colette, ta Cheffe de projet → Serena, tes Cas clients

## Docs de référence attendus

Ils sont créés par le skill `florence-documents-de-reference` (interview en notes vocales). Les skills cherchent d'abord ces documents (Notion ou Google Drive via le connecteur, ou fichiers joints) et **demandent ce qui manque** avant de produire. Aucun chiffre, verbatim ou cas client n'est inventé.

- **🧬 ADN, méthode & économie** (`ADN-methode-economie.md`) : qui tu es, tes offres et prix, ton équation business, ta vente, ta méthode, ton client idéal. Remplace `services.md`, `methode.md` et le doc Économie.
- **🎙️ Ma voix** (`Ma-voix.md`) : ton ton externe et interne, tes mots, tes exemples. Remplace Ta Voix.
- **⚙️ Mes règles IA** (`Mes-regles-IA.md`) : à coller dans les instructions personnalisées de ton IA, pas à joindre aux agents.
- **VoC** : page de synthèse Voix du Client, enrichie au fil de l'eau
- **Calendrier de contenu** (Notion) · **fiches Projets / Prospects / Clients / Tâches** (Notion)
- **Cas clients** + liens témoignages · `charte-graphique.md` (formats visuels)

## Connecteurs utiles

Pas obligatoires, mais ils rendent les skills autonomes :
- **Notion** : transcripts, fiches, calendrier, page VoC
- **Gmail / Slack** : brouillons de mails de suivi et de récaps (jamais d'envoi automatique)
- **Recherche web** : mini-veille prospect (`berthe-preparation-rdv`), benchmarks sourcés (`nawal-propale`)

## Installation

**Cowork** : importer le fichier `ia-factory-agents.plugin`.

**Claude Code** (repo privé, il faut avoir accès au dépôt) :

```bash
claude plugin marketplace add manonmrcpro-gif/ia-factory-agents-claude
```

```bash
claude plugin install ia-factory-agents@ia-factory
```

## Source

Généré à partir de la base Notion « 🤖 Bibliothèque d'agents ». Quand un agent évolue dans Notion, mettre à jour le `SKILL.md` correspondant et incrémenter la version dans `.claude-plugin/plugin.json`.
