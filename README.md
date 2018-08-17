# Hello World With Keras and Tensorflow

# References:

* [TensorFlow - An open source machine learning framework for everyone.](https://www.tensorflow.org);
* [Keras: The Python Deep Learning library](https://keras.io)

# Installation:

You need to have install python 3.0 or later, and create a virtual enviroment using **venv**.

	$ python3 -m venv <name_venv>

Then access your virtual enviroment

	$ source <name_venv>/bin/activate

Now install Keras from PyPI (recommended)

	$ pip3 install keras

Altermatively, install Keras from hte GitHub source:

	$ git clone https://github.com/keras-team/keras.git

Then ` cd ` to the Keras folder and run the install command:

	$ cd keras
	$ sudo python setup.py install


# Configure Keras:

If you have run Keras at least once, you will find the Keras configuration file at:

	$HOME/.keras/keras.json

If it isn't there, you can create it. The default configuration file looks like this:

	{
		"image_data_format": "channels_last",
		"epsilon": 1e-07,
    		"floatx": "float32",
    		"backend": "tensorflow"
	}

Simply change the field ` "backend" ` to ` "theano" `, ` "tensorflow" `, or ` "cntk" `, and Keras will use the new configuration next time you run any Keras code.

You can also define the environment variable ` KERAS_BACKEND ` and this will override what is defined in your config file:

	KERAS_BACKEND=tensorflow python -c "from keras import backend"
	Using TensorFlow backend.


# Using Keras:


