# Brain-Tumor-Search

A	fost folosita baza de date : https://www.kaggle.com/navoneel/brain-mri-images-for-brain-tumor-detection
Aceasta contine 98 de imagini MRI ale unor creiere sanatoase si 145 ale unor creiere cu tumoare.

Programul a fost realizat in python3, google colab. Am creat o retea neuronala formata din 3 seturi de straturi convolutionale si max pooling, un start de turtire, unul dens si inca unul cu functia de activare sigmoid.
Imaginile au fost impartite in 3 seturi: de antrenament, de validare si de testare.

Am eliminat stratul dens cu functia de activare sigmoid, iar noua retea am folosita pentru a obtine descriptorii imaginii. Am aplicat functia de similitudine cosinus pentru a afla cat de mult se aseamana imaginile intre ele.
Pentrue evaluarea subiectiva am afisat imaginea originala alaturi de 5 cele mai asemanatoare imagini cu ea.
Pentru evaluarea obiectiva am masurat TP,FP,TN,FN si am calculate precizia si reamintirea.
S-a obtinut precizia: 0.804 si reamintirea: 0.997

In a doua parte a proiectului am luat matricea cu vectorii descriptori, am aplicat PCA si am antrenat un cluster de tipul K-means.
