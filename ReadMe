#Tensorflow update:0.12-->1.2
##Modofied work:
1)from tensorflow.contrib.slim.python.slim.nets.resnet_v1 import resnet_v1_block
Resnet Framwork: choose 'resnet_v1_block' ,nor resnet_utils

2)bboxes = tf.stop_gradient(tf.concat([y1, x1, y2, x2],1))  
Change the position of different axis

3)reshaped = tf.reshape(to_caffe,tf.concat(axis = 0,values = [[self._batch_size,num_dim,-1], [input_shape[2]]]))
or reshaped = tf.reshape(to_caffe,tf.concat(axis = 0,values = [[self._batch_size],[num_dim,-1], [input_shape[2]]]))
Definition: 'axis'  and 'values'

##Try to optimize:
1)image preprocessing (Opencv)
SRM Filter---substract the noise edge (core part)
gaussian filter
Gabor filter---great alternative for SRM filter.
2)different model frameworks.
