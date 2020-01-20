# Image Captioning using Deep Learning
Image Captioning is the process of generating textual description of an image. It uses both **Natural Language Processing** and **Computer Vision** to generate the captions.
The generated output is expected to describe in a single sentence, what is shown in the image – the objects present, their properties, the actions being performed and the interaction between the objects, etc.

Image captioning is a combination of object recognition in an image and sequence prediction.To achieve image captioning a CNN **“Encoder”** (for feature extraction and object recognition) and a LSTM **“Decoder”** (for sequence prediction) are used.
- CNN converts the features of the image into a vector and this vector is passed as input to LSTM (Decoder).
- LSTM predicts the next word in the sentence by considering all the previous words in the sentence till t-1 time.

Network architecture is show in below diagram

<p align='center'>
  <img width="330" height="300" src = 'https://github.com/anand-kummari/image-captioning/blob/master/model.png?raw=true'>
</p>

## Dataset
### Flickr8k Dataset
- It conatains two folders, images and text.
- Text contains tokens.txt file in which for each image there  are five given descriptions.
- Each line in tokens.txt contains image id and image description.

## Results
- On below image the model outputs ***A white and black dog is running through the water***

<p align='center'>
  <img src = https://github.com/anand-kummari/image-captioning/blob/master/dog.jpg?raw=true>
</p>

- for below image, the model outputs ***man is skiing on snowy hill***

<p align='center'>
  <img src = https://github.com/anand-kummari/image-captioning/blob/master/ski.jpg?raw=true>
</p>
