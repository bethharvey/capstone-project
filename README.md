# Machine Learning Model for Sparrow Classification

Beth Harvey

October 22, 2023

Data Analytics Capstone Project

# Abstract

It can be very difficult to distinguish between different types of sparrows, including between species that are native to North America and species introduced from Europe that are considered invasive here. Conservation efforts should be focused only on native species, so it is important to be able to accurately differentiate the two families in in order to identify and address problems that are faced by native birds. Using data from the AVONET database [9], the model described here can classify a sparrow specimen into the Passerellidae (new-world sparrows) family or the Passeridae (old-world sparrows) family based on observable traits and measurements with over 96% accuracy

# Introduction

As climate change, habitat loss, and disease continue to threaten wildlife through-out the world, detailed research is becoming more and more important. In 2023 alone, the U.S. Fish and Wildlife service took 21 species off of the Endangered Species Act list because they are now considered extinct [7]. Ten of those 21 species are birds. More research and resources are needed to develop effective conservation efforts. Some key components of bird conservation research are being able to accurately classify individual specimens, as well as being able to identify potential connections between different species. One of the most valuable resources for an effort like this is an extensive collection of detailed measurements for a wide variety of species. There are several different families of birds that are difficult to differentiate. One of the more challenging pairs is old-world sparrows and new-world sparrows [2]. Both families are part of the order Passeriformes, but the old-world sparrows make up the Passeridae family, while the new-world sparrows compose the Passerellidae family [4] [3]. New-world sparrows are native to North America, while old-world sparrows are native to Europe, but are also widespread in North America as introduced species [2]. It is important to be able to distinguish if a specimen is an old-world or new-world sparrow before exploring conservation efforts, so that these efforts can focus on helping native species, not introduced ones.

# Project Goals

The goal of this project is to build a model that can predict what taxonomic order a bird falls into based on several physical measurements. This could help researchers more accurately classify individuals when two or more species are possible. The model will be trained and tested using the AVONET dataset [8], a collective effort by researchers and volunteers to provide measurements of over 90,000 specimens of over 11,000 bird species. 

# Files

* AVONET Supplementary dataset 1.xlsx: Original full dataset for this project
* avonet_raw.csv: Main data file for this project, containing measurements of 90,020 bird specimens representing over 11,000 species
* avonet1_birdlife.csv: Measurement averages of each species, with habitat, lifestyle, and geographic information
* sparrow_classification_model.ipynb: Jupyter Notebook containing the code, analyses, and results of this project

# Links
 The relevant sheets (AVONET Raw Data and AVONET3 BirdTree) were saved CSV files and loaded into Pandas DataFrames for analysis in the [Jupyter Notebook project file](avonet_bird_identification.ipynb).
 The entire project can be viewed on [GitHub](https://github.com/bethharvey/capstone-project).
 The full report for this project can be viewed on [Overleaf](https://www.overleaf.com/read/hzzmcjpxkfvz#0b9003).

# Running the Code
Required: 
* Git
* Python 3.7 or higher
* Virtual environment:
    * `python3 -m venv .venv`
    * `source .venv/bin/activate`
    * `pip install -r requirements.txt`

# References 

1. Bhattarai, A., T., F.: Knnimputer. https://github.com/scikit-learn/
scikit-learn/blob/093e0cf14/sklearn/impute/_knn.py#L20 (2014), accessed
on October 31, 2023
2. Camfield, A.: Emberizidae buntings, american sparrows, and relatives. https://
animaldiversity.org/accounts/Emberizidae/ (2004), accessed on November 5,
2023
3. Cornell: New world sparrows—passerellidae. https://www.allaboutbirds.org/
guide/browse/taxonomy/Passerellidae (2023), accessed on November 5, 2023
4. Cornell: Old world sparrows—passeridae. https://www.allaboutbirds.org/
guide/browse/taxonomy/Passeridae (2023), accessed on November 5, 2023
5. Geron, A.: Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow.
O’Reilly (2022)
6. Pedregosa, F., Varoquaux, G., Gramfort, A., Michel, V., Thirion, B., Grisel, O.,
Blondel, M., Prettenhofer, P., Weiss, R., Dubourg, V., Vanderplas, J., Passos, A.,
Cournapeau, D., Brucher, M., Perrot, M., Duchesnay, E.: Scikit-learn: Machine
learning in Python. Journal of Machine Learning Research 12, 2825–2830 (2011)
7. Schuldheisz, C.: Fish and wildlife service delists 21 species from the endangered
species act due to extinction. https://www.fws.gov/press-release/2023-10/
21-species-delisted-endangered-species-act-due-extinction (2023), ac-
cessed on October 18, 2023
8. Shrestha, N.: Detecting multicollinearity in regression analysis. http://article.
sciappliedmathematics.com/pdf/ajams-8-2-1.pdf (2020), accessed on Novem-
ber 8, 2023
9. Tobias: Avonet: morphological, ecological and geographical data for all birds.
https://figshare.com/s/b990722d72a26b5bfead (2022), accessed on October 18,
2023
10. Tobias, J.A., Sheard, C., Pigot, A.L., Devenish, A.J.M., Yang, J., Sayol, F., Neate-
Clegg, M.H.C., Alioravainen, N., Weeks, T.L., Barber, R.A., Walkden, P.A., Mac-
Gregor, H.E.A., Jones, S.E.I., Vincent, C., Phillips, A.G., Marples, N.M., Monta ̃no-
Centellas, F.A., Leandro-Silva, V., Claramunt, S., Darski, B., Freeman, B.G., Breg-
man, T.P., Cooney, C.R., Hughes, E.C., Capp, E.J.R., Varley, Z.K., Friedman,
N.R., Korntheuer, H., Corrales-Vargas, A., Trisos, C.H., Weeks, B.C., Hanz, D.M.,
T ̈opfer, T., Bravo, G.A., Remeˇs, V., Nowak, L., Carneiro, L.S., Moncada R., A.J.,
Matysiokov ́a, B., Baldassarre, D.T., Mart ́ınez-Salinas, A., Wolfe, J.D., Chapman,
P.M., Daly, B.G., Sorensen, M.C., Neu, A., Ford, M.A., Mayhew, R.J., Fabio Sil-
veira, L., Kelly, D.J., Annorbah, N.N.D., Pollock, H.S., Grabowska-Zhang, A.M.,
McEntee, J.P., Carlos T. Gonzalez, J., Meneses, C.G., Mu ̃noz, M.C., Powell, L.L.,
Jamie, G.A., Matthews, T.J., Johnson, O., Brito, G.R.R., Zyskowski, K., Crates,
R., Harvey, M.G., Jurado Zevallos, M., Hosner, P.A., Bradfer-Lawrence, T., Maley,
J.M., Stiles, F.G., Lima, H.S., Provost, K.L., Chibesa, M., Mashao, M., Howard,
J.T., Mlamba, E., Chua, M.A.H., Li, B., G ́omez, M.I., Garc ́ıa, N.C., P ̈ackert,
M., Fuchs, J., Ali, J.R., Derryberry, E.P., Carlson, M.L., Urriza, R.C., Brzeski,
K.E., Prawiradilaga, D.M., Rayner, M.J., Miller, E.T., Bowie, R.C.K., Lafontaine,
R.M., Scofield, R.P., Lou, Y., Somarathna, L., Lepage, D., Illif, M., Neuschulz,
E.L., Templin, M., Dehling, D.M., Cooper, J.C., Pauwels, O.S.G., Analuddin, K.,
Fjelds ̊a, J., Seddon, N., Sweet, P.R., DeClerck, F.A.J., Naka, L.N., Brawn, J.D.,
Aleixo, A., B ̈ohning-Gaese, K., Rahbek, C., Fritz, S.A., Thomas, G.H., Schleuning,
M.: Avonet: morphological, ecological and geographical data for all birds. Ecology
Letters 25(3), 581–597 (2022). https://doi.org/https://doi.org/10.1111/ele.13898, 
https://onlinelibrary.wiley.com/doi/abs/10.1111/ele.13898