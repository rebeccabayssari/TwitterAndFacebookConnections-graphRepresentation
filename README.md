# Graph Analysis & Embeddings — Centralities, Community Detection, Node2vec & GNN

##  Description
Ce projet propose une analyse comparative des méthodes d’**analyse de graphes** appliquées à deux datasets réels (*Twitter* et *Facebook*).  
Il inclut :
- Analyse de **centralités** (degré, intermédiarité, proximité, valeur propre).  
- **Détection de communautés** avec plusieurs algorithmes et comparaison des métriques.  
- Étude des **embeddings** de graphes :
  - Approches classiques (Node2vec).  
  - Approches spectrales (Laplacian eigenmaps, auto-encodeurs).  
  - Approches basées sur les **Graph Neural Networks (GNNs)**.  

---

##  Datasets
Deux graphes issus de SNAP (Stanford Network Analysis Project) :

- **Twitter** : [twitter_combined.txt.gz](https://snap.stanford.edu/data/twitter_combined.txt.gz)  
- **Facebook** : [facebook_combined.txt.gz](https://snap.stanford.edu/data/facebook_combined.txt.gz)  

Les graphes sont non orientés et représentent des réseaux sociaux réels.

---

##  Étapes du projet

### 1. Prétraitement
- Chargement des graphes via **NetworkX**.  
- Vérification des propriétés (taille, densité, composantes connexes).  

### 2. Centralités
- Calcul et comparaison des centralités :  
  - **Degree Centrality**  
  - **Betweenness Centrality**  
  - **Closeness Centrality**  
  - **Eigenvector Centrality**  

### 3. Détection de communautés
- Expérimentations avec au moins **2 algorithmes** (Louvain, Infomap, Label Propagation).  
- Comparaison des résultats selon plusieurs métriques :  
  - Modularité  
  - Nombre et taille des communautés  
  - Densité intra-communauté  

### 4. Embeddings
- **Node2vec** : génération d’embeddings, visualisation (t-SNE/UMAP).  
- **Spectral approach** : embeddings basés sur la décomposition du Laplacien.  
- **GNN (Graph Convolutional Networks, GraphSAGE, etc.)** : apprentissage d’embeddings avec supervision légère.  
- Comparaison des approches (qualité des clusters, link prediction, classification de noeuds).  

### 5. Comparaison finale
- Analyse comparative entre méthodes classiques, spectrales et GNNs.  
- Interprétation selon les caractéristiques des graphes Twitter vs Facebook.  

---

## Résultats attendus
- Identification des noeuds les plus centraux dans chaque graphe.  
- Découverte et comparaison des communautés.  
- Visualisations des embeddings (2D).  
- Comparaison Node2vec vs Spectral vs GNN.  

---
