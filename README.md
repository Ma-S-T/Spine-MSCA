# Spine-MSCA
The dataset is accompanied by a set of labels that indicate the regions of interest in the images. It contains a total of 426 lumbar T2 sagittal MRI images, each from a different patient. The resolution was uniformly adjusted to 512x512 using linear interpolation, and the intensity was uniformly adjusted to [0,1] using a normalisation method. The data format is designated as .pt, and each dataset comprises one original image and labelled annotations (the annotated regions correspond to the lumbar vertebrae L1-L5, intervertebral discs D1-D5, and sacrum S1).
# Data composition
数据的构成如下：
|  | All | Train data |Vali data|Test data|
|-----|-----|-----|-----|-----|
| Quantity | 426 | 326 |50 |50 |
| Sex ratio(man) | 40% | 39% |38% |44% |
| Name | | Train.zip.001(2,3) |Vail.zip |Test.zip |

# Data Description
每个数据由img.pt和label.pt组合而成，描述如下：
| Key | Dimension |Description|
|-----|-----|-----|
| img.pt | 512x512 | Raw Image |
| label.pt | 1x512x512 | Label Map |
# 标签
标签描述如下：
| label | 解释 | 
|-----|-----|
| 0 | 背景 | 
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
# 示例
![图像](https://github.com/user-attachments/assets/e9cc199b-74b3-479e-afc6-850e94aebf3b)
![标签](https://github.com/user-attachments/assets/f0c17171-ee40-4124-ad68-1f77ec17a9c9)
# 用法
安装**PyTorch**并使用torch.load()等语句查看数据属性，使用plt.show()等语句查看示例
