<p align="center">
  <a href="https://github.com/GEL-3014-Equipe01">
    <img src="profile/logo-ulaval.webp" alt="Université Laval" width="300">
  </a>
</p>

<h1 align="center">Segment Grue — Ville Portuaire Intelligente 2026 — Équipe #1</h1>

<p align="center">
  <strong>Design III — GEL-3014 · Université Laval</strong>
</p>

---

## 🎯 Présentation

Ce dépôt regroupe le développement du **segment grue autonome** du projet  
*Ville Portuaire Intelligente (VPI) 2026*, incluant les volets **Software et Hardware (PCBs)**.

Le segment grue assure la **prise, le déplacement et le dépôt automatisé de marchandises**, en coordination avec des véhicules autonomes et une station de supervision.

Les objectifs principaux sont :

- Contrôle **temps réel** et sécuritaire des mouvements de la grue
- Gestion autonome des cycles de manutention
- Communication fiable entre sous-systèmes (grue, préhenseur, balance, station PC)
- Supervision, diagnostic et traçabilité des états système
- Conception et intégration de **cartes électroniques dédiées**

---

## 🧩 Architecture globale

Le système repose sur une approche de **co-conception matériel / logiciel**, où les cartes électroniques sont développées spécifiquement pour répondre aux contraintes de :

- temps réel
- robustesse électromécanique
- sécurité fonctionnelle
- intégration avec les sous-systèmes VPI

Sous-systèmes principaux :

- **Grue (STM32F429ZI-DISC1)**  
  Contrôle moteur, capteurs, sécurité et logique de séquencement

- **Préhenseur**  
  Pilotage de l’électroaimant, IMU, capteur infrarouge et communication Bluetooth

- **Balance**  
  Mesure de la quantité de marchandises transportées (phase véhicule)

- **Alimentation**
  Distribution de l'alimentation dans les sous-systèmes de la grue.

- **Station PC**  
  Supervision, diagnostic, communication Bluetooth/USB et planification de trajets

---

## ⚙️ Technologies utilisées

- **Langages** : C / C++, Python  
- **Microcontrôleurs** : STM32 (STM32F429ZI-DISC1)  
- **Communication** : Bluetooth, USB  
- **Capteurs** : IMU, capteur infrarouge  
- **Outils logiciels** : STM32CubeIDE, analyse CSV, cartes SD  
- **Outils matériels** : Altium Designer, tests électriques, PCBs

---

## 🚀 Mise en route (général)

1. Cloner le dépôt :

   ```bash
   git clone https://github.com/GEL-3014-Equipe01/REPO.git
   ```
2. Configurer l’environnement de développement correspondant au sous-système ciblé
3. Compiler et téléverser le code sur la carte STM32 ou lancer l’application Station PC

---

## 📄 Licence et cadre académique

Projet réalisé dans le cadre du cours **Design III — GEL-3014**
**Université Laval**

Ce dépôt est destiné à un usage académique. Toute réutilisation doit respecter le cadre pédagogique et les règles de l’Université Laval.

---

## 👥 Équipe

**Équipe #1 — Segment Grue**
Ville Portuaire Intelligente 2026
