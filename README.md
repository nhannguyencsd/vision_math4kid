# Math4Kid
In this project, I implement the conditional generative adversarial network to help kids learning various numbers from 0 to 9 as well as doing simple arithmetic operations such as addition, subtraction and multiplication.
<br/><br/>

## Condition GAN Architecture
#### High Level
![](static/depict/high_cgan.png#center)
#### Low Level
![](static/depict/low_cgan.png#center)
<br/><br/>

## How It Works
The generator of the conditional generative adversarial network takes a conditional input number from 0 to 9 and generates an image with that condition. Here are sample results that I ran for every condition from 0 to 9 at epoch 20th. </br>
![](static/depict/zeros.png)</br>
![](static/depict/ones.png) </br>
![](static/depict/twos.png) </br>
![](static/depict/threes.png) </br>
![](static/depict/fours.png) </br>
![](static/depict/fives.png) </br>
![](static/depict/sixs.png) </br>
![](static/depict/sevens.png) </br>
![](static/depict/eights.png) </br>
![](static/depict/nines.png) </br>
<br/>
After the generator knows how to generate a condition number image from 0 to 9, it generates two random conditional numbers(two operands) and performs the operation on those two operands along with a random operator. </br>
![](static/depict/first_answer.png#center) </br>
![](static/depict/second_answer.png#center) </br>
![](static/depict/third_answer.png#center) </br>
![](static/depict/fourth_answer.png#center)
<br/><br/>

## Technologies
- Python
- Pytorch
- Jupyter notebook
- Pillow
- Matplotlib
<br/><br/>

## Installation and Running
    $ git clone https://github.com/nhannguyencsd/vision_math4kid.git
    $ cd vision_math4kid
    $ python3 -m venv venv 
    $ source venv/bin/activate
    $ pip install -r static/libraries/requirements.txt
    $ jupyter notebook
* Once your jupyter notebook is opened, you can run a training_cgan.ipynb or math4kid.ipynb.</li>
* If you are not able to install libraries from requirements.txt or run on any notebooks, you are welcome [run](https://nhancs.com/project/3) the model on my website.
<br/><br/>

## Contributing
If you found any problems with this project, please let me know by opening an issue. Thanks in advance!
<br/><br/>

## License
This project is licensed under the MIT [License](LICENSE)
<br/><br/>

## References
The Conditional GAN paper: [https://arxiv.org/abs/1411.1784]https://arxiv.org/abs/1411.1784) <br/>
MNIST datasets: [http://yann.lecun.com/exdb/mnist/](http://yann.lecun.com/exdb/mnist/) <br/>
Convolutional GAN on MNIST: [https://github.com/rasbt/deeplearning-models/blob/master/pytorch_ipynb/gan/gan-conv.ipynb](https://github.com/rasbt/deeplearning-models/blob/master/pytorch_ipynb/gan/gan-conv.ipynb) <br/>
