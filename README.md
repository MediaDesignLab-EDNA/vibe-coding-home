# Vibe coding et collaboration · UX UI 2e année

L'École de design Nantes Atlantique · Media Design lab

Ce dépôt est le point de départ du cours. Suivez les étapes **dans l'ordre**, en même temps que la classe. Cochez au fur et à mesure dans votre tête… ou sur papier.

---

## Séance 1 · Votre environnement et votre première page en ligne

### Avant de commencer

- [ ] Un ordinateur, chargé.
- [ ] Votre téléphone.
- [ ] L'accès à votre boîte mail de l'école.
- [ ] Une photo ou un PDF de votre **certificat de scolarité 2026-2027** (ou de votre carte étudiante).

### 1 · Où en êtes-vous ? (questionnaire anonyme, 10 min)

- [ ] Groupe A : https://forms.gle/bLpL99tN6BBgQgXe9
- [ ] Groupe B : https://forms.gle/UmNX8PGdJBSnnHWy7

### 2 · Créer votre compte GitHub

- [ ] Allez sur https://github.com/signup
- [ ] Email : **l'adresse de l'école**.
- [ ] Username : un pseudo que vous assumerez sur un CV (par exemple `prenom-nom`). Il apparaîtra dans l'adresse de vos sites.
- [ ] Recopiez le code reçu par mail.

### 3 · Sécuriser le compte (double authentification)

- [ ] Installez une appli d'authentification sur votre téléphone : **Google Authenticator** ou **Microsoft Authenticator** (gratuites, App Store ou Google Play).
- [ ] Sur GitHub : https://github.com/settings/security › **Enable two-factor authentication**.
- [ ] Scannez le QR code avec l'appli, recopiez le code à six chiffres.
- [ ] **Téléchargez les codes de secours** et rangez-les dans un gestionnaire de mots de passe (Bitwarden, 1Password, Mots de passe d'Apple, gestionnaire de Chrome). Téléphone perdu sans codes de secours = compte perdu.

### 4 · Demander l'offre étudiante GitHub Education

- [ ] Allez sur https://github.com/education/students › **Rejoindre GitHub Education**.
- [ ] Statut : étudiant·e. École : L'École de design Nantes Atlantique.
- [ ] Envoyez une photo nette de votre certificat de scolarité.
- [ ] La validation prend de quelques heures à quelques jours. Vous recevrez un mail.

### 5 · Copilot

- [ ] Aujourd'hui : **Copilot Free** fonctionne tout de suite, rien à faire.
- [ ] Quand l'offre étudiante est validée : https://github.com/settings/copilot › activez **Copilot Student**. **Ne payez rien** : si on vous demande une carte bancaire, vous êtes au mauvais endroit.

### 6 · Rejoindre l'organisation du Media Design lab

- [ ] Allez sur https://github.com/MediaDesignLab-EDNA/vibe-coding-inscriptions/issues/new/choose › **Je rejoins le cours**.
- [ ] Choisissez votre groupe, tapez le **code donné en cours**, puis **Submit new issue**.
- [ ] Dans votre boîte mail, ouvrez l'invitation de GitHub et cliquez sur **Join**.

### 7 · Copier le modèle de projet dans votre espace

- [ ] Allez sur https://github.com/MediaDesignLab-EDNA/vibe-coding-starter
- [ ] **Use this template › Create a new repository**.
- [ ] Owner : **votre compte** (pas l'organisation). Nom : `vibe-coding-starter`. Visibilité : **Public**.
- [ ] **Create repository**.

> Si VS Code vous propose plus tard « Publish » ou « Create a fork » : vous avez ouvert le codespace sur le modèle et non sur votre copie. Acceptez, choisissez votre compte et « public repository ».

### 8 · Ouvrir votre codespace

- [ ] Dans **votre** dépôt (`github.com/votre-pseudo/vibe-coding-starter`) : **Code › Codespaces › Create codespace on main**.
- [ ] Repérez les zones de l'éditeur : explorateur (fichiers), éditeur, terminal, panneau Copilot.

### 9 · Faire générer votre page par l'IA

- [ ] Dans le panneau Copilot, demandez par exemple :

  > Crée une page de présentation pour une étudiante en design : son nom, une phrase sur ce qu'elle fait, un bouton qui affiche trois de ses projets. Sépare le HTML, le CSS et le JavaScript dans trois fichiers. Explique-moi ensuite le rôle de chaque fichier, en deux phrases maximum.

- [ ] Remplacez par votre nom et vos projets.
- [ ] Voir le résultat : clic droit sur `index.html` › **Show Preview**. Si rien ne s'affiche : dans le terminal, `python3 -m http.server 8000`, puis onglet **Ports** › icône globe.

### 10 · Enregistrer (commit) et envoyer sur GitHub

- [ ] Onglet **Source Control** (barre de gauche) : écrivez un message clair, par exemple « Ajoute ma page de présentation ».
- [ ] **Commit**, puis **Sync Changes**.
- [ ] Vérifiez sur github.com que votre commit apparaît dans votre dépôt.

### 11 · Mettre votre page en ligne avec GitHub Pages

- [ ] Dans votre dépôt sur github.com : **Settings › Pages**.
- [ ] Source : **Deploy from a branch**. Branch : **main**, **/ (root)**, puis **Save**.
- [ ] Attendez 1 à 2 minutes, rechargez : « Your site is live at… ».
- [ ] Votre page est à l'adresse `https://votre-pseudo.github.io/vibe-coding-starter/`. **Ouvrez-la sur votre téléphone.**
- [ ] À chaque nouveau commit envoyé (Sync), le site se met à jour en une minute environ (onglet **Actions** pour suivre).

> Votre dépôt est public : jamais de mot de passe, de clé d'API, d'adresse ou de numéro de téléphone dans le code, ni dans l'historique.

### 12 · Avant de partir

- [ ] Répondez aux trois questions de fin de séance.
- [ ] **Arrêtez votre codespace** : https://github.com/codespaces › … › Stop codespace (il consomme votre quota gratuit).

### Bon à savoir (facultatif)

- Gemini : un an de Google AI Plus offert aux étudiants, à activer avant le 31 décembre 2026 : https://gemini.google/fr/students/ — une carte bancaire est demandée et l'abonnement devient payant (4,99 €/mois) après 12 mois si vous ne résiliez pas. Mettez un rappel.

---

## En cas de problème

| Problème | Que faire |
| --- | --- |
| Pas de mail de GitHub | Regardez dans les spams. Vérifiez l'adresse dans Settings › Emails. |
| L'offre étudiante est refusée | Photo plus nette, document daté de cette année, nom complet sur votre profil GitHub. Redemandez. |
| Le ticket d'inscription dit « code incorrect » | Vérifiez le code et le groupe, ouvrez un nouveau ticket. |
| Settings › Pages dit « Upgrade or make this repository public » | Votre dépôt est privé : Settings › General › Danger Zone › Change visibility › Public. |
| L'aperçu ne s'affiche pas | Plan B du point 9 (terminal, puis onglet Ports). |
| Le site en ligne ne change pas | Avez-vous fait Commit **et** Sync ? Regardez l'onglet Actions, attendez une minute, rechargez. |
