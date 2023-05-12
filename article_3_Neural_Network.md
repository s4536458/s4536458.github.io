# Foundation of Neural Networks

## 1. Neural Network Concept

As discussed by [IBM](https://www.ibm.com/topics/neural-networks), neural networks are a fundamental component of deep learning models.

They consists of **node layers**. Each node is designated a certain weight and threshold. 

As shown below, the **input** layers are related to the **output** layers via multiple hidden layers:

<!----------- IMAGE ------------>
<img src="images/NEURAL_NETWORK.jpg">

From paper ["Using Deep Learning to Localize Gravitational Wave Sources"](https://www.researchgate.net/publication/335855384_Using_Deep_Learning_to_Localize_Gravitational_Wave_Sources/figures?lo=1)


## 2. Neural Model 
As shown in the above image, a neuron (node) is fed **inputs**. Additionally, 
each node has an inherent **weight** ($ w $). The multiplication of the input 
with its corresponding weight, plus the addition of a **bias** ($b$), yields 
an expression for the output of a neuron.

### *Output of a Neuron* 

   $$ O_{i,j} = x_{i,k} w_{k,j} + b_{j} $$

We can deduce from this equation, neuron output is inherently matrix multiplication. 

[from Fast AI Textbook - Chapter 17](https://nbviewer.org/github/fastai/fastbook/blob/master/17_foundations.ipynb)

## 3. Broadcasting
Tensors (matrices) will not always have the same rank. In a situation where two tensors in an operation do not have the same shape, broadcasting is used to make sure they are compatible with one another. 

There are several types of broadcasting: 

### 3.1 Broadcasting with a Scalar
Consider when an array and scalar are both involved in an operation.

    a = np.array([1, 2, 3])
    b = 2
    c = a * b

In this situation, broadcasting rules stipulate the scalar is **extended** into an array
of the same size as the matrix/array, as shown in the conceptual diagram below: 




### 3.2 Vector to Matrix


