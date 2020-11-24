
<img src="https://i.ibb.co/3rHVxT6/resnet.png" width="500"><br><br>

**SUMMARY**<br>

This is an image identification task on Pytorch built with Resnet model and served with Flask/uWSGI server

The code for model was taken from the Pytorch [official tutorials](https://pytorch.org/tutorials/intermediate/flask_rest_api_tutorial.html)

Resnet is a network, where:


> "We explicitly reformulate the layers as learning residual functions with reference to the layer inputs, instead of learning unreferenced functions. We provide comprehensive empirical evidence showing that these residual networks are easier to optimize, and can gain accuracy from considerably increased depth. On the ImageNet dataset we evaluate residual nets with a depth of up to 152 layers---8x deeper than VGG nets but still having lower complexity. An ensemble of these residual nets achieves 3.57% error on the ImageNet test set. This result won the 1st place on the ILSVRC 2015 classification task. We also present analysis on CIFAR-10 with 100 and 1000 layers"

More details on this paper can be found [here](https://arxiv.org/abs/1512.03385)

<br/>
The Vue client code is not exposed since it's trivial

When installing Python dependencies, note that _torchvision_ is .8Gb, so better pull with _--no-cache-dir_ flag


***Flask-Pytorch setup***

```
cd your-folder

python3 -m venv env
source env/bin/activate

pip install --no-cache-dir  -r requirements.txt

```

