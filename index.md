## Skin Hair Dataset 
Setting the benchmark for effective hair inpainting methods for improving the image quality of dermoscopic images


# Introduction
# Motivation 
One of the advantages of deep learning methods is the relative lack of preprocessing needed. In most computer vision tasks, including segmentation and classification which are mostly based on CNNs, datasets without any preparation or preprocessing are directly passed to the backbone of the CNN network in order to learn thefeatures. However, prior research indicates that, in the case of dermoscopic image analysis, most of the algorithms perform better when the artifacts are removed or inpainted.
The presence of hair in dermoscopic images poses a significant challenge as they may occlude some of the information of the lesion such as its boundary and texture.  Hence, the removal of hair is an important preprocessing step which, due to its diverse appearances, causes significant problems. We propose a dermoscopic image dataset which gives the possibility to work in the area of removing artifacts and can be used as a benchmark for researchers working on hair detection and inpainting. 
# Dataset Description
The dataset has been designed based on the ISIC dataset and consists of dermoscopic images with artificially added hairs as well as corresponding binary masks. We divide the dataset into two separate parts containing hair and without hair, respectively. Due to the very large variety and complexity of the hair patterns, we decided to transfer the hair from other dermoscopic images, which allowed us to maintain their natural appearance (Fig. 1). ????????The process of creating a dermoscopic image with hairs consists of the following steps: 1) Choosing a raw image without artifacts from the ISIC dataset, 2) Choosing an image including hairs from the ISIC dataset, 3) Manually marking the hair areas using Photoshop quick mask with alpha channel, soft, round brush with full opacity and size adapted to the size of the marked hair, 4) Cutting out the hair to a new transparent layer and clearing any additional areas of skin visible on this layer, 5) Applying the hair mask to the dermatoscopic image.?????
The extracted hair patterns have been augmented using the following methods: 1) randomly moving and rotating the mask, 2) modification of the selection with small, medium and large number of hairs; 3) changing the color of the hair into three main categories (light, brown, and dark) using brightness, contrast tool and color blending mode; 4) randomly applying different masks onto different clean images, without hair; and 5) for each modified pattern, a reference mask was created using a threshold tool.
In total, we used 77 non-hair images as the basis for applying different hair configurations. We augmented the extracted hair by changing the size, amount and colour. In total 252 images were generated with 84 unique masks to cover the different hair types. The Skin Hair dataset contains:
35 images with small density (each in three colours - light, brown and dark), 27 images with medium density (each in three colours - light, brown and dark) and 22 images with high density (each in three colours - light, brown and dark).


1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Skin-HairDataset/SHD/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
