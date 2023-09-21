### Wtf is that
**Image kernel** -> sth like filter, which is a small matrix applied to an entire image (blur filter)

### How to apply cernel to image
Among values between -1 and 1 it is possible to apply fitler with 0 and -1, where the values are corresponding 
then values are multipled by filter weights, sum result and output value

<br>
<a href="https://www.setosa.io/ev/image-kernels">sample image kernel fitler</a>


filters are reffered as convolution kernels
convolution -> process of passing them over to image

<u>during convultion borders are always lost! So pad can be implied (padding) so any border information is not lost</u>
not all neurons will be fully connected, instead neurons are only connected to a subset of local neurons in the next layer

Fo one filter there are localized_connections, so the network itself will figure is out. Then Second filter is applied
which will figure out how to connect it. 

for input image we assign 0 - 1 image matrix -> filter to scan image (or pad image) -> localize connections ->
for stride 2 we connect for certain subsets of neurons. It is up to neurons to connect each other.
This process is described as convolution layers.

COLOR OBJECTS can be described as 3D objects with RGB assignment.
**When You read in an image it will have (width, height, color_channels)**, where collor channels are values between 1

Convolution on a color image?
With 3D filter, there are 3 instances and for each instance many filters (so fitlers per color channel)
This allows to discover patterns between pattern


### Pooling Layer
pooling layers are used to reduce parameters
use max pooling, which takes biggest from 2x2 wiondow to pooling window with stride 2
this will remove 75% of input data

#### Dropout
form of regularization to prevent overfitting, units are randomly dropped along with their
connections

Both of this methods helps with co-adapting

CIFAR-10 sample colorful data