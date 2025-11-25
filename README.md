# COLORBOT VALORANT MAIN GUI

**Créateur : moi**  \
**Tous droits réservés**

---

## Présentation
COLORBOT VALORANT MAIN GUI est une suite complète pour piloter un colorbot Valorant et gérer un module de spoofing USB Arduino Leonardo. L’application propose une interface moderne inspirée de Valorant, un panneau de connexion premium, ainsi qu’un centre de commandes unifié pour configurer, surveiller et personnaliser le bot en toutes circonstances.

## Fonctionnalités principales
- **Connexion sécurisée** via le panneau premium « ACCÈS PREMIUM » et synchronisation de licence.
- **Command Center** avec onglets dédiés pour l’aimbot, le triggerbot, l’anti-recul et le suivi matériel.
- **Overlay FOV** configurable en temps réel (couleurs, clignotements, stroke, etc.).
- **Calibration avancée** des sensibilités, DPI, profils de ciblage (tête/corps/pieds) et intensités prédéfinies.
- **Spoofing USB** intégré : détection des périphériques, clonage VID/PID et téléversement automatisé du firmware Arduino.
- **Diagnostic** complet : logs, résumé système, monitoring FPS capture et statut Arduino.

## Services proposés
- Gestion centralisée du colorbot (capture, traitement, clic automatisé) avec options de discrétion et personnalisation.
- Spoofing USB rapide via l’outil intégré, sans dépendances externes supplémentaires.
- Enregistrement automatique des paramètres et journaux pour faciliter le support et la maintenance.

## Prérequis
- Windows 10/11 64 bits.
- Python 3.10+ avec pip.
- Carte Arduino Leonardo (ou compatible) pour le spoofing.
- Connexion Internet pour le téléchargement d’arduino-cli si nécessaire.

## Installation
1. Cloner ou extraire ce dépôt localement.
2. Ouvrir un terminal PowerShell à la racine du projet (`COLORBOT VALORANT MAIN GUI`).
3. Créer un environnement virtuel (recommandé) :
   ```powershell
   python -m venv .venv
   .\.venv\Scripts\Activate.ps1
   ```
4. Installer les dépendances listées dans `docs/requirements.txt` :
   ```powershell
   pip install -r docs/requirements.txt
   ```
5. Vérifier la présence du fichier `configuration/settings.ini` (généré automatiquement au premier lancement si absent).

## Lancement et utilisation
1. Depuis l’environnement virtuel actif, exécuter :
   ```powershell
   python main.py
   ```
2. Saisir votre licence dans le panneau de connexion.
3. Configurer les paramètres souhaités dans le Command Center :
   - Onglet **General** pour le backend de capture, mode faible consommation, preview.
   - Onglet **FOV** pour l’overlay visuel.
   - Onglet **Aimbot** pour les vitesses, offsets, profils et puissances.
   - Onglet **Triggerbot** pour les délais et zones.
   - Onglet **Anti Recoil** pour la compensation automatique.
   - Onglet **Spoofing** pour lancer l’outil Arduino.
   - Onglet **User** pour les informations système/licence.
4. Cliquer sur **Lancer le bot** pour démarrer les modules sélectionnés.
5. Ouvrir l’outil de spoofing USB si besoin pour cloner votre souris et uploader le sketch Arduino.

## Structure du projet
```
COLORBOT VALORANT MAIN GUI/
├── assets/                # Icônes et éléments graphiques
├── build/pyinstaller/     # Fichiers de configuration de build
├── dist/                  # Artefacts générés (vidés par défaut)
├── docs/                  # Documentation et guides
├── hardware/microcontroller/  # Firmware et outils Arduino
├── logs/
│   ├── activity/          # Journaux applicatifs consolidés
│   └── crash/             # Crash dumps et traces
├── scripts/               # Scripts utilitaires (ex: generate_icon)
├── src/                   # Code Python principal (application + configuration)
└── main.py
```

## Maintenance & logs
- Les journaux applicatifs se trouvent désormais dans `logs/activity/` (settings, licences, erreurs courantes).
- Les rapports de crash détaillés sont regroupés dans `logs/crash/`.
- Les ressources Arduino sont conservées dans `hardware/microcontroller/`.

## Mentions légales
- SAOBOT Colorbot est un logiciel propriétaire. Toute reproduction, modification, rétro-ingénierie, diffusion ou revente sans accord écrit est strictement interdite.
- Chaque licence est nominative et liée au HWID/nom d’utilisateur déclaré. Le partage ou la duplication entraîne la révocation immédiate de la clé.
- Toute violation (contournement des protections, distribution non autorisée, modification du code) conduit à un bannissement définitif de l’utilisateur et de la licence, sans remboursement.
- L’utilisation du logiciel implique l’acceptation de ces conditions ainsi que des contrôles de licence automatisés.

---

© moi — Tous droits réservés. Toute reproduction ou diffusion est interdite sans autorisation préalable.
