# Bioinfo Project 2023
Pour commencer a traiter les données nous avons crées deux classes, data1 et data2 data1 est la classe contenant le dataframe des echantillons et des genes avec plusieurs getters,setters et methodes. La classe data2 est la classe contenant le dataFrame associé au fichier xml avec des getters et des methodes. 

# Premier traitement des données
Nous avons commencer par calculer les données de base, la median,la moyenne,std,max et min. On a afficher ces valeurs la pour chaque gene et echantillons.On peut deja realiser une premiere observation,on remarque que certains gene ont des valeurs particulierement elevées. Nous avons donc relever ces gens en questions, il s'agit de MATAL1, AluJb, L2a:L2, L2c:L2, MIR:MIR:SINE, MIRb:MIR:SINE, MIRc:MIR:SINE.

# PCA
Nous avons ensuite realisé une PCA, ce processus a pour but de reduire la dimension de nos données. Pour cela nous avons commencé par centrée et reduire nos données puis apres pour realisé une premiere reduction de nos données on a affiché le graphe de la variance explicité et on peut remarque que avec 51 composante principale on represente 80% de la variance explicite. On reduit donc nos données aux 50 premiers echantillons et on realise la PCA. Nous n'avons cependant pas reussit a obtenir de resultat avec les differents diagrammes. On a pas reussita identifier de combinaison lineaire entre les variables. 

# T-TEST 
