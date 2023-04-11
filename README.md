# Bioinfo Project 2023
Nous avons créé deux classes pour traiter les données : Data1 et Data2. La classe Data1 contient un dataframe qui représente les échantillons et les gènes, ainsi que plusieurs méthodes, getters et setters pour manipuler les données. La classe Data2 quant à elle contient un dataframe associé à un fichier XML, ainsi que des méthodes et getters pour interagir avec les données. 

# Premier traitement des données
Nous avons débuté en calculant les statistiques de base telles que la médiane, la moyenne, l'écart-type, le maximum et le minimum. Nous avons ensuite affiché ces valeurs pour chaque gène et échantillon. Nous avons rapidement remarqué que certains gènes présentaient des valeurs particulièrement élevées. Après avoir identifié ces gènes, à savoir MATAL1, AluJb, L2a:L2, L2c:L2, MIR:MIR:SINE, MIRb:MIR:SINE et MIRc:MIR:SINE.

# PCA
Nous avons ensuite effectué une PCA (Analyse en Composantes Principales) pour réduire la dimension de nos données. Pour ce faire, nous avons centré et réduit nos données. Nous avons ensuite tracé le graphe de la variance explicite et avons constaté que nous pouvions représenter 80% de la variance explicite avec les 51 premières composantes principales. Nous avons donc réduit nos données aux 51 premiers échantillons et effectué la PCA. Malheureusement, nous n'avons pas réussi à obtenir de résultats concluants à partir des différents diagrammes que nous avons générés. Nous n'avons pas pu identifier de combinaison linéaire entre les variables.

# T-TEST 
Nous avons utilisé le test t pour comparer la moyenne des gènes entre deux groupes, les malades et les non-malades. Nous avons effectué un test t pour chaque gène, ce qui nous a permis de comparer la moyenne du groupe de malades à celle du groupe de non-malades. Les résultats ont été stockés dans une liste appelée pvalues. Les valeurs de pvalues représentent des mesures de probabilité indiquant le pourcentage de chance d'avoir une telle différence entre les deux moyennes. Lorsque ce pourcentage est faible, cela signifie qu'il y a de fortes chances que le gène permette de différencier les deux groupes.

Pour faciliter l'analyse de ces données, nous avons réalisé un volcano plot. Dans ce graphique, les points situés en haut de la figure représentent les variables ayant une différence significative et importante entre les deux groupes, et sont donc les plus intéressantes à étudier.
