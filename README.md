# Spine-MSCA
The dataset is accompanied by a set of labels that indicate the regions of interest in the images. It contains a total of 426 lumbar T2 sagittal MRI images, each from a different patient. The resolution was uniformly adjusted to 512x512 using linear interpolation, and the intensity was uniformly adjusted to [0,1] using a normalisation method. The data format is designated as .pt, and each dataset comprises one original image and labelled annotations (the annotated regions correspond to the lumbar vertebrae L1-L5, intervertebral discs D1-D5, and sacrum S1).
# Data composition and download
The data has been structured in the following manner and is available for download as required.
|  | All | Train data |Vali data|Test data|
|-----|-----|-----|-----|-----|
| Quantity | 426 | 326 |50 |50 |
| Sex ratio(man) | 40% | 39% |38% |44% |
| Name | | Train.zip.001(2,3) |Vail.zip |Test.zip |
| Download | | [Train1](https://github.com/Ma-S-T/Spine-MSCA/raw/refs/heads/main/Train.zip.001),[Train2](https://github.com/Ma-S-T/Spine-MSCA/raw/refs/heads/main/Train.zip.002) ,[Train3](https://github.com/Ma-S-T/Spine-MSCA/raw/refs/heads/main/Train.zip.003)|[Vail](https://github.com/Ma-S-T/Spine-MSCA/raw/refs/heads/main/Vail.zip) |[Test](https://github.com/Ma-S-T/Spine-MSCA/raw/refs/heads/main/Test.zip) |
# Data description 
Each data point consists of img.pt and label.pt, as explained in detail below:
| Key | Dimension |Description|
|-----|-----|-----|
| img.pt | 512x512 | Raw Image |
| label.pt | 1x512x512 | Label Map |
# Label
The numerals 1-11 (with 0 serving as the background) are employed to denote distinct cone blocks, as explained in detail below:
| Label | Explanation | 
|-----|-----|
| 0 | background | 
| 1 | L1 | 
| 2 | L2 | 
| 3 | L3 | 
| 4 | L4 |
| 5 | L5 |
| 6 | S1 | 
| 7 | D1 | 
| 8 | D2 | 
| 9 | D3 | 
| 10 | D4 |
| 11 | D5 |
# Sample data
![图像](https://github.com/user-attachments/assets/e9cc199b-74b3-479e-afc6-850e94aebf3b)
![标签](https://github.com/user-attachments/assets/f0c17171-ee40-4124-ad68-1f77ec17a9c9)
# Usage
The installation of PyTorch is required, along with the utilisation of statements such as torch.load() for the purpose of viewing data attributes,and use statements such as plt.show() to generate image examples.
