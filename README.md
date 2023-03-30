# Project structure

This repository contains the notebooks and data related to the computer vision blockweek at HSLU in February 2023.
Each member of our group (Giancarlo, Philipp, Levin) tried to classify skin tissue using different CNN architectures.

The results that were presented on the 30.03.2023 are contained in the script in the folder "Image_classification_Giancarlo". 
Furthermore, the Variational Autoencoderscripts are present in the related folder.
## Data

This data set represents a collection of textures in histological images of human colorectal cancer. It contains two files:
"Kather_texture_2016_image_tiles_5000.zip": a zipped folder containing 5000 histological images of 150 * 150 px each (74 * 74 µm). Each image belongs to exactly one of eight tissue categories (specified by the folder name).
"Kather_texture_2016_larger_images_10.zip": a zipped folder containing 10 larger histological images of 5000 x 5000 px each. These images contain more than one tissue type.

## Image format

All images are RGB, 0.495 µm per pixel, digitized with an Aperio ScanScope (Aperio/Leica biosystems), magnification 20x. Histological samples are fully anonymized images of formalin-fixed paraffin-embedded human colorectal adenocarcinomas (primary tumors) from our pathology archive (Institute of Pathology, University Medical Center Mannheim, Heidelberg University, Mannheim, Germany).

## Ethics statement

All experiments were approved by the institutional ethics board (medical ethics board II, University Medical Center Mannheim, Heidelberg University, Germany; approval 2015-868R-MA). The institutional ethics board waived the need for informed consent for this retrospective analysis of anonymized samples. All experiments were carried out in accordance with the approved guidelines and with the Declaration of Helsinki.


The dataset serves as a much more interesting MNIST or CIFAR10 problem for biologists by focusing on histology tiles from patients with colorectal cancer. In particular, the data has 8 different classes of tissue (but Cancer/Not Cancer can also be an interesting problem). 

The dataset is composed of two parts:
- The small images that will be used to test the classification models
- The big microscope images (5000x5000)

The first dataset is quite small but the second are much bigger (250 Mb and 700 Mb). You can get them on 
kaggle: https://www.kaggle.com/code/kmader/histology-mnist-csv-overview/data. The original data can be found on zenodo: https://zenodo.org/record/53169#.Y3R-ty8w3Lu
Instructions and Code

[1] http://www.ceebl.manchester.ac.uk/ebl/, Last Accessed 13th November 2022.
