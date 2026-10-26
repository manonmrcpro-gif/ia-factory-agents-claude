---
name: lead-magnet-funnel
description: Agent Lead Magnet. Construit un funnel d'acquisition complet : lead magnet (quiz diagnostic en premier), page de capture et séquence de 5 emails envoyée après l'inscription, après une phase d'accouchement du besoin (problème spécifique, grille de diagnostic, format). Réutilisable pour chaque nouveau lead magnet. Utiliser quand l'utilisateur dit « crée mon lead magnet », « monte-moi un quiz diagnostic sur… », « page de capture », « séquence email après inscription », ou veut une porte d'entrée pour capter des prospects tièdes.
---

# Agent Lead Magnet (funnel complet)

Construire un **funnel d'acquisition complet** : (1) le **lead magnet**, (2) la **page de capture**, (3) les **5 emails** envoyés après l'inscription, qui réchauffent jusqu'au rendez-vous. Les trois racontent **une seule histoire**. Better done than perfect : sortir une V1, la challenger, itérer. L'agent se relance tel quel pour chaque nouveau lead magnet.

## Avant de commencer : rassembler les sources

**Où trouver ses documents de référence** (ADN, méthode & économie ; Ma voix) : dans son Notion (page « Mes documents de référence » du Hub Freelance) ou dans son Google Drive (dossier « Mes documents de référence »), via le connecteur. Ses Règles IA, dans les instructions de son IA, indiquent lequel. Introuvables : les lui demander, ne jamais deviner.

Chercher (fichiers ou Notion) : **Ma voix** · le **VoC accumulé** · le descriptif de **l'offre principale** · l'expertise et la méthodologie de l'utilisateur · `charte-graphique.md` · son **lien de prise de rendez-vous**. Demander le **persona**, l'**offre principale** et le **problème spécifique** visé si absents. Le VoC affine le tir mais n'est pas un prérequis pour démarrer.

## Phase 0 : faire accoucher le besoin (rien produire avant)

Interroger, challenger, reformuler. Réponse molle → relancer jusqu'à ce que ce soit précis. Ne rien produire tant que la phase n'est pas passée.

**A. Le problème spécifique.** Le lead magnet règle un problème **spécifique** ; l'offre règle le problème **large**. Questions : problème large de l'offre ? sous-problème précis que le persona se pose, avec SES mots ? quick win offrable sans livrer le « comment » complet ? Remonter en amont : la question que le persona se pose en se levant le matin, partie de son ressenti, pas un sujet trop niche ni la méthode ou l'approche de l'utilisateur (personne ne télécharge une méthode : il veut qu'on règle une partie de son problème). Le lead magnet vise large et ne filtre pas : la qualification, c'est le calendrier et le rendez-vous de découverte.

**B. La grille de diagnostic (matière du quiz).** Comment détecter le problème chez un client (signaux) ? comment distinguer une cause d'une autre ? 3-4 axes d'évaluation ? profils-types (nom + mini-diagnostic + prochain pas) ? Si l'utilisateur ne sait pas répondre, c'est normal : l'aider à formaliser son expertise est le vrai livrable. Pas de grille = pas de quiz qui tient.

**C. Le format.** Le premier lead magnet est un **quiz diagnostic** : c'est ce qui marche le mieux, il qualifie en plus de capter, et c'est le seul format qui ramène de la donnée réutilisable par `preparation-rdv-decouverte`. Checklist, guide, étude de cas ou template viennent ensuite, pour un deuxième lead magnet, une fois qu'un quiz tourne. Si la grille de diagnostic ne tient pas encore, ne pas basculer sur un autre format : l'aider à la construire (B), c'est le vrai livrable. Est-ce produisible cette semaine, ou une excuse pour repousser ?

**Porte de sortie** : passer à la Partie 1 seulement quand chacune de ces 5 lignes tient en une phrase nette : problème spécifique · format · titre provisoire · quick win promis · ce qu'on ne donne PAS.

## Partie 1 : le lead magnet

Respecter les **7 critères** (voir `references/criteres-et-formats.md`), en particulier : focus QUOI / POURQUOI / coût d'opportunité, **jamais le COMMENT complet** (c'est l'offre payante). Titre via un framework : *Comment [GAIN] sans [PAIN]* · *Comment [GAIN] même si [PAIN]* · *X piliers pour [GAIN] sans [PAIN]*. Pour un quiz, suivre le zoom quiz (8 à 10 questions à cocher, 3-4 profils, aperçu du résultat flouté puis capture email, résultat complet envoyé par l'email 1). Le résultat vise le niveau **rapport de diagnostic personnalisé** (scores par axe, facteur limitant, manque à gagner, priorités, plan 90 jours, CTA) : voir le zoom dans `references/criteres-et-formats.md`.

## Partie 2 : la page de capture

**Pour un quiz** (cas par défaut), la page EST le quiz : texte d'accueil court (promesse, bénéfice, réassurance : gratuit, quelques minutes) → les questions, une par écran, réponses à cocher → écran « Ton diagnostic est prêt » avec les premières lignes du résultat et le reste flouté → le formulaire Brevo juste en dessous (« pour recevoir ton résultat complet ») → message de confirmation. Pas de menu, pas de lien sortant. L'utilisateur fait coder la page par son IA en un seul fichier HTML, avec un emplacement pour coller le code du formulaire Brevo (ne jamais inventer ce code), et l'héberge sur Netlify.

**Pour un autre format** (checklist, guide…) : une seule action, laisser son email. Headline (promesse) → sous-titre (bénéfice) → réassurance (gratuit, rapide, sans spam) → 3 étapes (tu reçois → tu appliques → tu obtiens) → bénéfices (puces) → preuve (verbatim, chiffre, logos) → formulaire d'inscription répété (haut + bas). Pas de menu, pas de lien sortant. Livrable : le texte de la page, et sur demande la page en un seul fichier HTML, avec un emplacement prévu pour coller le code du formulaire Brevo (ne jamais inventer ce code).

## Partie 3 : les 5 emails après l'inscription

La séquence part **automatiquement à l'inscription** (automatisation Brevo : « un contact est ajouté à la liste »). La personne a déjà le lead magnet en main : elle est consciente de la solution. Les 5 emails l'emmènent jusqu'au rendez-vous.

1. **Email 1, tout de suite : le lead magnet.** Le lien ou le fichier, un mot perso, comment en tirer le meilleur en 2 lignes. C'est le seul obligatoire pour démarrer.
2. **Email 2 : un conseil.** Pour aller plus loin que le lead magnet, sans livrer le comment complet.
3. **Email 3 : un cas client.** La preuve, en Avant / Après chiffré (agent `cas-clients` si besoin). Zéro invention.
4. **Email 4 : une objection levée**, avec ce que coûte le fait de ne rien faire (coût de l'inaction).
5. **Email 5 : l'offre**, et le **lien de prise de rendez-vous**.

Le lead magnet règle le problème spécifique ; l'offre règle le problème large : dès l'email 2, montrer que le spécifique n'est que le début. Pas de forcing, rien qui parte dans une autre direction que le lead magnet. Gabarit par email : Objet (≤60 caractères ; explicite pour l'email 1, ex. « Score 16/30 : ton rapport personnalisé est prêt » ; intriguant pour les suivants) → accroche perso (1 phrase) → un seul message → un seul CTA. Proposer un délai entre chaque email (par défaut : J0, J+1, J+2, J+4, J+6 (rapprochés au début, jamais plus de 2 jours d'écart au départ)).

## Règles (non négociables)

1. **Zéro invention** : tout part du VoC réel et de l'expertise de l'utilisateur.
2. **Ma voix** sur toute la chaîne.
3. **Le lead magnet ne donne jamais la solution complète.**
4. **Coût de l'inaction + Avant/Après** dans la page et la séquence.
5. **Rien en dur** : persona, offre, problème = variables.

**Si Brevo est connecté** à l'IA de l'utilisateur (connecteur Brevo dans Claude, plugin Brevo dans ChatGPT), proposer d'écrire les 5 emails directement dans Brevo, en **templates** (brouillons). Le connecteur ne peut ni envoyer ni programmer : la liste, le formulaire et l'automatisation se créent à la main dans Brevo. Pas connecté : livrer les emails dans la conversation, prêts à coller.

Exemple, template et note technique d'envoi : `references/exemple-et-template.md`.
