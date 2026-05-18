# Politique de confidentialité — Workout Session

**Dernière mise à jour : 14 mai 2026**

La présente Politique de confidentialité décrit comment l'application mobile **Workout Session** (« l'Application », « nous ») collecte, utilise et protège tes données personnelles lorsque tu utilises notre service.

En utilisant Workout Session, tu acceptes la collecte et l'utilisation d'informations conformément à la présente politique.

---

## 1. Responsable du traitement

L'éditeur de Workout Session est responsable du traitement des données collectées via l'Application.

**Contact :** [À COMPLÉTER — ton email de contact, ex: privacy@workoutsession.app]

---

## 2. Données que nous collectons

### 2.1 Données fournies directement par l'utilisateur
- **Adresse email** (compte classique ou via Sign in with Apple / Google)
- **Nom complet** (optionnel)
- **Mot de passe** (stocké de manière chiffrée avec bcrypt — nous ne pouvons pas le lire)
- **Photo de fond d'écran personnalisée** (uniquement pour les abonnés Premium, stockée sur nos serveurs sous forme chiffrée base64)

### 2.2 Données générées par l'utilisation de l'app
- **Exercices créés** : nom, description, groupe musculaire, niveau, séries, répétitions, temps de repos
- **Sessions d'entraînement** : date, heure, série, poids et reps réels effectués
- **Planning hebdomadaire** : assignations d'exercices par jour
- **Préférences** : unité (kg/lbs), langue

### 2.3 Données techniques
- **Identifiants de connexion fournis par tiers** :
  - `apple_id` (identifiant stable Apple Sign-In)
  - `google_id` (identifiant stable Google OAuth)
- **Identifiants de paiement** :
  - `stripe_customer_id` et `stripe_subscription_id` (pour les abonnements web)
  - Identifiants de transaction Apple IAP / Google Play Billing (pour les abonnements mobile)
- **Date de création du compte**
- **Adresses IP** des requêtes (logs serveur, conservés 30 jours)

### 2.4 Données que nous NE collectons PAS
- ❌ Pas de tracking publicitaire
- ❌ Pas d'identifiants de publicité (IDFA, AAID)
- ❌ Pas de géolocalisation
- ❌ Pas de données du téléphone (contacts, photos hors fond d'écran choisi explicitement par toi, micro, caméra)
- ❌ Pas de données biométriques
- ❌ Pas de partage avec des courtiers de données

---

## 3. Comment nous utilisons tes données

Nous utilisons tes données uniquement pour les finalités suivantes :

| Finalité | Base légale (RGPD) |
|----------|-------------------|
| Te permettre de créer et utiliser ton compte | Exécution du contrat |
| Stocker tes exercices, séances et progression | Exécution du contrat |
| Gérer ton abonnement Premium (paiement, renouvellement, résiliation) | Exécution du contrat |
| Générer des séances personnalisées (Premium Coach) | Exécution du contrat |
| Te répondre quand tu nous contactes pour assistance | Intérêt légitime |
| Sécuriser le service (anti-fraude, logs techniques) | Intérêt légitime |

Nous **n'utilisons jamais** tes données pour de la publicité ciblée ou pour les revendre.

---

## 4. Tiers avec lesquels nous partageons des données

Nous partageons un minimum strict de données avec les prestataires techniques suivants :

| Tiers | Données partagées | Finalité | Localisation |
|-------|------------------|----------|--------------|
| **Stripe, Inc.** | Email, ID client, montant | Traitement des paiements (abonnements web) | États-Unis (clauses contractuelles types) |
| **Apple Inc.** | Identifiant de transaction IAP | Vérification des achats in-app (iOS) | États-Unis |
| **Google LLC** | Token d'achat Play Billing | Vérification des achats in-app (Android) | États-Unis |
| **Anthropic, PBC** (Claude AI) | Requête de génération de séance anonymisée (groupes musculaires, niveau, durée — **PAS** ton email ni tes données perso) | Génération des séances Premium Coach | États-Unis |
| **MongoDB Atlas** | Toutes données ci-dessus | Hébergement de la base de données | UE (Frankfurt) |

Aucun de ces tiers n'a le droit d'utiliser tes données à d'autres fins que celle pour laquelle elles ont été transmises.

---

## 5. Durée de conservation

| Donnée | Durée |
|--------|-------|
| Compte actif (toutes données) | Tant que ton compte existe |
| Compte supprimé par toi | Effacement immédiat de toutes les données personnelles et workout |
| Logs serveur techniques (IP, requêtes) | 30 jours |
| Données de facturation (Stripe) | 10 ans (obligation comptable) |
| Sauvegarde de base de données | 90 jours après suppression du compte |

---

## 6. Tes droits (RGPD)

En tant que résident de l'Union européenne (et indépendamment), tu as les droits suivants :

- **Droit d'accès** : obtenir une copie de toutes tes données
- **Droit de rectification** : corriger des données inexactes
- **Droit à l'effacement** (« droit à l'oubli ») : supprimer ton compte et toutes tes données
- **Droit à la portabilité** : recevoir tes données dans un format structuré (JSON)
- **Droit d'opposition** : refuser certains traitements
- **Droit à la limitation** : restreindre le traitement temporairement

Pour exercer ces droits : **[À COMPLÉTER — ton email de contact]**

Tu peux supprimer ton compte directement depuis l'app (Profil → Supprimer mon compte) — l'effacement est immédiat et irréversible.

Si tu estimes que tes droits ne sont pas respectés, tu peux saisir la **CNIL** : https://www.cnil.fr/fr/plaintes

---

## 7. Sécurité

Nous appliquons les mesures techniques et organisationnelles suivantes :

- ✅ Mots de passe stockés avec **bcrypt** (jamais en clair)
- ✅ Communications chiffrées en **HTTPS/TLS 1.2+**
- ✅ Tokens JWT signés et à durée limitée
- ✅ Accès à la base de données restreint et audité
- ✅ Pas de logs des mots de passe ni des données de carte bancaire (Stripe gère tout)
- ✅ Webhooks Stripe et notifications Apple **vérifiés cryptographiquement** (signature)

---

## 8. Apple Sign-In et adresses email privées

Si tu choisis « Hide My Email » au moment de Sign in with Apple, Apple nous fournit une adresse anonymisée de la forme `xxxxx@privaterelay.appleid.com`. Cette adresse fonctionne normalement : les emails que nous t'envoyons sont transférés vers ta vraie boîte par Apple, sans que nous puissions voir ta véritable adresse.

Tu peux modifier ce choix à tout moment depuis : **iPhone → Réglages → Apple ID → Connexion et sécurité → Connexion avec Apple → Workout Session**.

---

## 9. Enfants

Workout Session n'est pas destinée aux enfants de moins de 13 ans. Nous ne collectons pas sciemment de données d'enfants. Si tu es parent et constates que ton enfant a créé un compte, contacte-nous et nous supprimerons les données immédiatement.

---

## 10. Modifications de cette politique

Nous pouvons mettre à jour cette politique pour refléter les évolutions de la loi ou de notre service. La date en haut du document indique la dernière modification. Les changements majeurs te seront notifiés dans l'app à l'ouverture suivante.

---

## 11. Contact

Pour toute question concernant cette politique ou tes données :

📧 **[À COMPLÉTER — email de contact]**

---

*Document rédigé en français, conforme au RGPD (Règlement UE 2016/679) et au CCPA (California Consumer Privacy Act).*
