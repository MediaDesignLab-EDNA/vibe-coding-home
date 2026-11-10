# Vibe coding et collaboration · UX UI 2e année

L'École de design Nantes Atlantique · Media Design lab

Ce dépôt est le point de départ du cours. Suivez les étapes **dans l'ordre**, en même temps que la classe. Cochez au fur et à mesure dans votre tête… ou sur papier.

- [Séance 2 · Structurer et spécifier](#séance-2--structurer-et-spécifier)
- [Séance 1 · Votre environnement et votre première page en ligne](#séance-1--votre-environnement-et-votre-première-page-en-ligne)
- [En cas de problème](#en-cas-de-problème)

---

## Séance 2 · Structurer et spécifier

> « Pourquoi l'IA a tout cassé au troisième prompt ? »

### 0 · Tout de suite : relancez votre codespace

- [ ] Allez sur https://github.com/codespaces et cliquez sur celui de `vibe-coding-starter` (pas « New codespace »).
- [ ] Laissez l'onglet ouvert : il met 5 à 15 minutes à démarrer. On s'en sert à l'étape 2.
- [ ] Codespace supprimé ? Depuis **votre** dépôt `vibe-coding-starter` : Code › Codespaces › Create codespace on main.

### 1 · Markdown et commits, dans votre journal de bord (sur github.com)

Un dépôt personnel où vous noterez, après chaque séance, ce que vous avez appris. Exemple complet : https://github.com/MediaDesignLab-EDNA/journal-exemple

**Créer le dépôt**

- [ ] https://github.com/new : Repository name `journal-vibe-coding`, Choose visibility **Public**, **Add README : On**, puis **Create repository** en bas de la page.

**Modifier le README** : sur la page du dépôt, cliquez sur le crayon en haut à droite du README. **Edit** pour écrire, **Preview** pour voir le rendu. Puis **Commit changes…**, remplacez « Update README.md » par votre message, et **Commit changes**. GitHub affiche alors le fichier.

- [ ] Effacez tout, puis écrivez (avec vos mots) :

  ```
  Journal de bord
  Je suis Camille, en 2e année UX UI.
  Ici, je note ce que j'apprends en vibe coding.
  ```

  Commit : « Écrit une première version du journal ». Regardez : les trois lignes sont collées.

- [ ] Remplacez par :

  ```markdown
  # Journal de bord

  Je suis Camille, en 2e année UX UI.

  Ici, je note ce que j'apprends en vibe coding.

  ## Qui je suis

  Étudiante en design, j'aime les interfaces sobres.
  ```

  Commit : « Ajoute des titres ».

- [ ] Ajoutez à la fin :

  ```markdown
  ## Ce que j'apprends

  - **Git** : garder l'historique de mon projet
  - **GitHub** : le partager en ligne
  - *Markdown* : écrire du texte mis en forme
  ```

  Commit : « Ajoute ce que j'apprends ».

- [ ] Ajoutez à la fin, avec votre pseudo :

  ```markdown
  ## Ma page

  [Voir ma page en ligne](https://VOTRE-PSEUDO.github.io/vibe-coding-starter/)
  ```

  Commit : « Ajoute un lien vers ma page ».

| Vous tapez | GitHub affiche |
| --- | --- |
| `# Titre` | un grand titre |
| `## Sous-titre` | un sous-titre |
| une ligne vide | un nouveau paragraphe |
| `- élément` | une puce de liste |
| `**gras**`, `*italique*` | du gras, de l'italique |
| `[texte](adresse)` | un lien |

**Un deuxième fichier, et un lien vers lui**

- [ ] **Add file › Create new file**, nom `seance-1.md` :

  ```markdown
  # Séance 1 · 4 novembre

  **Fait** : mon compte GitHub, ma première page en ligne.

  **Pas compris** : à quoi sert Sync.

  **Ma question** : où vont mes commits ?
  ```

  Commit : « Ajoute mes notes de la séance 1 ».

- [ ] Dans le README, ajoutez :

  ```markdown
  ## Sommaire

  - [Séance 1](seance-1.md)
  ```

  Commit : « Ajoute un sommaire ».

**L'historique**

- [ ] Sur la page du dépôt, cliquez sur l'horloge à droite du dernier commit : c'est l'historique. Ouvrez un commit : en vert les lignes ajoutées, en rouge les lignes retirées.
- [ ] Défi : retrouvez votre README tel qu'il était après votre premier commit (bouton `<>` dans l'historique, ou **Browse files** sur la page d'un commit).

### 2 · Revenir en arrière (sur github.com, dans votre journal)

- [ ] **L'accident** : crayon du README, supprimez les sections « Qui je suis » et « Ce que j'apprends ». Commit : « Oups ».
- [ ] Sur la page du README, cliquez sur l'horloge **History** (à droite du dernier commit).
- [ ] Repérez le commit juste avant « Oups », puis cliquez sur son icône **View code at this point**.
- [ ] Vous voyez le README d'avant l'accident (en haut à gauche, le numéro du commit remplace « main »). Cliquez sur l'icône **Copy raw file**.
- [ ] Revenez à la page du dépôt (« main »), crayon du README, tout sélectionner (Cmd+A sur Mac, Ctrl+A sur PC), coller (Cmd+V ou Ctrl+V).
- [ ] Commit : « Restaure le README d'avant l'accident ».
- [ ] Ouvrez l'historique : « Oups » y est toujours. Rien n'a été effacé, une version a été ajoutée.

### 3 · Donner des règles à l'IA : AGENTS.md et DESIGN.md (dans le codespace)

Une IA ne se souvient de rien d'une conversation à l'autre, et la même demande peut donner des résultats différents. Le fichier `AGENTS.md`, écrit en Markdown à la racine de votre projet, contient des règles que Copilot relit avant chaque réponse.

**L'expérience, en binôme** : l'ordinateur **A** reçoit une charte, l'ordinateur **B** garde le fichier de départ.

- [ ] **Sur A, ensemble** : dans le codespace, explorateur à gauche, ouvrez `AGENTS.md` et ajoutez à la fin, en l'adaptant à l'interface que vous avez apportée :

  ```markdown
  ## Ma charte
  - Couleurs : #002B3B pour le texte, #B7FF6A pour les accents, #FFFFFF pour le fond.
  - Police : « Space Grotesk » de Google Fonts.
  - Ton : tutoiement, phrases courtes.
  - Texte : jamais moins de 16 px.
  - Titres de section en capitales.
  - Pas d'emoji.
  - Notre règle : …
  ```

  L'enregistrement est automatique. Puis **Source Control** › Commit « Ajoute nos règles » › **Sync Changes**.

- [ ] **Sur A** : ouvrez une nouvelle conversation (bouton **+** du chat), demandez « Ajoute une section À propos avec trois phrases sur moi. », puis dépliez **References** sous la réponse : `AGENTS.md` doit apparaître.
- [ ] **Sur A, puis sur B**, une nouvelle conversation pour chaque demande :
  - « Ajoute une section À propos avec trois phrases sur moi. »
  - « Ajoute un formulaire de contact. »
  - « Ajoute un pied de page avec mes réseaux sociaux. »
- [ ] Comparez les deux pages sur vos téléphones : mêmes couleurs ? une seule police ? même ton ? titres de même forme ? des ajouts non demandés ?

**AGENTS.md ou DESIGN.md ?** `AGENTS.md` dit à l'IA **comment travailler** ; Copilot le lit automatiquement. `DESIGN.md` dit **à quoi le projet doit ressembler** (couleurs, polices, composants, ton) ; c'est un format proposé par Google, encore en version alpha ([spécification](https://github.com/google-labs-code/design.md)). Il n'est pas lu automatiquement : `AGENTS.md` doit y renvoyer.

- [ ] **Sur A** : explorateur du codespace, clic droit dans la zone vide › **New File…** › `DESIGN.md` (à la racine, à côté d'`AGENTS.md`). Copiez-y ce modèle, avec les valeurs de votre charte :

  ```markdown
  # Design de ma page

  ## Couleurs
  - Texte : #002B3B
  - Accent (boutons, liens) : #B7FF6A
  - Fond : #FFFFFF

  ## Typographie
  - Police : « Space Grotesk »
  - Taille minimale : 16 px
  - Titres de section en capitales

  ## Composants
  - Boutons : fond accent, coins arrondis de 8 px

  ## Ton
  - Tutoiement, phrases courtes, pas d'emoji
  ```

- [ ] Dans `AGENTS.md`, supprimez la section « Ma charte » et ajoutez à la place :

  ```markdown
  ## Apparence
  - Pour l'apparence, suis le fichier DESIGN.md.
  ```

- [ ] **Source Control** › Commit « Range la charte dans DESIGN.md » › **Sync Changes**.
- [ ] Nouvelle conversation (+), demandez « Ajoute un bouton “Me contacter” sous mon nom. », puis dépliez **References** : `AGENTS.md` et `DESIGN.md` doivent apparaître. Si `DESIGN.md` manque, refaites la demande en ajoutant `#DESIGN.md` à la fin.

### 4 · Une demande qu'on peut vérifier

On ne parle pas ici de tests unitaires (du code qui vérifie du code, le travail des développeurs). On fait une **recette** : une personne vérifie, à la main, que le résultat correspond à la demande. Les conditions à vérifier s'appellent des **critères d'acceptation**. Un bon critère, c'est une action et ce qu'on doit voir : votre binôme peut le vérifier sans vous poser de question.

- [ ] Commit, puis demandez « Fais un joli menu. » Votre binôme : « C'est fini ? C'est réussi ? »
- [ ] **Discard All Changes** (Source Control › survolez « Changes » › flèche arrondie) : retour au commit.
- [ ] Créez `demandes.md` et écrivez la même demande avec trois critères « quand… → je vois… », par exemple :

  ```markdown
  Ajoute un menu en haut de la page, vers mes projets et mon contact.
  C'est réussi si :
  - quand j'ouvre la page sur mon téléphone → je vois le menu sur une ligne, sans défiler de côté ;
  - quand je touche « Projets » → je vois la page descendre jusqu'à mes projets ;
  - quand j'appuie sur Tab, sur ordinateur → je vois chaque lien du menu entouré d'un contour.
  ```

- [ ] Votre binôme relit : peut-il vérifier chaque critère sans vous poser de question ?
- [ ] Donnez la demande et ses critères à Copilot. Commit, Sync.
- [ ] Votre binôme fait la recette sur son téléphone et note ✓ ou ✗ sous chaque critère. Un ✗ devient une nouvelle demande.

### Ce qu'on a construit : le harnais de votre projet

| Fichier | Pour qui | Son rôle |
| --- | --- | --- |
| Le dossier Git (`.git/`) | Vous | Garde chaque version ; permet de revenir en arrière |
| `README.md` | Les humains | Ce que fait le projet, comment le voir |
| `AGENTS.md` | L'IA | Comment travailler ; lu à chaque conversation ; renvoie vers `DESIGN.md` |
| `DESIGN.md` | L'IA et les designers | À quoi le projet doit ressembler |
| `index.html`, `css/`, `js/` | Le navigateur | Le code, écrit par l'IA, vérifié avec vos critères |

### 5 · Avant de partir

- [ ] Dans votre journal de bord : **Add file › Create new file** › `seance-2.md`, et répondez aux quatre questions projetées :

  ```markdown
  # Séance 2 · 10 novembre

  1. Comment je retrouve ce que disait un fichier il y a trois commits :
  2. Comment je répare mon README abîmé, sur github.com :
  3. Ce qui va dans AGENTS.md, et dans DESIGN.md (un exemple chacun) :
  4. Un critère d'acceptation pour « fais un joli menu » :
  ```

  Commit : « Ajoute mes notes de la séance 2 ». Ajoutez aussi `[Séance 2](seance-2.md)` au sommaire du README.
- [ ] **Arrêtez votre codespace** : https://github.com/codespaces › … › Stop codespace.

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
| Copilot dit que la limite est atteinte | Activez Copilot Student si votre offre est validée. Sinon, continuez sur le codespace de votre binôme, ou utilisez un chat gratuit et collez le code dans le bon fichier. |
| Je ne retrouve pas mon codespace | https://github.com/codespaces : la liste de vos codespaces. S'il a été supprimé, recréez-le depuis **votre** dépôt (Code › Codespaces). |
| Le codespace charge encore | Suivez sur l'écran de votre binôme, puis rattrapez. |
| « References » n'affiche pas AGENTS.md | Vérifiez que le fichier s'appelle exactement `AGENTS.md`, à la racine du projet, puis ouvrez une nouvelle conversation (+). |
| « Copy raw file » ne colle rien | Ouvrez l'onglet **Code** de la version d'avant, sélectionnez tout le texte à la main, copiez, puis collez. |
