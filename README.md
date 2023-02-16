# Hidden Knowledge: Mathematical Methods for the Extraction of the Fingerprint of Medieval Paper from Digital Images

This repository is the official implementation of "Hidden Knowledge: Mathematical Methods for the Extraction of the Fingerprint of Medieval Paper from Digital Images" by Tamara G. Grossmann, Carola-Bibiane Schönlieb and Orietta Da Rold.

Medieval paper, a handmade product, is made with a mould which leaves an indelible  imprint on the sheet of paper. This imprint includes chain lines, laid lines and watermarks which are often visible on the sheet. Extracting these features allows the identification of paper stock and gives information about chronology, localisation and movement of books and people. Most computational work for feature extraction of paper analysis has so far focused on radiography or transmitted light images. While these imaging methods provide clear visualisation for the features of interest, they are expensive and time consuming in their acquisition and not feasible for smaller institutions. However, reflected light images of medieval paper manuscripts are abundant and possibly cheaper in their acquisition. In this paper, we propose algorithms to detect and extract the laid and chain lines from reflected light images. We tackle the main drawback of reflected light images, that is, the low contrast attenuation of lines and intensity jumps due to noise and degradation, by employing the spectral total variation decomposition and develop methods for subsequent line extraction. Our results clearly demonstrate the feasibility of using reflected light images in paper analysis. This work enables the feature extraction for paper manuscripts that have otherwise not been analysed due to a lack of appropriate images. We also open the door for paper stock identification at scale.

If you use this code, please cite:
```bibtex
@misc{grossmann2023,
  author = {Grossmann, Tamara G. and Schönlieb, Carola-Bibiane and Da Rold, Orietta},
  title = {Hidden Knowledge: Mathematical Methods for the Extraction of the Fingerprint of Medieval Paper from Digital Images},
  year = {2023}
}
```

## Requirements
The code is written in Python using the following packages:

- numpy
- scipy
- matplotlib
- skimage

Additionally, we assume that the user obtains the TV flow solution or the spectral TV decomposition of the images prior to using this code. There are multiple codes freely available to obtain the desired data, such as from Gilboa et al. (https://guygilboa.net.technion.ac.il/2020/10/09/spectral-total-variation-color/) or from Grossmann et al. (https://github.com/TamaraGrossmann/TVspecNET).
