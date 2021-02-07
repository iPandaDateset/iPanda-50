# iPanda-50
The iPanda-50 dataset is used for fine-grained panda identification and it was proposed in [Le Wang, Rizhi Ding, Yuanhao Zhai, Qilin Zhang, Wei Tang, Nanning Zheng, and Gang Hua, “Giant Panda Identification”, IEEE Transactions on Image Processing, 2021.](https://doi.org/10.1109/tip.2021.3055627) In case you do not have convenient access to IEEE Xplore, the preprint PDF can be accessed [here from Github.io](https://qilin-zhang.github.io/_pages/pdfs/Giant_Panda_Identification_TIP.pdf) or [here from xjtu.edu.cn](http://gr.xjtu.edu.cn/documents/1809645/0/manuscript.pdf/47589606-3110-53de-eb0e-c7b4965940ad?t=1611713263900). If you find this dataset helpful in your research, please consider citing this publication. 
```
@ARTICLE{Wang21Giant,
  author={Le Wang and Rizhi Ding and Yuanhao Zhai and Qilin Zhang and Wei Tang and Nanning Zheng and Gang Hua},
  journal={IEEE Transactions on Image Processing}, 
  title={Giant Panda Identification}, 
  year={2021},
  doi={10.1109/TIP.2021.3055627},}
```
This dataset can be downloaded as a ZIP file from either one of the following links. Some filenames of the JPG images contain UTF-8 characters, please enable proper encoding while reading these files. A bug-fixing ZIP file is also provided to address the encoding issues. 

* [Baidu NetDisk Download Link 百度网盘下载链接](https://pan.baidu.com/s/1V2ghuy3Il6GFad7GFbE5MA) Extraction code 提取码: ``n07z`` File Size: 1.2GB 
Note: In this ZIP file, text files in its ``iPanda50-split`` folder contain [Windows Code page 936 (abbreviated MS936)](https://en.wikipedia.org/wiki/Code_page_936_\(Microsoft_Windows\)) encoded characters. They are highly likely to appear as cryptic glyphs (unreadable characters) on your computer. 
* [Google Drive Download Link](https://drive.google.com/open?id=1973u5DiS7NhlxURprJQ5fT6ItaqClnfJ) ``MD5 checksum: c71155875793276caafbee0faa4e7c0e`` File Size: 1.2GB 
Note: In this ZIP file, text files in its ``iPanda50-split`` folder contain [Windows Code page 936 (abbreviated MS936)](https://en.wikipedia.org/wiki/Code_page_936_\(Microsoft_Windows\)) encoded characters. They are highly likely to appear as cryptic glyphs (unreadable characters) on your computer. 
* [Bug fix of converting MS936-encoding to UTF-8, Google Drive Link]() ``MD5 checksum: ***`` File Size: MB. This ZIP file only contains the ``iPanda50-split`` folder. Please unzip it and overwrite previous ``iPanda50-split`` version. All text files here are encoded with UTF-8. 

![ipand50](https://github.com/iPandaDateset/iPanda-50/raw/master/iPanda50.png)

**Figure:** Sample images and statistics of the iPanda-50 dataset. Statistics are formatted as identity, #*images*  ( #*images-in-training*/#*images-in-testing* )

The iPanda-50 dataset consists of 6,874 images of 50 giant panda individuals with 49 ~ 292 images per panda.   
After you download the 'iPanda-50.zip' file, extract it into any directory.  You can see three folders, i.e., "iPanda50-images", "iPanda50-split", "iPanda-50-eyes-labels".

## iPanda50-images

All images are in the "iPanda50-images" folder, with the directory structure as follows.  

```
.
├── 00_aibang
├── 01_aoliao
├── 02_baolan
├── 03_bingdian
├── 04_chengdui
├── 05_chengjiu
├── 06_chengshi
├── 07_chengshuang
├── 08_fulai
├── 09_fushun
├── 10_hexing
├── 11_jiaoao
├── 12_jingjing
├── 13_jingliang
├── 14_maodou
├── 15_maosun
├── 16_maotao
├── 17_meibang
├── 18_miaomiao
├── 19_nannan
├── 20_nike
├── 21_nina
├── 22_nini
├── 23_qiubang
├── 24_qixi
├── 25_qiyi
├── 26_qiyuan
├── 27_rourou
├── 28_sa
├── 29_shuangxiong
├── 30_shuqing
├── 31_shurong
├── 32_susu
├── 33_wuyi
├── 34_xiaoqiao
├── 35_xilan
├── 36_xingda
├── 37_xinger
├── 38_xingfan
├── 39_xinghui
├── 40_xingrong
├── 41_xingxiao
├── 42_xingyi
├── 43_yaxing
├── 44_yayi
├── 45_yayun
├── 46_yazhu
├── 47_yingying
├── 48_yongbang
└── 49_yuanrun 
```

These 50 subfolders (00_aibang until 49_yuanrun) represent the numeric labels and names of these 50 giant panda individuals. For example, Panda #0 has the name "aibang" and Panda #49 has the name "yuanrun".   


## iPanda-50 split

We randomly divide the iPanda-50 dataset into the training split and the testing split at approximately 3:2 ratio, leading to a training set of 4,106 images and a test set of 2,768 images. This division operation was repeated for a total of 5 times (i.e., 5 Monte Carlo trials), and the results are saved in this ``iPanda50-split`` folder. 

The directory structure of ``iPanda50-split`` is as follows. 

```
.
├── split0_test.txt
├── split0_train.txt
├── split1_test.txt
├── split1_train.txt
├── split2_test.txt
├── split2_train.txt
├── split3_test.txt
├── split3_train.txt
├── split4_test.txt
└── split4_train.txt
```

## iPanda-50-eyes-labels

The area around eyes may contribute significantly to the identification of giant pandas, therefore we have provided additional eye annotations (i.e., location) in JSON format in the ``iPanda-50-eyes-labels`` folder. Only images with at least one eye visible are annotated. A total of 5,696 images are annotated in this folder. These JSON files are organized similar to the ``iPanda50-images`` folder, with each JSON file corresponding to an image with the same name.  
