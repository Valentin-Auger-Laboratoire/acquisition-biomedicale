# Acquisition de signaux biomédicaux

*[English version below](#biomedical-signal-acquisition)*

Travaux pratiques en binôme, ECUE 325 Systèmes de mesures nomades, EPISEN.

Ce dépôt présente deux chaînes d'acquisition analogiques de signaux physiologiques, du capteur jusqu'à l'affichage à l'oscilloscope : capteur, conditionnement par amplificateur opérationnel et filtrage passe-bas.

## Projets

| Projet | Grandeur mesurée | Chaîne de mesure | Fréquence de coupure du filtre |
|---|---|---|---|
| [Détection du pouls par capteur piézoélectrique](pouls-piezoelectrique/) | Vibrations de la carotide | Capteur piézoélectrique → convertisseur charge-tension → filtre RC (1 MΩ / 0,47 µF) | ≈ 0,34 Hz |
| [Mesure de la résistance cutanée](resistance-cutanee/) | Résistance électrique de la peau | Électrodes → pont de Wheatstone → amplificateur différentiel → filtre RC (330 kΩ / 0,47 µF) | ≈ 1,03 Hz |

Chaque dossier contient un README (en français puis en anglais) qui détaille l'objectif, le principe physique, le montage et le rôle de chaque composant, le calcul de la fréquence de coupure, les tests, les limites et les pistes d'amélioration. Les schémas et les captures d'oscilloscope se trouvent dans `images/`.

## Matériel utilisé

- Amplificateurs opérationnels
- Résistances et condensateurs de laboratoire
- Capteur piézoélectrique (projet 1) et électrodes cutanées (projet 2)
- NI VirtualBench : oscilloscope à signaux mixtes, alimentation continue et générateur de fonctions (pour le test de l'amplificateur du projet 2)

---

# Biomedical signal acquisition

Lab work in pairs, ECUE 325 Wearable Measurement Systems (Systèmes de mesures nomades), EPISEN.

This repository presents two analogue acquisition chains for physiological signals, from the sensor to the oscilloscope display: sensor, op-amp conditioning and low-pass filtering.

## Projects

| Project | Measured quantity | Measurement chain | Filter cut-off frequency |
|---|---|---|---|
| [Pulse detection with a piezoelectric sensor](pouls-piezoelectrique/) | Carotid artery vibrations | Piezoelectric sensor → charge amplifier → RC filter (1 MΩ / 0.47 µF) | ≈ 0.34 Hz |
| [Skin resistance measurement](resistance-cutanee/) | Electrical resistance of the skin | Electrodes → Wheatstone bridge → differential amplifier → RC filter (330 kΩ / 0.47 µF) | ≈ 1.03 Hz |

Each folder has a README (French first, then English) covering the objective, physical principle, circuit and role of each component, cut-off frequency calculation, tests, limitations and possible improvements. Diagrams and oscilloscope captures are in `images/`.

## Equipment

- Operational amplifiers
- Lab resistors and capacitors
- Piezoelectric sensor (project 1) and skin electrodes (project 2)
- NI VirtualBench: mixed-signal oscilloscope, DC power supply and function generator (used to test the project 2 amplifier)
