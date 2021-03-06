## 3-D Density Kernel Estimation for Counting in Microscopy Image Volumes Using 3-D Image Filters and Random Decision Trees  

DOI of this repository.
![DOI](https://zenodo.org/badge/63594339.svg)(https://zenodo.org/badge/latestdoi/63594339)


From journal paper:
DOI of journal article: 10.1007/978-3-319-46604-0_18

Waithe D. et al. (2016) 3-D Density Kernel Estimation for Counting in Microscopy Image Volumes Using 3-D Image Filters and Random Decision Trees. In: Hua G., Jégou H. (eds) Computer Vision – ECCV 2016 Workshops. ECCV 2016. Lecture Notes in Computer Science, vol 9913. Springer, Cham

[Online link to conference paper](http://link.springer.com/chapter/10.1007/978-3-319-46604-0_18)

[Direct link to pre-submission pdf](submissionFinal.pdf)


#### Abstract

We describe a means through which cells can be accurately counted in 3-D microscopy image data, using only weakly annotated images as input training material. We update an existing 2-D density kernel estimation approach into 3-D and we introduce novel 3-D features which encapsulate the 3-D neighbourhood surrounding each voxel. The proposed 3-D density kernel estimation (DKE-3-D) method, which utilises an ensemble of random decision trees, is computationally efficient and achieves state-of-the-art performance. DKE-3-D avoids the problem of discrete object identification and segmentation, common to many existing 3-D counting techniques, and we show that it outperforms other methods when quantification of densely packed and heterogeneous objects is desired. In this article we successfully apply the technique to two simulated and to two experimentally derived datasets and show that DKE-3-D has great potential in the biomedical sciences and any field where volumetric datasets are used.

#### Summary Figure
![alt](summary_fig.png)

Training scheme in 3-D. (A) Input image volume with dot annotation (red, exaggerated) in xy dimension and also orthogonal max projections (zy, right) (xz, bottom). (B) Ground-truth density function in xy dimension and also orthogonal max projections (zy, right) (xz, bottom). Scale bar is 40 pixels. (C) Schematic for data input and output with the ensemble of decision trees. Input features are calculated from input image volumes and associated with ground-truth density volume. Sampled voxel features and associated ground-truth voxels are then concatenated into a long vector (number of voxels, number of features) and used to train the ensemble of decision trees. Each decision tree receives a boot-strap sample of input voxels. At inference time, for a given voxel, the output density is calculated using the average output of each tree for that voxel to produce the predicted density image. 

#### Datasets


Datasets used in paper, please see paper for additional details:

[Dataset 1](http://sara.molbiol.ox.ac.uk/dwaithe/software/data/dataset1.zip) Simulation closely resembles cultures of HL60 cells with their nuclei stained with DAPI, which is a fluorescent DNA binding agent commonly applied in the life sciences for cell counting.

[Dataset 2](http://sara.molbiol.ox.ac.uk/dwaithe/software/data/dataset2.zip) The second dataset  has been designed to closely simulate colon tissue sampled from human patients suffering from adenocarcinoma, a type of cancer.

[Dataset 3](http://sara.molbiol.ox.ac.uk/dwaithe/software/data/dataset3.zip) 3-D confocal micrographs acquired from Drosophila melanogaster fly brains cultured for several days, fixed and then stained with DAPI nuclear dye, which stained the nuclei of the cells within the brain. 

[Dataset 4](http://sara.molbiol.ox.ac.uk/dwaithe/software/data/dataset4.zip) deep 3-D volume imaging of the heart organ from intact Zebrafish embryos.
