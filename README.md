# Classificator-of-images-for-Music-A.I.
I spent my internship at L.I.N.K.S., a foundation born out of an 
agreement between Compagnia di San Paolo and the Politecnico di Torino, which specifically 
 deals with research in the field of artificial intelligence.
During this course, I studied deep learning, specifically convolutional neural networks. 
This was possible thanks to my participation in the 
Music A.I project, concerning an artificial intelligence that translates musical sentiment into images, specifically works of art. 
I, together with two of my fellow interns, had the task of 
develop an image classifier that would divide 'spurious' images 
i.e. images with certain characteristics ( a predominant colour for 
the whole image, the same texture throughout the image, absence of shapes, 
images consisting only of text, photography within the image), from the 
rest of the images ('non_spurious') so that the final model (Music 
A.I.) would not produce the former.
To do this we used a dataset of images:'wikiart' that contained within 
abstract and figurative works of art, but also some 'spurious' ones, so as to be able to 
divide the dataset into two classes (spurious, non_spurious) and be able to train
our model prototypes on them.
However, the classes were unbalanced, as the spurious were much less than the rest of the 
images and were not enough to achieve an 
effective training of the model, enabling it to recognise them. 
By searching for other examples of 'spurious' images on the net and applying techniques such as 
'augmentation' (which generates new examples by modifying and transforming the starting 
examples), we were able to obtain a balanced dataset.
Once the final dataset was obtained, we experimented with different configurations of a 
pre-trained convolutional neural network (resnet), and some methods of 
optimisation of the hyperparameters with the aim of obtaining the best 
configuration that would give us the best results.
After several attempts we found several configurations effective for the 
purpose, with a high precision in the detection of 'spurious' within an 
set of images.
