# lincolnbeet_dataset
The lincolnbeet dataset is an object detection dataset designed to encourage research in the identification of items in environments with high levels of occlusion, and in the development of better approaches to evaluate object detection models in practical scenarios. This dataset was introduced in the paper:

***"Self-supervised Representation Learning for Reliable Robotic Monitoring of Fruit Anomalies"***. Adrian Salazar-Gomez, Madeleine Darbyshire, Junfeng Gao, Elizabeth I Sklar, and Simon Parsons. 

You can find the paper on [[arXiv]](https://arxiv.org/abs/2109.11048). Currently, this work has been submitted to the IEEE for possible publication and the copyright may be transferred without notice, after which this version may no longer be accessible.


# Download link and dataset reference
The dataset contains 4402 images that contain weed plants and sugar beets which are located with object detection labels. The image size is 1920 x 1080 pixels, and the labels included in the dataset are in COCOjson, XML, and darknets formats. To download the dataset, please click on the following link.

https://www.dropbox.com/s/0rq7cc8t6rja632/all_fields_lincolnbeet.zip?dl=0

If you are using the dataset, please do not forget to cite it using the following bib entry:

```
@article{2021towards,
  title={Towards practical object detection for weed spraying in precision agriculture},
  author={Salazar-Gomez, Adrian and Darbyshire, Madeleine and Gao, Junfeng and Sklar, Elizabeth I and Parsons, Simon},
  journal={arXiv preprint arXiv:2109.11048},
  year={2021}
}
```

# How to use the dataset and dataset structure.
Once you have the .zip file that you got from the [[DATASET LINK]](https://www.dropbox.com/s/0rq7cc8t6rja632/all_fields_lincolnbeet.zip?dl=0), unzip the zip file to get a folder called "all_fields_lincolnbeet". The structure of the folder is as follows:


```

all_field_lincolnbeet                             #Dataset folder.
│
└───all                                          #Folder that contains the dataset images and the xml and darknet labels
│
|   └───.png
│   └───.txt files                              #Folder that contains the code to train and test the faster R CNN
|   └───.xml files                                 #This folder contains tools to train density-based models.
|       |   creation_density_maps.py              #Code to create the ground truth density maps.
|
└───all_fields_lincolnbeet_test_.json             #Folder where we save the datasets.
└───all_fields_lincolnbeet_train_.json            #Folder where we save the datasets.
└───all_fields_lincolnbeet_val_.json              #Folder where we save the datasets.
└───all_fields_lincolnbeet_test_.txt              #Folder where we save the datasets.
└───all_fields_lincolnbeet_train_.txt             #Folder where we save the datasets.
└───all_fields_lincolnbeet_val_.txt               #Folder where we save the datasets.
└───all_fields_lincolnbeet.json                   #Folder where we save the datasets.
└───json_test_set.json                            #Folder where we save the datasets.
└───json_test_set.json                            #Folder where we save the datasets.
└───json_test_set.json                            #Folder where we save the datasets.

```


# Characteristics of the dataset 
The lincolnbeet beet dataset is . The challenge

|                 |  Lincolnbeet | 
|---------------- | ------|
| **# of images** | 3,520 | 
| **Percentage**  | 100%  | 
| **Avg. WxH**    | 63x66 | 
| **Std. WxH**    | 18x23 |



And the characteristics of the items present in the dataset are:


|                 |  All items  |  Sugar beet  | weed |
|---------------- | ------|-------|--------|
| **# of images** | 3,520 | 462   | 2,406  | 
| **Percentage**  | 100%  | 13.1% | 68.4%  | 
| **Avg. WxH**    | 63x66 | 75x81 | 59x61  | 
| **Std. WxH**    | 18x23 | 18x22 | 17x22  |

Here is the basic statistics of the images included in Riseholme-2021, where WxH denotes the width x height of image. 
The severe *class imbalance* between normal and anomalous samples (95.7% vs 4.3%) simulates the *rare* occurrence of anomalous observation in realistic detection tasks. 


# Contact
If there is any questions about the dataset, please do not hesitate to drop an email to asalazargomez@lincoln.ac.uk.
