# Lead magnet : exemple, template, note technique

## Exemple (extraits)

> **Lead magnet (quiz)** : « Es-tu en train de perdre de l'argent sur tes devis ? (test en 10 questions) ». 3 profils (« artisan du devis » / « semi-outillé » / « prêt à automatiser »). Capte l'email ET qualifie.
> **Résultat (profil « semi-outillé »)** : *Où tu en es* : tu envoies 6 à 10 devis par mois, sous 3 à 5 jours, et tu en relances rarement (d'après tes réponses). *Les risques* : un devis envoyé après 48 h perd une bonne part de ses chances, et chaque devis non relancé est un chantier laissé au concurrent. *Tes 3 priorités* : 1. réduire le délai d'envoi, 2. relancer chaque devis, 3. suivre ton taux de signature. *Quoi faire maintenant* : un premier pas par priorité + un gabarit de relance. Puis le lien de prise de rendez-vous.
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
- Profil : …
- Où tu en es (à partir de ses réponses) : …
- Les risques (coût de l'inaction) : …
- Tes 3 priorités : …
- Quoi faire maintenant (un premier pas par priorité) + une ressource : …
- Lien de prise de rendez-vous

PAGE DU QUIZ
Accueil : promesse … · bénéfice … · réassurance (gratuit, X minutes) · bouton « … »
Questions (8 à 10, à cocher) : …
Écran résultat : premières lignes … + reste flouté → formulaire Brevo
Nom de domaine : [oui / non]
Après le formulaire, avec nom de domaine : récap en 2-3 lignes · « ton rapport complet t'attend dans ta boîte mail » · lien de prise de rendez-vous
Après le formulaire, sans nom de domaine : redirection vers la page de résultat (résultat complet du profil) · « je te l'envoie aussi, pense à tes spams » · lien de prise de rendez-vous
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

Les emails partent de **Brevo** (plan gratuit pour commencer, Starter à 7 € par mois s'il bloque), pas de la boîte mail de l'utilisateur : une liste « Lead magnet », un formulaire d'inscription Brevo intégré à la page de capture, et une automatisation « un contact est ajouté à la liste » qui envoie les 5 emails. Si le quiz a des profils, ajouter un attribut de contact « PROFIL » que la page transmet au formulaire : c'est lui qui permet d'envoyer à chacun le résultat et la suite de son profil. Brevo demande de vérifier l'adresse d'envoi. **Nom de domaine : deux parcours.** Avec un nom de domaine (recommandé) : l'authentifier dans Brevo, c'est la priorité (des enregistrements DNS à ajouter chez le fournisseur du domaine, l'IA guide pas à pas), et l'utiliser comme adresse d'envoi ; tant qu'à faire, le brancher aussi sur Netlify pour que la page ait une adresse propre (une adresse en .netlify.app n'est pas grave). Un seul nom de domaine pour l'activité, pas un par quiz : on y rattache autant de pages et de quiz qu'on veut (ex. prenomnom.fr/quiz-devis). Éviter OVH, pénible à paramétrer. Sans nom de domaine : avec une adresse Gmail, Brevo envoie depuis une adresse à lui (prenom@xxx.brevosend.com), ça fonctionne, mais une grosse partie des emails part en spam ou n'arrive pas. D'où le parcours sans nom de domaine : la personne arrive sur la page de résultat qui suit le formulaire, et la séquence part quand même, en sachant qu'une partie des emails risque de ne pas arriver. Le formulaire demande au minimum prénom, nom, mail, poste et entreprise, avec la case pour accepter de recevoir les mails : le lead magnet ne filtre pas, il ratisse large, la qualification se fait à la prise de rendez-vous. La page de capture s'héberge sur **Netlify** (plan gratuit). Le plan gratuit de Vercel est réservé à un usage non commercial : si l'utilisateur y est déjà, le lui signaler. Itérer la page dans l'IA et ne la remettre en ligne qu'une fois prête : sur le plan gratuit de Netlify, chaque mise en ligne consomme des crédits (une vingtaine par mois), et au-delà le site est mis en pause jusqu'au mois suivant.
