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

![Alt text](./Good%20Caption/Bike.png?raw=true "Title")

![Alt text](./Good%20Caption/Skate.png?raw=true "Title")

![Alt text](./Good%20Caption/Skii.png?raw=true "Title")

![Alt text](./Good%20Caption/Sleeping.png?raw=true "Title")

![Alt text](./Good%20Caption/Surf.png?raw=true "Title")

![Alt text](./Good%20Caption/Veges.png?raw=true "Title")

Failed Captioning
--------------------------
**Not Even Close** 

![Alt text](./Failed%20Caption/Car.png?raw=true "Title")

**Wow, the algorithms is predicting the future. Heisenberg wears a hat** :laughing:

![Alt text](./Failed%20Caption/Heiseinberg.png?raw=true "Title")

**Not justice to the peaky blinders**

![Alt text](./Failed%20Caption/Peaky%20Blinders.png?raw=true "Title")

**What's going on rick??**

![Alt text](./Failed%20Caption/Rick%20and%20Morty.png?raw=true "Title")

**Totally nailed it**

![Alt text](./Failed%20Caption/Singing.png?raw=true "Title")


