# Lead magnet : exemple, template, note technique

## Exemple (extraits)

> **Lead magnet (quiz)** : « Es-tu en train de perdre de l'argent sur tes devis ? (test en 6 questions) ». Résultat = un profil (« artisan du devis » / « semi-outillé » / « prêt à automatiser ») + le premier pas. Capte l'email ET qualifie.
> **Email 1 (J0)** : Objet « Ton résultat : tu es [profil] ». Le résultat du quiz, un mot perso, comment s'en servir en 2 lignes.
> **Email 4** : Objet « Le vrai coût d'un devis fait à la main ». Lève l'objection « j'ai pas le temps de m'y mettre » avec le coût de l'inaction (en heures par an, à partir des chiffres de l'utilisateur).
> **Email 5 (final)** : Objet « On automatise ton chiffrage ? ». Récap Avant/Après + l'offre + le lien de prise de rendez-vous.

## Template

```
LEAD MAGNET
- Problème spécifique visé : …
- Format : [Quiz / Checklist / Guide-ebook / Étude de cas / Template / Mini-atelier]
- Titre : « Comment [GAIN] sans [PAIN] »
- Quick win promis : …
- Ce qu'il NE donne PAS (gardé pour l'offre) : …

PAGE DE CAPTURE
Headline : … · Sous-titre : … · 3 étapes : … · Preuve : … · CTA : « … »

5 EMAILS APRÈS L'INSCRIPTION (automatisation Brevo, délai entre crochets)
1. [J0] Le lead magnet · Objet : … · message : …
2. [J+2] Un conseil pour aller plus loin · …
3. [J+4] Un cas client, Avant / Après · …
4. [J+7] Une objection levée + coût de l'inaction · …
5. [J+10] L'offre + lien de prise de rendez-vous · …
```

## Note technique : quel outil d'envoi ?

Les emails partent de **Brevo** (plan Starter, 7 € par mois), pas de la boîte mail de l'utilisateur : une liste « Lead magnet », un formulaire d'inscription Brevo intégré à la page de capture, et une automatisation « un contact est ajouté à la liste » qui envoie les 5 emails. Brevo demande de vérifier l'adresse d'envoi : une adresse pro (nom de domaine) passe mieux qu'une adresse Gmail. La page de capture s'héberge sur **Netlify** (plan gratuit), sauf si l'utilisateur a déjà Vercel en plan payant : le plan gratuit de Vercel est réservé à un usage non commercial. Itérer la page dans l'IA et ne la remettre en ligne qu'une fois prête : sur le plan gratuit de Netlify, chaque mise en ligne consomme des crédits (une vingtaine par mois), et au-delà le site est mis en pause jusqu'au mois suivant.
