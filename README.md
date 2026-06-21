# 📈 FC Annecy — Analyse de saison (Ligue 2, 2025/2026)

Projet personnel d'**analyse de la trajectoire d'une équipe sur une saison** de Ligue 2 (FC Annecy, 2025/2026), de la **collecte des données** à leur **analyse**.

L'objectif : à partir de données de match publiques, construire un jeu de données propre puis dégager les **tendances de la saison** (dynamique de résultats, points cumulés, différence de buts, impact domicile/extérieur, possession, formations).

> 📊 **Données publiques** (statistiques de matchs type FBref) : résultats, scores, possession, formations, capitaine, arbitre — toutes des informations publiquement disponibles. Aucune donnée confidentielle.

---

## 🧰 Stack

`Python` · `pandas` · `numpy` · `Matplotlib` · `requests` / `BeautifulSoup` (collecte) · `Jupyter`

## 📂 Structure

```
data/raw/         Données de match brutes de la saison (TSV)
data/processed/   Jeu de données enrichi (features : points/diff cumulés, domicile, etc.)
notebooks/
  01_data_collection.ipynb   Collecte & structuration des données
  02_season_analysis.ipynb   Analyse de la saison & visualisations
```

### Variables principales
Journée, lieu (dom./ext.), résultat, buts pour/contre, possession, affluence, formation, formation adverse, arbitre — enrichies de : différence de buts, points, points cumulés, différence de buts cumulée.

## ▶️ Lancer le projet

```bash
pip install -r requirements.txt
jupyter lab   # puis ouvrir notebooks/01 puis 02
```

---

*Projet réalisé dans le cadre de ma spécialisation en data appliquée au football (alternance recherchée — Data Analyst / Football Analytics).*
