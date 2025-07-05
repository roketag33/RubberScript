# RubberScript - Collection de Scripts Rubber Ducky

Collection de scripts Rubber Ducky pour tests d'intrusion et démonstrations de sécurité.

## ⚠️ Avertissement

Ces scripts sont conçus pour des **tests d'intrusion autorisés** et des **démonstrations de sécurité**. Utilisez-les uniquement sur des systèmes dont vous êtes propriétaire ou pour lesquels vous avez une autorisation explicite.

## 🎯 Scripts Disponibles

### 1. 🎹 Clavier Schizophrène
**Localisation :** `ClavierSchizophrene/`

Fait clignoter les LED du clavier (Caps Lock, Num Lock, Scroll Lock) de manière aléatoire.

- **Windows :** `windows_clavier_schizophrene_simple.txt` | `windows_clavier_schizophrene_avance.txt`
- **Linux :** `linux_clavier_schizophrene_simple.txt`
- **macOS :** `macos_clavier_schizophrene_simple.txt` (Caps Lock uniquement)

**Durée :** 60 secondes à 5 minutes
**Sortie :** Remise automatique à l'état normal

### 2. 🗣️ TTS Fantôme
**Localisation :** `TTSFantome/`

Utilise la synthèse vocale pour prononcer des phrases loufoques.

- **Windows :** `windows_tts_fantome.txt` (PowerShell + System.Speech)
- **Linux :** `linux_tts_fantome.txt` (espeak)
- **macOS :** `macos_tts_fantome.txt` (commande say)

**Durée :** 2 minutes
**Volume :** 50% (modéré)

### 3. 🎢 Tapis Roulant
**Localisation :** `TapisRoulant/`

Fait tourner l'écran à 0°, 90°, 180°, 270° en boucle.

- **Windows :** `windows_tapis_roulant.txt` (Ctrl+Alt+Flèches)
- **Linux :** `linux_tapis_roulant.txt` (xrandr)
- **macOS :** `macos_tapis_roulant.txt` (effets visuels alternatifs)

**Durée :** 2 minutes
**Failsafe :** Retour automatique à 0°

### 4. 📝 Pop-Up Shakespeare
**Localisation :** `PopUpShakespeare/`

Ouvre des éditeurs de texte avec des citations de Shakespeare et proverbes tech.

- **Windows :** `windows_popup_shakespeare.txt` (Notepad)
- **macOS :** `macos_popup_shakespeare.txt` (TextEdit)

**Durée :** 100 secondes
**Citations :** 10 citations différentes

### 5. 🎛️ Panneau de Contrôle Disco
**Localisation :** `PanneauControleDisco/`

Ouvre successivement 12 applets système Windows.

- **Windows :** `windows_panneau_disco.txt`

**Durée :** 90 secondes
**Applets :** Gestionnaire de tâches, Calculatrice, Services, etc.

### 6. 🌐 Navigateur Fugitif
**Localisation :** `NavigateurFugitif/`

Ouvre des URLs innocentes dans le navigateur par défaut.

- **Windows :** `windows_navigateur_fugitif.txt`

**Durée :** 80 secondes
**Sites :** Flickr, YouTube, Unsplash, Wikipedia, NASA

### 7. 🔊 Volume Yoyo
**Localisation :** `VolumeYoyo/`

Fait varier le volume de 0% à 100% puis retour de manière progressive.

- **Windows :** `windows_volume_yoyo.txt`

**Durée :** 2 minutes
**Phases :** Montée, Descente, Yoyo, Normalisation

### 8. 🖥️ Écran de Veille Vintage
**Localisation :** `EcranVeilleVintage/`

Active des screensavers vintage Windows (.scr natifs).

- **Windows :** `windows_ecran_veille_vintage.txt`

**Durée :** 3 minutes
**Screensavers :** Bulles, Mystify, Ribbons, Photos

## 🛡️ Fonctionnalités de Sécurité

### Failsafes Intégrés
- **Durée limitée :** Tous les scripts ont une durée maximale
- **Remise à l'état normal :** Automatique en fin de script
- **Pas de destruction :** Aucun script ne supprime ou modifie des fichiers
- **Pas d'UAC :** Aucun privilège administrateur requis

### Nettoyage Automatique
- Fermeture automatique des applications
- Effacement des historiques de commandes
- Remise des paramètres par défaut

## 📋 Utilisation

### 1. Préparation
1. Charger le script sur votre Rubber Ducky
2. Vérifier la compatibilité avec le système cible
3. S'assurer d'avoir l'autorisation nécessaire

### 2. Exécution
1. Insérer le Rubber Ducky dans le port USB
2. Le script s'exécute automatiquement
3. Attendre la fin du script (durée indiquée)

### 3. Récupération
1. Retirer le Rubber Ducky
2. Vérifier que le système est revenu à l'état normal
3. Documenter les résultats pour le rapport

## 🔧 Personnalisation

### Variables Configurables
Chaque script contient une section `CONFIGURATION` avec :
- **Durées :** Modifiables selon vos besoins
- **Répétitions :** Nombre de cycles
- **Délais :** Temporisations entre actions
- **Contenu :** Citations, URLs, phrases TTS

### Principes de Développement
- **DRY (Don't Repeat Yourself) :** Code modulaire et réutilisable
- **SOLID :** Responsabilités bien définies
- **KISS (Keep It Simple, Stupid) :** Simplicité avant tout
- **YAGNI (You Ain't Gonna Need It) :** Pas de fonctionnalités superflues

## 📊 Compatibilité

| Script | Windows | Linux | macOS |
|--------|---------|--------|--------|
| Clavier Schizophrène | ✅ | ✅ | ✅ |
| TTS Fantôme | ✅ | ✅ | ✅ |
| Tapis Roulant | ✅ | ✅ | ⚠️ |
| Pop-Up Shakespeare | ✅ | ❌ | ✅ |
| Panneau Disco | ✅ | ❌ | ❌ |
| Navigateur Fugitif | ✅ | ❌ | ❌ |
| Volume Yoyo | ✅ | ❌ | ❌ |
| Écran de Veille Vintage | ✅ | ❌ | ❌ |

**Légende :**
- ✅ Entièrement compatible
- ⚠️ Fonctionnalités limitées
- ❌ Non implementé (peut être ajouté)

## 🎓 Objectifs Pédagogiques

Ces scripts démontrent :
- L'importance de la **sécurité physique**
- Les **risques des ports USB**
- Les **techniques d'ingénierie sociale**
- Les **bonnes pratiques de sécurité**

## 📄 Licence

Ces scripts sont fournis à des fins éducatives et de test de sécurité uniquement. L'utilisateur est responsable de l'utilisation appropriée et légale de ces outils.

## 🤝 Contribution

Les contributions sont les bienvenues ! Respectez les principes DRY et SOLID lors de vos ajouts.

---

**Auteur :** RubberScript Team  
**Version :** 1.0  
**Date :** 2025

*"La sécurité est un processus, pas un produit" - Bruce Schneier* 