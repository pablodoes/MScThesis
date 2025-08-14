# MScThesis

This repository contains the code developed for the MSc thesis by Pablo Domínguez Estévez, titled Extreme Events Control based on Autoencoder-discovered Clusters. In the script "solver.py" the koldol script with the extra control functions is shown, while in the CODE folder all of the necessary scripts can be found.

The folders in the CODE directory are structured as follows:

1.- Data_Gen contains the scripts to generate the dataset using KolSol, generate plots and animations, and choose the artificial peaks for the initial conditions.
2.- CAE contains all of the scripts necessary for the CAE to work, the script that runs the whole process is cae_main.py.
3.- Clustering contains the scripts fr the three explored clustering methods. With respect to the MetaClustering with K-Means, the initial process is executed via main_with_loop_only_features.py and then with MetaClustering.py.
4.- Control contains all of the script performing the optimization and the testing.
  4.1.- The scripts containing noOpt are the ones that only test the system for a given bk vector and don't perform any optimization.
  4.2.- The script containing BULK are the ones that perform n runs to obtain relevant control system statistics.
  4.3.- The scripts containing betaVar1 or betaVar2 refer to the second and third control strategies explored in the MSc Thesis, modifying the Kolmogorov forcing term (2nd) or introducing another term (3rd).
5.- The folder Saves contains necessary information from clusteing, dimensionality reduction and control results.
6.- The folder SavesModBasedClust contains relevant information for the Modularity Based clustering process.
