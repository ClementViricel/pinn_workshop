# Atelier PINN

Page pédagogique interactive pour comprendre les **Physics-Informed Neural Networks (PINN)**.

👉 **Voir la page : https://clementviricel.github.io/pinn_workshop/**

## Ce que montre la page

- **Problème direct** : un petit réseau de neurones apprend la solution de l'EDO `u′ = −k u` avec `u(0) = 1`, sans solveur, en pénalisant le résidu de l'équation sur des points de collocation.
- **Problème inverse** : à partir de quelques mesures bruitées, le réseau retrouve le paramètre inconnu `k` en l'entraînant avec ses poids.
- **Lien avec l'article de référence** de Raissi, Perdikaris & Karniadakis (2019), qui fait la même chose sur l'équation de Burgers.
- **Transposition aux modèles osseux** : ce qui change pour un système d'EDO de remodelage (plusieurs variables d'état, paramètres de taux et de seuils, données partielles).

## Fonctionnement

Tout tourne dans le navigateur, en JavaScript pur, sans aucune librairie : le réseau (une couche cachée de 20 neurones `tanh`), ses dérivées exactes et l'optimiseur Adam sont écrits à la main dans `index.html`. Seules les polices viennent de Google Fonts.

Pour l'utiliser en local, il suffit d'ouvrir `index.html` dans un navigateur.

## Licence

MIT, voir [LICENSE](LICENSE).
