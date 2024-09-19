# Description

Neural Network training with **'DarkMark'**, **'Darknet'** based **'yolov4-tiny'** architecture with resources of **'OMiLab'** at the **'university of Vienna'**. Operating system is **'ubuntu'**. It has been defined 3 scenarios called Net1, Net2 and Net3 with different options to compare them at the end.
It also has been used server on computer in OMiLab with camera in this laboratory.

## Domain

Domain was Smart city objects. It has been used 6 default objects and 4 extra objects and in total 10 classes to train the network.

## Net1
We prepared the dataset in 10 classes with one white paper as a background.Pictures was in .png format. Then we labeled training data with DarkMark. DarkMark makes .json and .txt files automatically.
Data augmentation was next step. Then we opened 01_ccnAugmentation project in the Visual Studio Code. After adapting **conig.ini** Augmented images will be created. It is time to execute dataAaugmentation.py script. After that it is time to refresh DarkMark and creating DarkNet files and customizing the parameters according to scenarios.

In first scenario neutwork has been traind with this congifuration:

    * `batch_size` = 64
    * `sub_division` = 8
    * `max_batch` = 4000

Mosaic and flip left and right were the techniques used for augmentation.
Labeling data has been done with DarkMark. At the end of training it has been used 3 file extensions made by DarkNet to test: .names, .cnf, .weights .

It took **14 min** to train.

## Net2
We prepared the dataset in 10 classes with one white paper as a background.Pictures was in .png format. Then we labeled training data with DarkMark. DarkMark makes .json and .txt files automatically.
Data augmentation was next step. Then we opened 01_ccnAugmentation project in the Visual Studio Code. After adapting **conig.ini** Augmented images will be created. It is time to execute dataAaugmentation.py script. After that it is time to refresh DarkMark and creating DarkNet files and customizing the parameters according to scenarios.

In first scenario neutwork has been traind with this congifuration:

    * `batch_size` = 32
    * `sub_division` = 8
    * `max_batch` = 4000

Cutmix and flip left and right were the techniques used for augmentation.
Labeling data has been done with DarkMark. At the end of training it has been used 3 file extensions made by DarkNet to test: .names, .cnf, .weights .

It took **7.28** min to train.

## Net3
We prepared the dataset in 10 classes with one white paper as a background.Pictures was in .png format. Then we labeled training data with DarkMark. DarkMark makes .json and .txt files automatically.
Data augmentation was next step. Then we opened 01_ccnAugmentation project in the Visual Studio Code. After adapting **conig.ini** Augmented images will be created. It is time to execute dataAaugmentation.py script. After that it is time to refresh DarkMark and creating DarkNet files and customizing the parameters according to scenarios.

In first scenario neutwork has been traind with this congifuration:

    * `batch_size` = 128
    * `sub_division` = 8
    * `max_batch` = 4000

Random corp and image zoom and tile images were the techniques used for augmentation.
Labeling data has been done with DarkMark. At the end of training it has been used 3 file extensions made by DarkNet to test: .names, .cnf, .weights .

It took **26.09** min to train.
