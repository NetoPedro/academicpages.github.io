---
title: "Deep Learning Based Analysis of Prostate Cancer from MP-MRI"
collection: publications
permalink: /publication/2020-05-25-Deep-Learning-Prostate-Cancer-MP-MRI
excerpt: 'Classification, detection and segmentation of prostate cancer lesions from MP-MRI with deep learning based methods'
date: 2020-05-25
venue: 'Aalto Docs'
paperurl: 'https://www.researchgate.net/publication/342453524_Deep_Learning_Based_Analysis_of_Prostate_Cancer_from_MP-MRI'
---

[Download document here](https://www.researchgate.net/publication/342453524_Deep_Learning_Based_Analysis_of_Prostate_Cancer_from_MP-MRI)


The diagnosis of prostate cancer faces a problem with overdiagnosis that leads to damaging side effects due to unnecessary treatment. Research has shown that the use of multi-parametric magnetic resonance images to conduct biopsies can drastically help to mitigate the overdiagnosis, thus reducing the side effects on healthy patients. This study aims to investigate the use of deep learning techniques to explore computer-aid diagnosis based on MRI as input. Several diagnosis problems ranging from classification of lesions as being clinically significant or not to the detection and segmentation of lesions are addressed with deep learning based approaches.
This thesis tackled two main problems regarding the diagnosis of prostate cancer. Firstly, a deep neural network architecture, XmasNet, was used to conduct two large experiments on the classification of lesions. Secondly, detection and segmentation experiments were conducted, first on the prostate and afterward on the prostate cancer lesions. The for- mer experiments explored the lesions through a two-dimensional space, while the latter explored models to work with three-dimensional inputs. For this task, the 3D models explored were the 3D U-Net and a pretrained 3D ResNet-18. A rigorous analysis of all these problems was conducted with a total of two networks, two cropping techniques, two resampling techniques, two crop sizes, five input sizes and data augmentations experi- mented for lesion classification. While for segmentation two models, two input sizes and data augmentations were experimented. Moreover the experiments were conducted for both sequences independently, and within the lesion classification problem, the experi- ments were also conducted for both sequences simultaneously. However, while the binary classification of the clinical significance of lesions and the detection and segmentation of the prostate already achieve the desired results (0.870 AUC and 0.915 dice score respec- tively), the classification of the PIRADS score and the segmentation of lesions still have a large margin to improve (0.664 accuracy and 0.690 dice score respectively). It was also studied how some flaws in the dataset can be addressed to improve the results of all these problems. Further research on the problem is still needed, but nonetheless, this thesis established sufficient ground for future work to be conducted.


> **_NOTE:_** @mastersthesis{Aaltodoc:http://urn.fi/URN:NBN:fi:aalto-202006213908,
title={Deep Learning Based Analysis of Prostate Cancer from MP-MRI},
author={Carneiro Neto, Pedro},
year={2020-06-16},
language={en},
pages={74+4},
keyword={deep learning; computer vision; mp-MRI; prostate cancer; 3D segmentation; medical imaging},
type={G2 Pro gradu, diplomityö},
url={http://urn.fi/URN:NBN:fi:aalto-202006213908},
}
