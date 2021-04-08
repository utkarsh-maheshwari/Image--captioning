## Project Topic: Image captioning using RNN
### Team Name: Sleepy Heads

### Input
<img display="inline" style="width:500px;height:auto;" src="https://i.imgur.com/NziP9Wg.jpg"> 

### Output
<img display="inline" style="width:500px;height:auto;" src="https://i.imgur.com/pz9T4FU.jpg"> 


### Model download
```
wget https://doc-0k-bc-docs.googleusercontent.com/docs/securesc/ha0ro937gcuc7l7deffksulhg5h7mbp1/ugaptvtuqmpggkod3ofpbng8b5jsbnhf/1555293600000/15570688570768808365/*/1nMn__KLw8WMj_6SDRIH8AFfbaFX78mh7?e=download
Place it in models/model directory and rename it as model.npy
```

To run the model use : python main.py --phase=test --model_file='./models/model/model.npy'  --beam_size=3
Input files hould be kept in test/images


### Explaination:
 
We input an image and in the output we get the image with a caption describing the contents of the image. It works on a CNN for extracting features from the image using inceptionV3 and uses RNN for decoding these features into a sentence. 
This project is implemented on Tensorflow.
