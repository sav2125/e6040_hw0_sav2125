# e6040_hw0_sav2125

HW0 assignment for ECBM 6040 Class

INSTRUCTIONS: It is recommended that you solve this homework using
a GPU instance on Amazon EC2. Instructions on how to use Amazon EC2
and Jupyter notebooks are available in this webpage. Information on how to
use Amazon EC2 will also be covered in Lecture #1.
If you have access to a fast GPU that supports CUDA, then you can also
use your own computer. You can find information on installing Theano here.
Make sure you install CUDA and cuDNN and enable GPU for Theano. If
you are not able to install GPU enabled Theano in a timely fashion, consider
using Amazon EC2 service with the provided machine image.
The submission for this homework should be a single Jupyter notebook file
called E6040 HW0.ipynb.
PROBLEM #1: In the notebook, execute the following examples in the
Deep Learning Tutorials with GPU support:
• code/logistic sgd.py
• code/convolutional mlp.py
Repeat the same using only CPU.
See this link for how to switch between using GPU and CPU. A suggested
way is to use command
%env THEANO FLAGS=d e vi c e=cpu
to configure the device right in the notebook. Notice that you need to restart
notebook kernel to load Theano with the new configuration (menu bar Kernel
→ Restart).
Save generated outputs using GPU and document any differences in execution
time when CPU is used. (If you do not want to wait until the end, you
can stop execution by using the menu bar Kernel → Interrupt. How many
training iterations has each example finished?)
PROBLEM #2: Read this tutorial (http://deeplearning.net/software/
theano/tutorial/examples.html) on how Theano defines functions, shared
variables and random numbers.
Perform the following operations in the notebook:
1. Create a Theano single precision floating point matrix X.
2. Create a RandomStream, and define a random stream of 10 × 10 matrices
A and a random stream of 10 × 1 vectors b, both from a normal
distribution.
3. Create a Theano function that performs (X + A)b, use a shared variable
in this function to record the randomly generated value of A and
another to record the value of b.
4. Evaluate the above function one time using a 10 × 10 numpy.ndarray
of your choice as input, and show that you can use the shared variables
to verify that the output of the function is correct.
Please save your code and the generated output in each step in the Jupyter
notebook.
