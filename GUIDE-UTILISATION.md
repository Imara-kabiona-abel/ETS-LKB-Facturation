# ETS LKB Company — Application de facturation
## Guide d'utilisation

## Ce que fait cette application

Une application unique (un seul fichier) qui remplace votre ancien classeur Excel avec macros :
- Création de **Devis**, **Bons de commande**, **Bons de livraison** et **Factures**, avec numérotation automatique.
- **Catalogue produits/services** et **fichier clients** réutilisables (plus besoin de retaper à chaque fois).
- **Historique** de tous vos documents, avec suivi du statut de paiement des factures (Payé / Impayé / Partiel).
- Génération de documents imprimables ou exportables en PDF, directement depuis votre navigateur.

**Pourquoi ce changement par rapport au fichier Excel ?** Le fichier `.xlsm` que vous utilisiez fonctionne avec des macros VBA. Les macros VBA ne s'exécutent ni sur Android ni sur iPhone (limitation d'Excel Mobile, pas de cette application). Cette version fonctionne à l'identique sur PC, Android et iPhone, car c'est une page web autonome — pas besoin d'Excel du tout.

## Important à savoir avant de commencer

Cette application ne nécessite **aucune connexion internet** pour fonctionner au quotidien (elle tourne entièrement dans votre navigateur). En revanche, vos données (documents, catalogue, clients) sont enregistrées **uniquement sur l'appareil et le navigateur où vous travaillez** — elles ne se synchronisent pas automatiquement entre votre PC et votre téléphone. Utilisez la fonction **Exporter / Importer une sauvegarde** (onglet Paramètres) pour transporter vos données d'un appareil à l'autre : exportez sur l'appareil source, envoyez-vous le fichier `.json` par WhatsApp ou email, puis importez-le sur l'autre appareil.

---

## 1. Ouvrir l'application

### Sur ordinateur (Windows / Mac)
Double-cliquez simplement sur le fichier `ETS-LKB-Facturation.html`. Il s'ouvre dans votre navigateur habituel (Chrome, Edge, Firefox...). Vous pouvez le garder sur le Bureau ou dans un dossier dédié.

### Sur téléphone Android
1. Recevez le fichier (WhatsApp, email, transfert de fichier) et enregistrez-le dans vos téléchargements.
2. Ouvrez l'application **Fichiers** (ou "Mes fichiers"), repérez le fichier, appuyez dessus.
3. S'il vous propose une application pour l'ouvrir, choisissez **Chrome** (ou votre navigateur).

### Sur iPhone
1. Recevez le fichier (WhatsApp, email, AirDrop) et enregistrez-le dans l'app **Fichiers**.
2. Ouvrez l'app **Fichiers**, repérez le fichier, appuyez dessus — il s'ouvre dans Safari.

*(Voir la section 5 pour créer une icône d'accès rapide sur l'écran d'accueil.)*

---

## 2. Créer un document (devis, commande, livraison, facture)

1. Onglet **Nouveau document** (ouvert par défaut).
2. Choisissez le type de document en haut.
3. Renseignez le client : sélectionnez-le dans la liste s'il existe déjà, ou remplissez ses informations — il sera automatiquement ajouté à votre fichier clients au moment d'enregistrer.
4. Ajoutez vos articles avec **+ Ajouter une ligne**. Vous pouvez choisir un produit depuis votre catalogue (le prix se remplit automatiquement) ou taper une désignation libre. Les totaux (HT, TVA, TTC) se calculent automatiquement.
5. Cliquez sur **Enregistrer le document** pour le garder dans l'historique.
6. Cliquez sur **Aperçu / Imprimer / PDF** pour obtenir la version imprimable, prête à envoyer au client ou à imprimer.

## 3. Enregistrer en PDF ou imprimer

Le bouton **Aperçu / Imprimer / PDF** ouvre la fenêtre d'impression de votre navigateur. La suite dépend de votre appareil :

**Ordinateur** — Dans la liste des imprimantes, choisissez **« Enregistrer en PDF »** au lieu d'une imprimante physique, puis validez.

**Android (Chrome)** — Dans l'aperçu, appuyez sur l'icône d'impression. À la ligne « Imprimante », sélectionnez **Enregistrer au format PDF**, puis appuyez sur la flèche de téléchargement pour choisir où l'enregistrer.

**iPhone (Safari)** — Dans l'aperçu d'impression, pincez l'image avec deux doigts pour l'agrandir (cette astuce la transforme en document PDF plein écran). Appuyez ensuite sur l'icône de partage pour l'enregistrer dans **Fichiers**, ou l'envoyer directement par WhatsApp ou email.

## 4. Suivre vos factures (Historique)

Onglet **Historique** : liste de tous vos documents, filtrable par type ou par recherche (nom du client, numéro). Pour les factures, un menu déroulant permet de changer le statut de paiement (**Payé / Impayé / Partiel**) directement dans le tableau — la mise à jour est instantanée et sauvegardée.

## 5. Installer l'application comme une icône (raccourci)

**Android (Chrome)** : ouvrez le fichier dans Chrome → menu ⋮ (trois points) → **Ajouter à l'écran d'accueil**.

**iPhone (Safari)** : ouvrez le fichier dans Safari → icône de partage (carré avec une flèche vers le haut) → **Sur l'écran d'accueil**.

Une fois installée, l'application s'ouvre comme une app normale, en plein écran, sans barre d'adresse.

## 6. Gérer votre catalogue et vos clients

Onglets **Catalogue** et **Clients** : ajoutez, consultez ou supprimez vos produits/services et vos clients. Ils sont ensuite disponibles directement lors de la création d'un nouveau document, sans avoir à ressaisir les informations.

## 7. Modifier les informations de l'entreprise

Onglet **Paramètres** : nom, adresse, téléphone, email, site, et taux de TVA (20% par défaut). Ces informations apparaissent automatiquement sur tous vos documents.

---

## Reprise de vos anciennes données

Votre fichier Excel contenait déjà : le catalogue (Imprimante Canon, Imprimante HP), 2 clients, et 6 factures dans le registre. J'ai repris le catalogue et les 2 clients tels quels dans l'application. Je n'ai **pas** repris les lignes "Ordinateur Lenovo" (Réf_003 à Réf_017, prix incrémentés de 1 CDF à chaque ligne) — elles ressemblaient à des données de test plutôt qu'à un vrai catalogue ; ajoutez vos produits réels dans l'onglet Catalogue. Je n'ai pas non plus recréé les 6 anciennes factures (informations trop incomplètes dans le fichier d'origine pour les reconstituer fidèlement) — vous repartez avec un historique propre à partir d'aujourd'hui.

## Limite à connaître : pas de synchronisation automatique

Cette application n'a pas de serveur central — c'est un choix délibéré pour qu'elle fonctionne hors ligne et sans coût d'hébergement. La conséquence : si vous créez une facture sur votre téléphone, elle n'apparaîtra pas automatiquement sur votre PC. Pensez à exporter/importer régulièrement (section Paramètres) si vous travaillez sur plusieurs appareils, ou choisissez un seul appareil "maître" pour la facturation.
