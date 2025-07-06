# Spine-MSCA
一个用于腰椎MRI图像分割的标注数据集，包含426名患者的**426**张腰椎T2矢状位MRI图像，使用线性插值方法统一将分辨率修改为512x512并使用归一化方法将强度统一调整到[0,1],数据格式为pt，每一个数据都包含一张原始图像和标注好的(标注区域为腰椎L1-L5、椎间盘D1-D5以及骶骨S1)标签。
# Download
下载所需数据
|  | All | Train data |Vali data|Test data|
|-----|-----|-----|-----|-----|
| Number | 426 | 326 |50 |50 |
| Sex ratio(man) | 40% | 39% |38% |44% |
|| | [Download]() |[Download]() |[Download]() |

# 标签
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
