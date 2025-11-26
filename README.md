# SAOBOT – Valorant Colorbot Suite

[![Saobot preview](PHOTO%20SAOBOT/images/LOGIN.png)](https://saobot.shop)

**Saobot** est une interface premium qui réunit colorbot, overlay FOV évolué et module de spoofing USB autour d’une expérience inspirée de Valorant. L’objectif est de montrer comment automatiser la vision par couleur, l’intégration Arduino et le pilotage d’outils temps réel dans un cadre éducatif. Toute diffusion vise la recherche et l’apprentissage : l’utilisateur final est seul responsable de l’usage qu’il en fait. Le produit commercialisé est **uniquement fourni sous forme d’exécutable `Saobot.exe`** (aucun accès direct au code propriétaire) et s’installe via un setup tout-en-un qui configure automatiquement Python 3.10.

> ⚠️ **Avertissement pédagogique** – Saobot est fourni pour illustrer des concepts (vision couleur, hooking d’événements, automatisation HID). Nous ne cautionnons ni n’encourageons une utilisation contraire aux CGU de Riot Games ou d’un tiers. En téléchargeant ce dépôt vous acceptez d’assumer l’entière responsabilité des actions menées avec le logiciel.

> ✅ **Pré-requis critique** – L’installateur Saobot embarque Python **3.10** et gère tout automatiquement. Aucun prérequis manuel n’est demandé au client, mais Python reste nécessaire pour l’exécution (le setup le déploie pour vous).

---

## Pourquoi Saobot ?

> 🎬 **Présentation vidéo** – Remplacez l’URL ci-dessous par votre trailer YouTube/Vimeo pour présenter Saobot. L’aperçu est cliquable.
>
> [![Demo vidéo](https://img.youtube.com/vi/xxxxxxxxxxx/maxresdefault.jpg)](https://www.youtube.com/watch?v=xxxxxxxxxxx)

- **Expérience unifiée** : login premium, dashboard modulaire, télémétrie live et sauvegarde auto des profils.
- **Contrôle chirurgical** : overlay FOV ultra-fin (circle/square/triangle/star/heart), clignotement RGB, stroke dynamique et transparence totale.
- **Automations combo** : aimbot, triggerbot et anti-recul fonctionnent ensemble ou séparément avec profils tête/corps/pieds, offsets précis et temps de réaction au milliseconde.
- **Spoofing intégré** : flash Arduino Leonardo, clonage VID/PID et scripts CLI sans quitter l’app, idéal pour étudier la chaîne complète capture ➜ HID.
- **Observabilité** : panneau systèmes, FPS capture, statut Arduino, logs temps réel, crash reporter dédié.
- **Stack moderne** : PyQt5, numpy, dxcam/d3dshot, pyserial, packaging PyInstaller (Saobot.exe) prêt à diffuser.
- **Nouvelles fonctionnalités** : Onglet Support / User avec boîte de contact pour accès direct au site web et Discord, confirmation de redémarrage pour éviter les pertes accidentelles.

## Fonctionnalités détaillées

- **Portail de licence** : panneau « ACCÈS PREMIUM » avec ouverture de ticket/support rapide (Discord & site `https://saobot.shop`).
[![Login premium](PHOTO%20SAOBOT/images/LOGIN.png)](https://saobot.shop)
- **Command Center** :
  - *General* – backends de capture (dxcam/d3dshot), throttling, preview basse latence.
[![General tab](PHOTO%20SAOBOT/images/general.png)](https://saobot.shop)
[![General alt](PHOTO%20SAOBOT/images/geenral2.png)](https://saobot.shop)
  - *FOV Overlay* – formes multiples, animations RGB, blink, stroke ajustable.
[![FOV overlay](PHOTO%20SAOBOT/images/fov.png)](https://saobot.shop)
  - *Aimbot* – vitesses X/Y indépendantes, offsets dynamiques, profils présets, safe-mode pour humains.
[![Aimbot tab](PHOTO%20SAOBOT/images/aimbot.png)](https://saobot.shop)
[![Aimbot presets](PHOTO%20SAOBOT/images/aimbot%202.png)](https://saobot.shop)
  - *Triggerbot* – délais personnalisables, filtres de couleur, zones flexibles.
[![Triggerbot](PHOTO%20SAOBOT/images/Triggerbot.png)](https://saobot.shop)
  - *Anti-Recoil* – courbes personnalisées par arme/profil.
[![Anti recoil](PHOTO%20SAOBOT/images/Anti%20recoil.png)](https://saobot.shop)
  - *Spoofing* – détection HID, clonage VID/PID, upload sketch `hardware/microcontroller/microcontroller.ino`.
[![Spoofing view](PHOTO%20SAOBOT/images/spoof.png)](https://saobot.shop)
  - *User/System* – infos licence, HWID, charge CPU, FPS capture.
[![User tab](PHOTO%20SAOBOT/images/user.png)](https://saobot.shop)
- **Overlay avancé** : fenêtrage frameless toujours-on-top, hints transparents, support multi-color palette & blinking.
- **Journaux & support** : `logs/activity/` pour observer la calibration, `logs/crash/` pour analyser les exceptions, export simple lors d’une demande de support.

## Comparatif express

| Solution | Saobot | Colorbots classiques |
| --- | --- | --- |
| UI & UX | Dashboard complet, thèmes clair/sombre, overlay custom | Interfaces minimalistes, options limitées |
| Spoofing | Gestion Arduino intégrée + firmware prêt | Outils tiers à configurer soi-même |
| Support | Boutons dédiés vers Discord/boutique, logs structurés | Généralement Discord-only sans diagnostics |
| Packaging | `.exe` PyInstaller signé d’un icon Saobot | Scripts bruts nécessitant Python manuel |

## Acheter & activer Saobot

1. Rendez-vous sur **[saobot.shop](https://saobot.shop)** et choisissez une formule (support instantané sur **[Discord](https://discord.gg/aQMcEPgUUa)**).
2. Après paiement, **la clé de licence unique est envoyée par e‑mail** à l’adresse saisie lors de l’achat.
3. Téléchargez le **setup Saobot** qui installe automatiquement Python 3.12 + `Saobot.exe` + les ressources.
4. À la fin du setup, lancez Saobot, saisissez la clé reçue : elle est automatiquement **verrouillée sur la machine (HWID)** et **ne peut pas être partagée ni réutilisée ailleurs**.

> Support instantané : bouton **Support Discord** dans l’écran de connexion ou réponse directe au mail de licence.

## Utilisation rapide

1. Double-cliquez sur `SaobotSetup.exe` : il installe automatiquement Python 3.10 puis Saobot.
2. Lancez Saobot via le raccourci, saisissez la clé reçue par e‑mail ➜ validation et verrouillage sur votre PC.
3. Paramétrez les modules nécessaires (Aimbot/Triggerbot/Anti-recoil/FOV/Spoofing).
4. Cliquez sur **Lancer le bot** pour démarrer la session.
5. Utilisez l’onglet Spoofing pour cloner/téléverser votre périphérique si nécessaire.

## Prérequis techniques

- Windows 10/11 64 bits.
- GPU compatible DirectX 11 (dxcam/d3dshot).
- Python 3.10+ (le setup installe automatiquement Python 3.10 si besoin, aucun prérequis manuel).
- Arduino Leonardo (ou compatible) **obligatoire pour piloter la souris** (mouvements/simulation HID) et donc pour faire fonctionner l’aimbot en toute discrétion.
- Connexion Internet (activation licence, téléchargement arduino-cli, mises à jour).

## Architecture du dépôt

La distribution client fournie sur GitHub/saobot.shop contient strictement :

```
Saobot-package/
├─ Saobot.exe          # Application finale à lancer
├─ saobot.ico          # Logo (utilisable pour raccourcis)
└─ Guide.pdf           # Instructions et FAQ
```

> Le code source complet reste propriétaire et n’est pas distribué dans les livrables clients.

### Organisation du dépôt développeur

```
src/
├─ application/          # Modules Python publics + proxys qui chargent les extensions compilées
├─ compiled/             # Extensions Cython (.pyd) générées à partir des sources protégées
├─ configuration/        # Gestion des settings, logs et persistance locale
├─ system/               # Fonctions transverses (HWID, compat shim, etc.)
└─ protected/            # Sources en clair compilées en extensions Cython
```

- **Modifier un module protégé** ➜ travaillez dans `src/protected/application`, puis exécutez `python scripts/build_extensions.py build_ext --inplace` (ou via la task associée) pour régénérer les `.pyd` dans `src/compiled/application`.
- **Modifier un module protégé** ➜ travaillez dans `src/protected/<package>` (application/configuration/system), puis exécutez `python scripts/build_extensions.py build_ext --inplace` pour régénérer les `.pyd` correspondants dans `src/compiled/`.
- **Chargement runtime** : chaque module public (`src.application.*`, `src.configuration.settings`, `src.system.*`) est un proxy qui tente d'abord `src.compiled...` puis retombe automatiquement sur la source protégée pour le développement.
- **Couverture totale** : capture, souris, thèmes, gestion des settings et HWID résident désormais côté protégé et sont donc compilés au même titre que le cœur GUI/spoofer.
- **Utilitaires système** : `src/system/*` ne contient plus que des proxys minces ; la logique vit dans `src/protected/system` et reste alignée avec `_alias_module` défini dans `src/__init__.py`.
- Les artefacts de compilation intermédiaires sont stockés dans `build/cython/` et peuvent être nettoyés à volonté.

## Support & communauté

- **Site officiel** : [saobot.shop](https://saobot.shop)
- **Discord** : [discord.gg/aQMcEPgUUa](https://discord.gg/aQMcEPgUUa) (tickets, annonces, releases)
- **Logs** : joignez `logs/activity/` + `logs/crash/` lors d’un ticket pour accélérer le diagnostic.

## Avertissements juridiques

- Saobot est fourni « tel quel » pour un usage éducatif/démonstratif. Aucune garantie quant aux conséquences en jeu ou sur votre compte.
- L’utilisation peut violer les CGU de Valorant ou de Riot Games. Vous êtes seul responsable des risques encourus (bannissement, sanctions, pertes de compte, etc.).
- Revente, rétro-ingénierie, redistribution ou partage de licence interdits sans accord écrit.
- Toute tentative de contournement, de duplication ou de partage de clé (1 licence = 1 machine) entraîne la révocation immédiate sans remboursement.
- Build vérifié le **26/11/2025** sur **Windows 11** et **Windows 10** (tests exhaustifs : capture, aimbot, spoofing Arduino, packaging PyInstaller). Fonctionne parfaitement à cette date.

---

© 2025 – Saobot. Tous droits réservés. Toute diffusion hors contexte éducatif nécessite notre accord écrit.
