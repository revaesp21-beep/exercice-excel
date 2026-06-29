# PLAN D'ACTION COMMERCIAL ET MARKETING 2026

## PROBLÉMATIQUE IDENTIFIÉE
**Baisse de la satisfaction client (-15% en 2025)** : Impact sur le taux de rétention et la croissance du chiffre d'affaires

---

## INSTRUCTIONS EXCEL À APPLIQUER

### 1️⃣ DATE AUTO-INCRÉMENTÉE (Cellule B2)
```excel
=AUJOURD'HUI()
```
Cela affichera la date du jour et s'incrémentera automatiquement chaque jour.

---

### 2️⃣ PLAN D'ACTION AVEC INDICATEURS

| # | OBJECTIF GLOBAL | SOUS OBJECTIF | ACTION À MENER | RESPONSABLE | RESSOURCES | DATE BUT | INDICATEUR | ATTEINTE OBJECTIF | RÉSULTAT | TYPE OBJECTIF | % ÉCART OBJECTIF | ACTION CORRECTIVE À METTRE EN PLACE | OBJECTIF ATTENDU | RÉSULTAT |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Améliorer satisfaction | Augmenter NPS | Mettre en place programme fidélité client | Commercial | Budget 50K€ | 31/12/2026 | **NPS (Net Promoter Score)** | `=D5/E5*100` | **75** | **Qualitatif** | | Renforcer programme récompenses | 70 | 75 |
| 2 | Améliorer satisfaction | Réduire délais | Optimiser processus livraison | Logistique | Outils IT 20K€ | 31/12/2026 | **Taux service (%)** | `=(F5/E5)*100` | **98** | **Quantitatif** | `=((F5-E5)/E5)*100` | Investir dans automatisation | 95 | 98 |
| 3 | Réduire réclamations | Baisse réclamations | Former équipe support client | Ressources | Formation 15K€ | 30/06/2026 | **Taux satisfaction support** | `=H5/G5*100` | **92** | **Qualitatif** | | Augmenter effectif support | 85 | 92 |
| 4 | Croissance CA | Augmenter revenus | Lancer nouvelle offre produit | Marketing | Budget 30K€ | 31/12/2026 | **Chiffre affaires additionnel (€)** | `=(J5/I5)*100` | **580000** | **Quantitatif** | `=((J5-I5)/I5)*100` | Ajuster pricing stratégie | 500000 | 580000 |

---

### 3️⃣ FORMULE ATTEINTE DES OBJECTIFS

**Colonne "ATTEINTE OBJECTIF"** → Formule générale :
```excel
=(RÉSULTAT / OBJECTIF) * 100
```

**Exemples par ligne :**
- Ligne 1 : `=F5/E5*100` (si ratio)
- Ligne 2 : `=F5/E5*100` (taux en %)
- Ligne 3 : `=H5/G5*100`
- Ligne 4 : `=J5/I5*100`

**Notation Typologie :**
- **Quantitatif** = mesurable en chiffres/pourcentage
- **Qualitatif** = mesurable en satisfaction/perception

---

### 4️⃣ MISE EN FORME CONDITIONNELLE (Jeux d'icônes - 100% en vert)

**Appliquer à colonne "ATTEINTE OBJECTIF" :**

1. Sélectionner les cellules d'atteinte (ex: D5:D8)
2. Accueil → Mise en forme conditionnelle → Jeu d'icônes
3. Configurer :
   - 🟢 **Vert** : ≥ 100%
   - 🟡 **Jaune** : 80-99%
   - 🔴 **Rouge** : < 80%

---

### 5️⃣ FORMULE ÉCARTS (Quantitatifs uniquement - %)

**Colonne "% ÉCART OBJECTIF"** → Appliquer UNIQUEMENT aux indicateurs quantitatifs :

```excel
=((RÉSULTAT - OBJECTIF) / OBJECTIF) * 100
```

**Exemples :**
- Ligne 2 (Taux service) : `=((F6-E6)/E6)*100`
- Ligne 4 (CA additionnel) : `=((J6-I6)/I6)*100`

**Pour indicateurs qualitatifs** : Laisser vide ou mettre "N/A"

---

### 6️⃣ MISE EN FORME CONDITIONNELLE (Écarts ≤ -20% en rouge)

**Appliquer à colonne "% ÉCART OBJECTIF" :**

1. Sélectionner les cellules d'écart (ex: L6:L8)
2. Accueil → Mise en forme conditionnelle → Nouvelle règle
3. Formule personnalisée :
   ```excel
   =$L6<=-20%
   ```
   ou
   ```excel
   =L6<=-0.2
   ```
4. Format : Remplissage **ROUGE**

---

## SYNTHÈSE DES RÉSULTATS

| Indicateur | Objectif | Résultat | Atteinte | Écart | Statut |
|---|---|---|---|---|---|
| NPS | 70 | 75 | 107% | N/A | ✅ Dépassé |
| Taux service | 95% | 98% | 103% | +3% | ✅ Dépassé |
| Satisfaction support | 85% | 92% | 108% | N/A | ✅ Dépassé |
| CA additionnel | 500K€ | 580K€ | 116% | +16% | ✅ Dépassé |

---

## NOTES IMPORTANTES

✅ **Tous les objectifs sont atteints ou dépassés** → Performance positive  
✅ **Aucun écart critique** (< -20%) → Pas d'action corrective urgente  
✅ **Écarts quantitatifs positifs** → Investissements rentables

---

**Exercice préparé pour analyse de performance commerciale - MMRC 1ère année**
