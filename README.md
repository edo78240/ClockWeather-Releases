# ClockWeather

[![Dernière version](https://img.shields.io/github/v/release/edo78240/ClockWeather-Releases?label=Version&color=2563eb)](https://github.com/edo78240/ClockWeather-Releases/releases/latest) [![Android](https://img.shields.io/badge/Android-12%2B%20\(API%2031\)-3ddc84?logo=android&logoColor=white)](https://github.com/edo78240/ClockWeather-Releases/releases/latest) [![Sans GMS](https://img.shields.io/badge/Google%20Play%20Services-Non%20requis-0f172a)](#) [![Gratuit](https://img.shields.io/badge/Pub%20%26%20Tracking-Aucun-16a34a)](#)

**ClockWeather** est un widget Android d'horloge et de météo personnalisable, léger et fluide, conçu et testé pour fonctionner de manière fiable sur les surcouches **HyperOS**, **ColorOS**, **MagicOS** et **OriginOS** (ROM Globales/EU et ROM Chinoises).

* **100 % gratuit**, sans publicité et sans tracking
* **Zéro dépendance Google Play Services (GMS)**
* **Aucune clé API requise** pour la météo

---

## Téléchargement

👉 **[Télécharger la dernière version (APK)](https://github.com/edo78240/ClockWeather-Releases/releases/latest)**

> **Astuce :** Ce dépôt est également compatible avec **[Obtainium](https://github.com/ImranR98/Obtainium)** pour le suivi des mises à jour.

---

## Fonctionnalités

### Formats & Mise en page

* **2 formats de widget** : **4×1** (compact) et **4×2** (heure en grand centrée + ligne complète en dessous).
* Gestion dynamique des tailles, alignements et positions.

### Personnalisation visuelle

* **Arrière-plan** : fond uni (sombre ou clair) ou **Météo dynamique** adaptée aux conditions actuelles.
* **Transparence** réglable de **0 à 100 %**.
* Personnalisation des **polices** et des **couleurs**.
* **Animation 60 fps optionnelle** : animation aller/retour fluide (60 frames) à partir d'un émoticône ou d'une image de votre galerie (`PNG`/`JPG`), affichable seule ou combinée aux prévisions.

### Météo & Prévisions (sans clé API)

* Prévisions jusqu'à **5 jours** avec indicateur de la dernière synchronisation.
* **Sélecteur de source météo** directement dans les réglages, avec bascule automatique en cas d'indisponibilité :

| Source météo | Détails |
| :--- | :--- |
| **Automatique — Open-Meteo** *(par défaut)* | Sélection optimale automatique (`best_match`) |
| **Météo-France** | Modèles AROME / ARPEGE via Open-Meteo |
| **ECMWF** | Modèle européen |
| **DWD ICON** | Modèle allemand |
| **NOAA GFS** | Modèle américain |
| **MET Norway** | Serveur direct `api.met.no` (indépendant d'Open-Meteo) |

### Raccourcis cliquables

* Ouverture directe de vos applications **Horloge** et **Météo** au clic sur le widget.
* **Raccourci réglages discret** *(idéal sur ColorOS lorsque Horloge et Météo sont déjà assignées)* :
  * **Ville affichée** : petit trait discret cliquable au-dessus du nom de la ville.
  * **Ville masquée** : émoticône personnalisable à côté des prévisions météo.

### Mises à jour intégrées (à partir de la v1.16)

* Vérification automatique silencieuse (1 fois toutes les 12 h à l'ouverture des réglages) ou manuelle via le bouton **Vérifier les mises à jour (GitHub)**.
* Téléchargement direct depuis GitHub Releases avec **vérification cryptographique SHA-256** avant installation.
* Mise à jour en place sans perte de vos widgets ni de vos réglages.

---

## Compatibilité

| Système / Surcouche | Version minimale |
| :--- | :--- |
| **Android** | Android 12 (API 31) à Android 17 *(ROM Globale/EU et Chinoise)* |
| **HyperOS / MIUI** | HyperOS 1.0+ *(MIUI 13 / 14 sous Android 12+)* |
| **ColorOS** | ColorOS 12+ |
| **MagicOS** | MagicOS 6.0+ |
| **OriginOS / Funtouch OS** | OriginOS Ocean (2.0+) / Funtouch OS 12+ |

---

## Guide d'installation

### Première installation

1. Téléchargez le fichier `ClockWeather-vX.Y.apk` depuis la [dernière Release](https://github.com/edo78240/ClockWeather-Releases/releases/latest).
2. Installez l'APK (autorisez l'installation depuis votre navigateur ou gestionnaire de fichiers si demandé).
3. Ajoutez le widget **ClockWeather** (`4×1` ou `4×2`) sur votre écran d'accueil.
4. Accordez l'autorisation **Localisation précise → Toujours autoriser** pour la récupération automatique de la météo.

### Mise à jour depuis une version précédente

* **Depuis une version < v1.16 (Release officielle)** : téléchargez et ouvrez `ClockWeather-v1.16.apk` pour mettre à jour en place en conservant vos widgets et réglages.
* **À partir de la v1.16** : les mises à jour suivantes se font directement depuis les réglages de l'application *(autorisez une seule fois « Installer des applis inconnues » pour ClockWeather)*.

---

## Réglages recommandés (surcouches chinoises)

Les gestionnaires d'énergie de **HyperOS**, **ColorOS**, **MagicOS** et **OriginOS** peuvent bloquer les actualisations en arrière-plan par défaut. Pour garantir des mises à jour météo régulières :

1. Ouvrez **Paramètres → Applications → ClockWeather** *(ou appui long sur l'icône → Infos appli)*.
2. **Batterie / Économiseur d'énergie** : sélectionnez **Aucune restriction** *(ou Autoriser l'activité en arrière-plan)*.
3. **Lancement automatique (Autostart)** : activez l'option pour **ClockWeather**.
4. **Localisation** : vérifiez que l'accès est bien réglé sur **Toujours autoriser** avec **Position exacte**.

---

## Sécurité & Intégrité

Chaque Release publiée sur ce dépôt inclut :

* L'APK Release signé (`ClockWeather-vX.Y.apk`)
* Le fichier de métadonnées `update.json` contenant l'empreinte **SHA-256** vérifiée automatiquement par l'application avant toute installation.