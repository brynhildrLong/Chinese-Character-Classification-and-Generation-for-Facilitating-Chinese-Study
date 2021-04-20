# Chinese-Character-Classification-and-Generation-for-Facilitating-Chinese-Study

### Abstract


With the increased usage of Chinese in various fields, more and more people are learning Chinese as a second language. However, there is no valid and accurate way to classify Chinese characters. In addition, understanding the evolution from oracle bone script, the predecessor of modern Chinese characters, to modern Chinese characters can also help in the learning and interpretation of oracle bones. In this project, we used Convolutional Neural Network to recognize and classify images of Chinese characters and were able to achieve 94% accuracy in the Duti/Heyi binary classification. In addition, we used various generative adversarial network models to compare the results of oracle script to simplified Chinese character transformation and finally found that CycleGANs are more advantageous in the transformation results. This project uses existing deep learning models to solve a new application problem and can contribute to the classification and style conversion of Chinese characters.<br>
<br>
<br>

### Code:


Firstly, code  **Chinese_image_crawl.py** could be used for images crawling from the webpage [dictionary](https://zd.hwxnet.com/).<br> <br>

The code is divided by name, and in the classification, the model for 2 class classification and 4 class classification is the same, i.e. 'CNN_classification_model.py'. <br> 
The code  **random_division.py** is used for dividing training and validation set randomly. The code  **n_average_division.py** is used for K-fold Cross-Validation and disrupts the order of the data set。 <br><br>

Using  **'DCGANs_Chinese.py'**  to implement the generation of simplified Chinese characters,  **'Pix2Pix_model.py'**  and  **'cyclegan_model.py '**  implement the oracle->Chinese character image style conversion. Note the path to replace the loaded image. <br>  <br>

The dataset of **'DCGANs_Chinese.py'** should be [Chinese characters only](https://drive.google.com/drive/folders/14Q3HB24dMEpazQ2-1H9n0T-YaEUgpTm7?usp=sharing). The dataset of **'Pix2Pix_model.py'** should be [Paired images](https://drive.google.com/drive/folders/1_oyGuPBBZwfnlU-O73zrJDVdtOOuPb17?usp=sharing). The dataset of **'cyclegan_model.py '** should be [Oracle Bone Characters](https://drive.google.com/drive/folders/14Q3HB24dMEpazQ2-1H9n0T-YaEUgpTm7?usp=sharing) and [Chinese characters only](https://drive.google.com/drive/folders/14Q3HB24dMEpazQ2-1H9n0T-YaEUgpTm7?usp=sharing).
<br>     
