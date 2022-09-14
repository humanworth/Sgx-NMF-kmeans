# Sgx-NMF-kmeans
<br> This program requires following packages to be installed properly
<br> 1- python 3.10
<br>	a- scikit-learn version 1.1.2
<br>	b- pandas version 1.4.4
<br>
<br>2- install and configure linux-sgx sdk 
<br>	a- run the following command :
<br>	 source [your sgxsdk environment file]



----------------------------------------------------------------------------------
After the prequisites are installed, move into the project folder and do the following:
<br>
1- make SGX_MODE=DEB
<br>
<br>Once the app is built successfully, run it through the following command:
<br>./app [dataset_file] [number_of_clusters] [number_of_cells] [number_of_genes]
<br>
<br>Example for small database:
<br>./app dataset/comb_S.csv 3 1200 1000
<br><br>

<br>in the next step, you will be asked to enter the number of threads that you wish to run the codes on.

-------------------------------------------------------------------------------
................... Wait for computations to be done.............................

<br><br><br><br>


<br>There will be 4 output file after the program successfully run.
<br>1- labels.seal  			[which is the encrypted class membership output]
<br>2- unsealed_labels.txt.txt  	[which is decrypted version of labels.seal]
<br>3- dataset.seal  			[which is the encrypted dataset]
<br>4- centroids.seal			[which is the encrypted of final centrois]

