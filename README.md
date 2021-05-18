# Knowledge_Distillation
Platform used - Tensorflow <br>

Knowledge distillation is a process of training a smaller model using a larger model usually known as a teacher model.<br>
It has various benifits of Transfer learning as the model has lesser parameters than the original Parent (Teacher) model. <br>

There are various different hyperparameter used to train here  - <br>
1) Temperature - here the softmax function is modified for creating a type of prediction which not have a hard boundary, In the paper it is discussed that knowing the relation between other images in the dataset about how close the given image is from other classes is helpful. So this type of prediction is created by reducing the exponentiated value by a hyper parameter known as temperature. Its values shouldn't be soo high that the predicted values are very close and no conclusion can be drawn <br>
2) Alpha - This is the parameter which decided the weightage that needs to be given to the custom defined Loss function, how much weightage should be given to the loss recieved from the parent loss function and the student loss function.

Link for paper - https://arxiv.org/abs/1503.02531

The code is reffered from the official Keras documentation
