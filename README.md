# <center> This is ML Classification Fun Trial on Kvasir Dataset</center>


## 1) Dataset downloaded via command 
```bash
wget https://datasets.simula.no/kvasir/data/kvasir-dataset.zip
unzip kvasir-dataset.zip
```
Dataset description as per the website 
```
"Kvasir version 1

The first version of the Kvasir dataset (v1) consists of 4,000 images in 8 classes showing anatomical landmarks, phatological findings or endoscopic procedures in the GI tract, i.e., 500 images for each class. The anatomical landmarks are Z-line, pylorus and cecum, while the pathological finding are esophagitis, polyps and ulcerative colitis. In addition, we provide two set of images related to removal of polyps, the "dyed and lifted polyp" and the "dyed resection margins".

Kvasir Dataset v1

The kvasir-dataset.zip (size 1.2 GB) archive contains 4,000 images, 8 classes, 500 images for each class. The images are stored in the separate folders named accordingly to the name of the class images belongs to. The image files are encoded using JPEG compression. The encoding settings can vary across the dataset and they reflecting the a priori unknown endoscopic equipment settings. The extension of the image files is ".jpg".

Extracted Features (Kvasir Dataset v1)

The kvasir-dataset-features.zip (size 4.7 MB) archive contains the extracted visual feature descriptors for all the image from the Kvasir Dataset. The extracted visual features are stored in the separate folders and files named accordingly to the name and the path of the corresponding image files. The extracted visual features are the global image features, namely: JCD, Tamura, ColorLayout, EdgeHistogram, AutoColorCorrelogram and PHOG. Each feature vector consists of a number of floating point values. The size of the vector depends on the feature. The size of the feature vectors are: 168 (JCD), 18 (Tamura), 33 (ColorLayout), 80 (EdgeHistogram), 256 (AutoColorCorrelogram) and 630 (PHOG). The extracted visual features are stored in the text files. Each file consists of eight lines, one line per each feature. Each line consists of a feature name separated from the feature vector by colon. Each feature vector consists of a corresponding number of floating point values separated by commas. The extension of the extracted visual feature files is ".features"."
```

## 2) Explore the data
We have 8 directories, each with 500 .jpg images.
Directories' names (classes' names): 
1. dyed-lifted-polyps
2. dyed-resection-margins
3. esophagitis
4. normal-cecum
5. normal-pylorus
6. normal-z-line
7. polyps
8. ulcerative-colitis

## 3) Downloading and Exploring the features' file
using the following _Bash_ commands:
``` bash
wget https://datasets.simula.no/kvasir/data/kvasir-dataset-features.zip
unzip kvasir-dataset-features.zip
```
The data organized in the sae way.. 8 directories.. each with 500 files (txt files in csv format but file name ending in .features)

## 4) Analysis
### Imporing Needed Libraries 
### Reading the data