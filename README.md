# wine-quality
this is solution for wine quality prediction by using basic ML Model and LazyPredict
the general data prescription has the different chemical compositions of wine , which effect the wine qualiy
I came up with an approach which can help us understand data by forming our own class label by giving constraints to pH attribute
we are using pH attribute because as manu know pH scale is standardized scale to determine the nature of any chemical compound/mixture or element 
The constraints of the pH are as follows:
if pH is in the range 3.4 to 3.6 --> it is considered to be good wine
if the pH value is less than 3.4 --> it is considered to be moderate wine because of its good color and bitter taste
if the pH is greater than 3.6 --> it is considered to be bad wine 
we label encode the above attribute and obtain the class label 
for proving that this can model is accurate I have also done lazypredict for confirmation.
