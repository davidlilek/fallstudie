# fallstudie

## Tutorial
* I started with the tutorial from https://satijalab.org/seurat/articles/pbmc3k_tutorial.html 
* data for this tutorial are in the folder data
* fallstudie-basecode-tutorial.Rmd contains the code from the whole tutorial
* the corresponding html the output
* everything worked like in the tutorial

## Running it on new data
* info_data_new.txt contains the links for the data I used
* 001 has only a few data and only works with some adjustments (eg. max number of components for PCA and the results) and I had troubles to run Umap on this data
* 002: here I could rerun the whole tutorial without technial problems -> code: fallstudie-data-new-002.Rmd
* 002: I think at the end the nomenclature for the clusters has to be adapted manually -> maybe also some improvement for the code


## Recommendations
* as Dmitirj and Milica said: the running the whole code lasts quite some time
* maybe we should save some parts and vairables using .RDS http://www.sthda.com/english/wiki/saving-data-into-r-data-format-rds-and-rdata
* and set at the beginning of the notebook which parts should be re-run
* we should also make a bit of a folderstructure for infile outfiles reports...
* some parts of the code are "hard-coded": e.g. pbmc <- ScoreJackStraw(pbmc, dims = 1:15) -> if the pca is only calculated with 10 PCs the jack straw won't work
