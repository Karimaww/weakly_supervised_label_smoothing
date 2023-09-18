# Weakly Supervised Label Smoothing
This research project focused on the study and implementation of the paper titled "Weakly Supervised Label Smoothing" authored by Gustavo Penha and Claudia Hauff. The primary objective of this project was to gain a deeper understanding of the proposed label smoothing technique and its potential applications in the field of machine learning and natural language processing.

### Protocole d'évaluation
1. Collection des données libre accès -> MS-MARCO-Hard-Negatives.jsonl

2. Transformation des données en triplets de (qid, pid, relevance) en fonction du Negative Sampling

3. Pour chaque requête on considère 1 triplet pertinent et 9 non-pertinents

4. Apprentissage du modèle L2R et Lissage d'étiquettes selon le choix : LS, T-LS, WSLS, T-WSLS 5.Evaluation des performances

### Choix de la metrique d'evaluation
1. Pour chaque requête on classe les documents selon leur score de pertinence
2. On calcule la position moyenne du document pertinent dans l'ensemble des documents 3. Le score correspond à 10 - Avg_pos