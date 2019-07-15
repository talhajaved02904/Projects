Image Captioning 
=====================

This idea comes from recent advances in machine translation between languages, where a Recurrent Neural Network (RNN) transforms, say, a French sentence into a vector representation, and a second RNN uses that vector representation to generate a target sentence in German.

Now, what if we replaced that first RNN and its input words with a deep Convolutional Neural Network (CNN) trained to classify objects in images? Normally, the CNN’s last layer is used in a final Softmax among known classes of objects, assigning a probability that each object might be in the image. But if we remove that final layer, we can instead feed the CNN’s rich encoding of the image into a RNN designed to produce phrases. We can then train the whole system directly on images and their captions, so it maximizes the likelihood that descriptions it produces best match the training descriptions for each image.

![Alt text](./Description.png?raw=true "Title")
(Source: https://ai.googleblog.com/2014/11/a-picture-is-worth-thousand-coherent.html)

Results
------------

Good Captioning
-----------------------

![](Good%20Caption/Airplane.PNG?raw=true "Title")

![](./Good%20Caption/Baseball.PNG?raw=true "Title")

![](./Good%20Caption/Bike.PNG?raw=true "Title")

![](./Good%20Caption/Skate.PNG?raw=true "Title")

![](./Good%20Caption/Skii.PNG?raw=true "Title")

![](./Good%20Caption/Sleeping.PNG?raw=true "Title")

![](./Good%20Caption/Surf.PNG?raw=true "Title")

![](./Good%20Caption/Veges.PNG?raw=true "Title")

Failed Captioning
--------------------------
**Not Even Close** 

![](./Fail%20Caption/Car.PNG?raw=true "Title")

**Wow, the algorithm is predicting the future. Heisenberg wears a hat** :laughing:

![](./Fail%20Caption/Heiseinberg.PNG?raw=true "Title")

**Not justice to the peaky blinders**

![](./Fail%20Caption/Peaky%20Blinders.PNG?raw=true "Title")

**What's going on rick??**

![](./Fail%20Caption/Rick%20and%20Morty.PNG?raw=true "Title")

**Totally nailed it**

![](./Fail%20Caption/Singing.PNG?raw=true "Title")


