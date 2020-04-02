# iPanda-50
The iPanda-50 dataset is used for fine-grained panda identification.
This dataset can be obtained in the following ways:  
[BaiduNetDisk](https://pan.baidu.com/s/1YPI5KbAQK92gM7agvkWBpA)  
[GoolgelDrive](https://drive.google.com/open?id=1ZVAyyZzKbRcr_cjUe79wsSrhJ2y5DUbs) 

![ipand30](https://github.com/iPandaDateset/ipanda30/blob/master/ipanda30.png)

**Figure:** Sample images and statistics of the iPanda-50 dataset. Statistics are formatted as identity, #*images*  ( #*images-in-training*/#*images-in-testing* )

The iPanda-50 dataset consists of 6,874 images of 50 giant panda individuals with 49 ~ 292 images per panda identity.   
The directory structure of iPanda-50 is as follows:  

```

----|00_aibang  
    ----|00_v001_f000455.jpg  
    ----|00_v002_f000945.jpg  
    ----|......    
----|01_aoliao 
    ----|01_v002_f001680.jpg  
    ----|......  
    ----|...... 
----|... ...  
----|... ... 
----|... ... 
----|49_yuanrun
    ----|......  
 
```

There are 50 subfolders in the iPanda50.zip folder. Each subfolder represents a certain category. The file name of each subfolder shows the label and name of the panda. For example, "00_aibang" means that the panda name is "aibang" and the label is 0, thus the corresponding panda images of this category are stored in this subfolder.   



## iPanda-50 split

Initially, we randomly divide the iPanda-50 dataset into the training set and testing set via a 2:1 ratio.  Thus the training set contains 4,106 images and test set contains 2,768 images.  This division result was recorded in the split0/split0_train.txt and split0/split0_test.txt, respectively. 
Similarly, we totally divide the dataset into five independent subsets recorded in the "split" folder.

The directory structure of iPanda-50 split is as follows: 

----|split0  
    ----|split0_train.txt  
    ----|split0_test.txt   
----|split1 
    ----|split1_train.txt  
    ----|split1_test.txt  

----|split2  
    ----|split2_train.txt  
    ----|split2_test.txt  

----|split3  
    ----|split3_train.txt  
    ----|split3_test.txt  

----|split4  
    ----|split4_train.txt  
    ----|split4_test.txt  

