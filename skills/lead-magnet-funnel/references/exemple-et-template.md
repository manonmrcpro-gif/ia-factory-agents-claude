# Lead magnet : exemple, template, note technique

## Exemple (extraits)

> **Lead magnet (quiz)** : « Es-tu en train de perdre de l'argent sur tes devis ? (test en 10 questions) ». Résultat = un profil (« artisan du devis » / « semi-outillé » / « prêt à automatiser ») + le premier pas. Capte l'email ET qualifie.
> **Email 1 (J0)** : Objet « Ton résultat est prêt : tu es [profil] ». Le résultat du quiz, un mot perso, comment s'en servir en 2 lignes.
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

RÉSULTAT PAR PROFIL (un bloc par profil)
- Profil : … · Diagnostic : … · 3 priorités : … · Ressource offerte : … · Prochain pas : …

PAGE DU QUIZ
Accueil : promesse … · bénéfice … · réassurance (gratuit, X minutes) · bouton « … »
Questions (8 à 10, à cocher) : …
Écran résultat : premières lignes … + reste flouté → formulaire Brevo
Confirmation : récap en 2-3 lignes · « ton rapport complet t'attend dans ta boîte mail » · lien de prise de rendez-vous
(Pas de témoignage, de logos ni de bannière : la vente, c'est le post LinkedIn.)

PAGE DE CAPTURE (autre format que le quiz)
Headline : … · Sous-titre : … · 3 étapes : … · Preuve : … · CTA : « … »

5 EMAILS APRÈS L'INSCRIPTION (automatisation Brevo, délai entre crochets)
1. [J0] Le lead magnet · Objet : … · message : …
2. [J+1] Un conseil pour aller plus loin · …
3. [J+2] Un cas client, Avant / Après · …
4. [J+4] Une objection levée + coût de l'inaction · …
5. [J+6] L'offre + lien de prise de rendez-vous · …
```

## Note technique : quel outil d'envoi ?

Les emails partent de **Brevo** (plan gratuit pour commencer, Starter à 7 € par mois s'il bloque), pas de la boîte mail de l'utilisateur : une liste « Lead magnet », un formulaire d'inscription Brevo intégré à la page de capture, et une automatisation « un contact est ajouté à la liste » qui envoie les 5 emails. Si le quiz a des profils, ajouter un attribut de contact « PROFIL » que la page transmet au formulaire : c'est lui qui permet d'envoyer à chacun le résultat et la suite de son profil. Brevo demande de vérifier l'adresse d'envoi. **Un nom de domaine n'est pas obligatoire** : avec une adresse Gmail, Brevo envoie depuis une adresse à lui (prenom@xxx.brevosend.com), ce qui suffit pour monter et tester le tunnel. Brevo déconseille l'adresse gratuite pour la délivrabilité : si l'utilisateur a un nom de domaine, l'authentifier dans Brevo et l'utiliser comme adresse d'envoi. Le formulaire demande au minimum prénom, nom, mail, poste et entreprise, avec la case pour accepter de recevoir les mails : le lead magnet ne filtre pas, il ratisse large, la qualification se fait à la prise de rendez-vous. La page de capture s'héberge sur **Netlify** (plan gratuit). Le plan gratuit de Vercel est réservé à un usage non commercial : si l'utilisateur y est déjà, le lui signaler. Itérer la page dans l'IA et ne la remettre en ligne qu'une fois prête : sur le plan gratuit de Netlify, chaque mise en ligne consomme des crédits (une vingtaine par mois), et au-delà le site est mis en pause jusqu'au mois suivant.
