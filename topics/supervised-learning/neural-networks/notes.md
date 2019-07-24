$$
% Display
\newcommand{\ds}{\displaystyle}
\newcommand{\ob}{\overbrace}
\newcommand{\ub}{\underbrace}
\newcommand{\code}{\texttt}

% Colours
\newcommand{\red}[1]{\textcolor{red}{#1}}
\newcommand{\redt}[1]{\textcolor{red}{\text{#1}}}
\newcommand{\blue}[1]{\textcolor{blue}{#1}}
\newcommand{\bluet}[1]{\textcolor{blue}{\text{#1}}}
\newcommand{\green}[1]{\textcolor{green}{#1}}
\newcommand{\greent}[1]{\textcolor{green}{\text{#1}}}

% Typefaces/Text-styles
\newcommand{\mc}{\mathcal}
\newcommand{\mf}{\mathfrak}
\newcommand{\b}{\mathbf}
\newcommand{\bs}{\boldsymbol}

% Fractions
\newcommand{\f}{\frac}

% Positioning
\newcommand{\l}{\left}
\newcommand{\m}{\middle}
\newcommand{\r}{\right}

% Logic
\newcommand{\n}{\not}
\newcommand{\eq}{\equiv}
\newcommand{\xor}{\oplus}

% Sets
\newcommand{\fa}{\forall}
\newcommand{\te}{\exists}
\newcommand{\empty}{\varnothing}
\newcommand{\set}[1]{\l\lbrace#1\r\rbrace}
\newcommand{\setb}[2]{\l\lbrace#1\ \m| \ #2\r\rbrace}
\newcommand{\bb}{\mathbb}
\newcommand{\R}{\bb{R}}
\newcommand{\N}{\bb{N}}
\newcommand{\Z}{\bb{Z}}
\newcommand{\Q}{\bb{Q}}
\newcommand{\C}{\bb{C}}

% Derivatives
\newcommand{\d}[1]{\mathrm{d}#1}
\newcommand{\deriv}[2]{\f{\d{#1}}{\d{#2}}}
\newcommand{\pderiv}[2]{\f{\partial #1}{\partial #2}}

% Sums/Integrals
\newcommand{\s}[3]{\sum_{#1}^{#2}#3}
\newcommand{\i}[4]{\int_{#1}^{#2}#3\ \d{#4}}

% Probability
\newcommand{\p}[1]{\bb{P}\l(#1\r)}
\newcommand{\cp}[2]{\p{#1\m|#2}}
\newcommand{\jp}[2]{\p{#1,#2}}
\newcommand{\e}[1]{\bb{E}\l[#1\r]}
\newcommand{\var}[1]{\text{Var}\l[#1\r]}
\newcommand{\sd}[1]{\text{SD}\l[#1\r]}
\newcommand{\cov}[2]{\text{Cov}\l[#1,#2\r]}

% Binomials
\newcommand{\ch}{\binom}
\newcommand{\pbin}[3][{}]{\l(#2 + #3\r)^#1}
\newcommand{\mbin}[3][{}]{\l(#2 - #3\r)^#1}

% Linear Algebra
\newcommand{\T}{\mathsf{T}}
\newcommand{\seq}[4][{}]{#2_{#3}#1 \ldots #1 #2_{#4}}
\newcommand{\rowv}[3]{\l(\seq[,]{#1}{#2}{#3}\r)}
\newcommand{\colv}[3]{\rowv{#1}{#2}{#3}^\T}
\newcommand{\sqpmat}[3][{}]{
    \begin{pmatrix}
		#2_{1{#1}1} & #2_{1{#1}2} & \cdots & #2_{1{#1}j} & \cdots & #2_{1{#1}#3} \\
		#2_{2{#1}1} & #2_{2{#1}2} & \cdots & #2_{2{#1}j} & \cdots & #2_{2{#1}#3} \\
		\vdots & \vdots & \ddots & \vdots & \ddots & \vdots \\
		#2_{i{#1}1} & #2_{i{#1}2} & \cdots & #2_{i{#1}j} & \cdots & #2_{i{#1}#3} \\
		\vdots & \vdots & \ddots & \vdots & \ddots & \vdots \\
		#2_{#3{#1}1} & #2_{#3{#1}2} & \cdots & #2_{#3{#1}j} & \cdots & #2_{#3{#1}#3} \\
	\end{pmatrix}
}
\newcommand{\sqmat}[3][{}]{
    \begin{matrix}
		#2_{1{#1}1} & #2_{1{#1}2} & \cdots & #2_{1{#1}j} & \cdots & #2_{1{#1}#3} \\
		#2_{2{#1}1} & #2_{2{#1}2} & \cdots & #2_{2{#1}j} & \cdots & #2_{2{#1}#3} \\
		\vdots & \vdots & \ddots & \vdots & \ddots & \vdots \\
		#2_{i{#1}1} & #2_{i{#1}2} & \cdots & #2_{i{#1}j} & \cdots & #2_{i{#1}#3} \\
		\vdots & \vdots & \ddots & \vdots & \ddots & \vdots \\
		#2_{#3{#1}1} & #2_{#3{#1}2} & \cdots & #2_{#3{#1}j} & \cdots & #2_{#3{#1}#3} \\
	\end{matrix}
}
\newcommand{\sqbmat}[3][{}]{
    \begin{bmatrix}
		#2_{1{#1}1} & #2_{1{#1}2} & \cdots & #2_{1{#1}j} & \cdots & #2_{1{#1}#3} \\
		#2_{2{#1}1} & #2_{2{#1}2} & \cdots & #2_{2{#1}j} & \cdots & #2_{2{#1}#3} \\
		\vdots & \vdots & \ddots & \vdots & \ddots & \vdots \\
		#2_{i{#1}1} & #2_{i{#1}2} & \cdots & #2_{i{#1}j} & \cdots & #2_{i{#1}#3} \\
		\vdots & \vdots & \ddots & \vdots & \ddots & \vdots \\
		#2_{#3{#1}1} & #2_{#3{#1}2} & \cdots & #2_{#3{#1}j} & \cdots & #2_{#3{#1}#3} \\
	\end{bmatrix}
}
\newcommand{\sqpmat}[3][{}]{
    \begin{pmatrix}
		#2_{1{#1}1} & #2_{1{#1}2} & \cdots & #2_{1{#1}j} & \cdots & #2_{1{#1}#3} \\
		#2_{2{#1}1} & #2_{2{#1}2} & \cdots & #2_{2{#1}j} & \cdots & #2_{2{#1}#3} \\
		\vdots & \vdots & \ddots & \vdots & \ddots & \vdots \\
		#2_{i{#1}1} & #2_{i{#1}2} & \cdots & #2_{i{#1}j} & \cdots & #2_{i{#1}#3} \\
		\vdots & \vdots & \ddots & \vdots & \ddots & \vdots \\
		#2_{#3{#1}1} & #2_{#3{#1}2} & \cdots & #2_{#3{#1}j} & \cdots & #2_{#3{#1}#3} \\
	\end{pmatrix}
}
\newcommand{\sqvmat}[3][{}]{
    \begin{vmatrix}
		#2_{1{#1}1} & #2_{1{#1}2} & \cdots & #2_{1{#1}j} & \cdots & #2_{1{#1}#3} \\
		#2_{2{#1}1} & #2_{2{#1}2} & \cdots & #2_{2{#1}j} & \cdots & #2_{2{#1}#3} \\
		\vdots & \vdots & \ddots & \vdots & \ddots & \vdots \\
		#2_{i{#1}1} & #2_{i{#1}2} & \cdots & #2_{i{#1}j} & \cdots & #2_{i{#1}#3} \\
		\vdots & \vdots & \ddots & \vdots & \ddots & \vdots \\
		#2_{#3{#1}1} & #2_{#3{#1}2} & \cdots & #2_{#3{#1}j} & \cdots & #2_{#3{#1}#3} \\
	\end{vmatrix}
}
\newcommand{\sqVmat}[3][{}]{
    \begin{Vmatrix}
		#2_{1{#1}1} & #2_{1{#1}2} & \cdots & #2_{1{#1}j} & \cdots & #2_{1{#1}#3} \\
		#2_{2{#1}1} & #2_{2{#1}2} & \cdots & #2_{2{#1}j} & \cdots & #2_{2{#1}#3} \\
		\vdots & \vdots & \ddots & \vdots & \ddots & \vdots \\
		#2_{i{#1}1} & #2_{i{#1}2} & \cdots & #2_{i{#1}j} & \cdots & #2_{i{#1}#3} \\
		\vdots & \vdots & \ddots & \vdots & \ddots & \vdots \\
		#2_{#3{#1}1} & #2_{#3{#1}2} & \cdots & #2_{#3{#1}j} & \cdots & #2_{#3{#1}#3} \\
	\end{Vmatrix}
}
$$

[TOC]

# Neural networks

**==Artificial neural networks==** are powerful and versatile machine learning systems that are perhaps the most commonly used learning method for many modern machine learning tasks.

Neural networks are often used for machine learning tasks where not much meaning or knowledge can be derived from the individual features of the training data. Instead, neural networks rely on a system of nodes called **neurons**, which are arranged in collections called **layers**, where the neurons in adjacent layers are connected. These connections have varied strengths, determined by a scalar referred to as a **weight**.

The purpose of the neurons on different layers is to learn the underlying (mostly non-linear) relationships between the original features and the output. Nevertheless, neural networks are often still treated as black boxes when compared to other machine learning models, since it isn't always straightforward to understand what the individual layers and neurons represent.

## Layers and neurons

A neural network may consist of many **layers**. Namely, there are three distinct types of layers:

- ==**Input layer**==: 

  - Consists of the features of the input vector $\b{x}^{(i)}$, or transformed feature vector $\bs{\phi}\l(\b{x}^{(i)}\r)$. This vector is also sometimes denoted as $\b{a}^{(1)}$ for consistency, as the notation $\b{a}^{(i)}$ in neural networks represents the output vector from the neurons in layer $i$, where indexing starts from $1$, with the input layer.
  - This layer **does not** pass the features through a weighted sum or activation function. The inputs are simply passed on to the next layer, with the corresponding weights $\bs{\theta}^{(1)}$ for this layer.
  - There may only be one input layer in a neural network.

- ==**Hidden layer**==:

  - Consists of **neurons**, each made up of two functions: a **weighted sum** and an **activation function**.

    <p style="text-align:center;">
    	<img src="./assets/neuron.png" width="70%"/>
    	<br>
    	<p style="text-align:center;">
        <b>Figure 1</b>: An artificial neuron (depicted in blue).
    	</p>
    </p>

    1. The **weighted sum** is computed from the inputs $\b{a}^{(i)}$, which are the outputs from the previous layer (along with their corresponding weights $\bs{\theta}^{(i)}$) . This is calculated as the dot product between these two vectors.
      
       Observe that this dot product may be an arbitrary real-valued number, depending on the weights—therefore, this result is passed through the activation function to transform it.
       
    2. The purpose of an **activation function** is to introduce non-linearity to a neural network—it transforms the value of the weighted sum and is chosen specifically for the type of task being performed.
    
       > **Example**: In the case of logistic regression, we saw that the logistic function $\sigma(x)=\frac{1}{1+e^{-x}}$ can be used to shrink $\R$ into the range $(0,1)$. This is an example of a commonly used activation function.
    
       <p style="text-align:center;">
           	<img src="./assets/logistic-sigmoid.png" width="35%"/>
       	<br>
           	<p style="text-align:center;">
           <b>Figure 2</b>: The logistic sigmoid activation function. (<a href="https://en.wikipedia.org/wiki/Sigmoid_function">source</a>)
           	</p>
           </p>
    
       There are many other activation functions which will be described later.
    
    - The output of one neuron is a **single value**, which is sent to each of the neurons on the next layer with new weights $\bs{\theta}^{(i+1)}$.
  
  - The outputs of the neurons in the final hidden layer are passed to the neurons in the **output layer**.
  
- ==**Output layer**==:

  - Functions the same way as a hidden layer—each output takes a weighted sum of its inputs and passes it through an activation function.
  - The number of output neurons is often the number of classes (in the case of a classification problem). However, in the case of binary classification, one output neuron is enough since we can represent the probability of the other class as the complement of the probability that is output by the neuron.

**Note**: When we say a neural network consists of $n$ layers, $n$ is the sum of hidden layers and the output layer.

## Activation functions

As explained previously, the purpose of an **==activation function==** is to introduce non-linearity to a neural network—it transforms the value of the weighted sum and is chosen specifically for the type of task being performed. Below is a list of some commonly used activation functions:

| **Name**                     |                         **Function**                         |                       **Plot**                        | **Comments**                                                 |
| ---------------------------- | :----------------------------------------------------------: | :---------------------------------------------------: | ------------------------------------------------------------ |
| Linear function              |                $\sigma_\text{Linear}(x;k)=kx$                | <img src="./assets/linear-plot.png" width="1000px"/>  |                                                              |
| Threshold (step) function    | $\sigma_\text{Step}(x;k)=\begin{cases}1& x\geq k\\ 0& x<k\end{cases}$ |  <img src="./assets/step-plot.png" width="1000px"/>   | <ul><li>Can be used to make a decision between binary classes $0$ and $1$, given a real-valued argument. For example, since $\sigma_\text{Logistic}$ yields a probability (where we would have to use $\arg\max$ to determine the class), we can determine the class by using $\sigma_\text{Step}(x;k=\frac{1}{2})$ in the output layer.</li></ul> |
| Logistic (sigmoid) function  |        $\sigma_\text{Logistic}(x)=\frac{1}{1+e^{-x}}$        | <img src="./assets/sigmoid-plot.png" width="1000px"/> | <ul><li>Typically used in the output layer of a neural network performing binary classification.</li><li>Suffers from the issue of vanishing gradients as $|x|$ increases.</li><li>Differentiable across entire domain.</li></ul> |
| Hyperbolic tangent function  |               $\sigma_\text{tanh}(x)=\tanh(x)$               |  <img src="./assets/tanh-plot.png" width="1000px"/>   | <ul><li>Can mathematically be represented as a shifted and scaled version of $\sigma_\text{Logistic}$ and is similarly used for binary classification tasks.</li><li>However, this cannot be directly used for negative log likelihood cost functions due to the function range being $(-1,1)$.</li><li>Suffers from the same vanishing gradient issue as $\sigma_\text{Logistic}$.</li></ul> |
| Rectified linear unit (ReLU) |              $\sigma_\text{ReLU}(x)=\max(0,x)$               |  <img src="./assets/relu-plot.png" width="1000px"/>   | ReLU is generally preferred to sigmoidal activation functions such as $\sigma_\text{Logistic}$ and $\sigma_\text{tanh}$ in deeper neural networks, mainly because:<ul><li> its simpler gradients (during backpropagation) allow for each layer to be trained quicker,</li><li>it does not suffer from the vanishing gradient problem.</li></ul> |

### Softmax function

Some special comments about softmax

## Multi-layer neural networks

A **==multi-layer neural network==** is a neural network that contains at least one hidden layer.

<p style="text-align:center;">
	<img src="./assets/multi-layer.png" width="90%"/>
	<br>
	<p style="text-align:center;">
    <b>Figure 3</b>: A multi-layer neural network consisting of one hidden layer with two neurons.
	</p>
</p>

As seen in *Figure 3*, each additional layer requires connections from the neurons in the layer to the neurons in the next layer, as well as the neurons in the previous layer. The connections between each layer depend on the outputs from the previous layer, and some weights for each neuron in the previous layer.

As a result, we require more structures and indexing to formally represent a neural network. Using *Figure 3* as an example:

- $\b{x}^{(i)}$ represents an arbitrary input feature vector with a bias term $x_0^{(i)}$.
  $$
  \b{x}^{(i)}=\colv{x^{(i)}}{0}{D}
  $$
  **Note**: $\b{x}^{(i)}$ is also treated as the first output—the output of the input layer, $\b{a}^{(1)}$.

- $\bs{\Theta}^{(i)}$ is the **weight matrix** representing the weights of the connections between the neurons in layer $i$ and the neurons in layer $i+1$.
  $$
  \begin{array}{c:ccccc}
  	\bs{\Theta}^{(i)} & \bs{\theta}_{0,\cdot}^{(i)} & \bs{\theta}_{1,\cdot}^{(i)} & \bs{\theta}_{2,\cdot}^{(i)} & \cdots & \bs{\theta}_{N_i,\cdot}^{(i)}\\
  	\hdashline
  	\blue{\bs{\theta}_{\cdot,1}^{(i)^\T}} & \theta_{0,1}^{(i)} & \theta_{1,1}^{(i)} & \theta_{2,1}^{(i)} & \cdots & \theta_{N_i,1}^{(i)}\\
  	\blue{\bs{\theta}_{\cdot,2}^{(i)^\T}} & \theta_{0,2}^{(i)} & \theta_{1,2}^{(i)} & \theta_{2,2}^{(i)} & \cdots & \theta_{N_i,2}^{(i)}\\
  	\vdots & \vdots & \vdots & \vdots & \ddots & \vdots\\
  	\blue{\bs{\theta}_{\cdot,N_{i+1}}^{(i)^\T}} & \theta_{0,N_{i+1}}^{(i)} & \theta_{1,N_{i+1}}^{(i)} & \theta_{2,N_{i+1}}^{(i)} & \cdots & \theta_{N_i,N_{i+1}}^{(i)}\\
  \end{array}
  $$

  > **Where**:
  >
  > - $N_i$ is the number of neurons in layer $i$.
  > - $\theta_{j,k}^{(i)}$ represents the weight from neuron $j$ in layer $i$, to neuron $k$ in layer $i+1$.
  > - $\bs{\theta}_{\cdot,k}^{(i)}=\l(\theta_{0,k}^{(i)},\ldots,\theta_{N_1,k}^{(i)}\r)^\T$ represents the weights from each neuron in layer $i$, to neuron $k$ in layer $i+1$.
  > - $\bs{\theta}_{j,\cdot}^{(i)}=\colv{\theta^{(i)}}{j,1}{j,N_{i+1}}$ represents the weights from neuron $j$ in layer $i$, to each neuron in layer $i+1$.

  Observe that there is no connection to the bias unit of the next layer—this bias unit is introduced independently and is not affected by the activations of the neurons from the previous layer. As a result, this weight matrix has dimensions:
  $$
  \dim(\bs{\Theta}^{(i)})=N_{i+1}\times (N_i+1)
  $$

- $\b{a}^{(i)}$ represents a vector consisting of the outputs from the neurons in layer $i$.
  $$
  \b{a}^{(i)}=\colv{a^{(i)}}{1}{N_i}
  $$

- $\b{n}^{(i)}$ represents the vector of neurons in layer $i$.
  $$
  \b{n}^{(i)}=\colv{n^{(i)}}{1}{N_i}
  $$

  > **Where**: Each neuron $n_j^{(i)}$ comprises an activation function $\sigma_j^{(i)}$ such that the output $a_j^{(i)}$ of this neuron is given by:
  > $$
  > a_j^{(i)}=\sigma_j^{(i)} \! \l(\bs{\theta}_{\cdot ,j}^{(i-1)}\b{a}^{(i-1)}\r)
  > $$
  > That is, the dot product between the weights from each neuron in layer $i-1$ to neuron $j$ in layer $i$, and the outputs of the neurons in the previous layer, applied to the activation function $\sigma_j^{(i)}$.
  >
  > However, it is usually the case that all of the sigmoid functions in one layer are the same—so we can just refer to this as $\sigma^{(i)}$.
  >
  > ---
  >
  > It is also possible to compute these activations all at once, using matrix multiplication of the weight matrix $\bs{\Theta}^{(i-1)}$ with the outputs of the previous layer, and a vector-valued activation function $\bs{\sigma}^{(i)}$:
  > $$
  > \begin{align}
  > 	\b{a}^{(i)}
  > 	&=\bs{\sigma}^{(i)} \! \l(\bs{\Theta}^{(i-1)}\b{a}^{(i-1)}\r)^\T\\
  > 	&=\bigg(
  > 		\underbrace{
  > 			\sigma^{(i)}\Big(\bs{\theta}_{\cdot,1}^{(i-1)}\b{a}^{i-1}\Big)
  > 		}_{a_1^{(i)}},
  > 		\ldots,
  > 		\underbrace{
  > 			\sigma^{(i)}\Big(\bs{\theta}_{\cdot,N_i}^{(i-1)}\b{a}^{i-1}\Big)
  > 		}_{a_{N_i}^{(i)}}
  > 	\bigg)^\T
  > \end{align}
  > $$

As an example of these forms of representation, the multi-layer neural network in *Figure 3* can be represented by the following matrices and vectors:
$$
\b{a}^{(1)}=\b{x}^{(i)}=\begin{pmatrix}
	x_0^{(i)} \\ x_1^{(i)} \\ x_2^{(i)} \\ x_3^{(i)} \\ x_4^{(i)}
\end{pmatrix},
\quad
\bs{\Theta}^{(1)}=\begin{pmatrix}
	\theta_{0,1}^{(1)} & \theta_{1,1}^{(1)} & \theta_{2,1}^{(1)} & \theta_{3,1}^{(1)} & \theta_{4,1}^{(1)} \\
	\theta_{0,2}^{(1)} & \theta_{1,2}^{(1)} & \theta_{2,2}^{(1)} & \theta_{3,2}^{(1)} &\theta_{4,2}^{(1)} \\
\end{pmatrix}
\\
\b{a}^{(2)}=\begin{pmatrix}
	a_0^{(2)} \\
	\sigma^{(2)} \Big(\bs{\theta}_{\cdot,1}^{(1)}\b{a}^{(1)}\Big) \\
	\sigma^{(2)} \Big(\bs{\theta}_{\cdot,2}^{(1)}\b{a}^{(1)}\Big)
\end{pmatrix},
\quad
\bs{\Theta}^{(2)}=\begin{pmatrix}
	\theta_{0,1}^{(2)} & \theta_{1,1}^{(2)} & \theta_{2,1}^{(2)} \\
	\theta_{0,2}^{(2)} & \theta_{1,2}^{(2)} & \theta_{2,2}^{(2)} \\
	\theta_{0,3}^{(2)} & \theta_{1,3}^{(2)} & \theta_{2,3}^{(2)} \\
\end{pmatrix}\\
\b{a}^{(3)}=\begin{pmatrix}
	\sigma^{(3)} \Big(\bs{\theta}_{\cdot,1}^{(2)}\b{a}^{(2)}\Big) \\
	\sigma^{(3)} \Big(\bs{\theta}_{\cdot,2}^{(2)}\b{a}^{(2)}\Big) \\
	\sigma^{(3)} \Big(\bs{\theta}_{\cdot,3}^{(2)}\b{a}^{(2)}\Big)
\end{pmatrix}
$$

### Training a multi-layer neural network

As with other machine learning algorithms such as linear and logistic regression, in order to train a neural network we need to find the weights that minimize some error function. However, this is more of a challenge in neural networks for three reasons:

1. There are far more weights to optimize—with one entire weight matrix $\bs{\Theta}^{(i)}$ between layers $i$ and $i+1$.

2. The change of a single weight connecting a neuron $n_j^{(i)}$ in layer $i$ to $n_k^{(i+1)}$ in layer $i+1$ will lead to all of the neurons in subsequent layers being affected due to propagation, as seen in *Figure 4* below.

   <p style="text-align:center;">
   	<img src="./assets/weight-modification.png" width="50%"/>
   	<br>
   	<p style="text-align:center;">
       <b>Figure 4</b>: The propagating effect of modifying one weight, on subsequent layers.
   	</p>
   </p>

3. The error functions used in neural networks are non-convex, meaning that optimization methods are not guaranteed to converge to a global minimum.

   Sometimes however, converging to a local minimum may be good enough and produce weights that the neural network can perform well with.

#### Error functions

The purpose of an **==error function==** is to evaluate the performance of the neural network when given some training examples. As neural networks are mostly commonly used in the supervised learning setting, we have access to the actual outputs of the training examples. 

The error function $C(\bs{\theta})$ is a measure of the inconsistency between the predicted outputs $\hat{y}^{(i)}$ and the actual outputs $y^{(i)}$ for a set of training examples. Therefore, a machine learning model's robustness and performance increases as the error function decreases. The optimal weights are thus the ones that minimize the error function $C(\bs{\theta})$:
$$
\hat{\bs{\theta}}=\arg\min_{\bs{\theta}} C(\bs{\theta})
$$
Neural networks may be used to predict the value of $y^{(i)}\in\R$ (like linear regression), $y^{(i)}\in\set{0,1}$ (binary classification), or $y^{(i)}\in\set{1,\ldots,K}$ (multi-class/multinomial classification). As a result, the error function used in a neural network must be chosen depending on the nature of the output variable.

##### Real-valued output $y^{(i)}\in\R$

Similarly to linear regression, the **residual sum of squares (RSS)** error function can be used for neural networks.
$$
\begin{align}
	C(\bs{\theta})
	&=\sum_{i=1}^N\l(y^{(i)}-\hat{y}^{(i)}\r)^2\\
	&=\sum_{i=1}^N\l(y^{(i)}-\bs{\theta}^\T\b{x}^{(i)}\r)^2
\end{align}
$$
However for the back-propagation training algorithm, it is normally preferable for the error function to be represented as a mean of the samples. For this reason, **==mean squared error (MSE)==** is used more often. Additionally, this quantity is scaled by $\frac{1}{2}$ to make derivatives cleaner:
$$
\begin{align}
	C(\bs{\theta})
	&=\frac{1}{2N}\sum_{i=1}^N\l(y^{(i)}-\hat{y}^{(i)}\r)^2\\
	&=\frac{1}{2N}\sum_{i=1}^N\l(y^{(i)}-\bs{\theta}^\T\b{x}^{(i)}\r)^2
\end{align}
$$

##### Binary output $y^{(i)}\in\set{0,1}$

As we have seen in logistic regression for binary classification, the output variable can be modeled by the Bernoulli distribution. As a result, the most appropriate cost function to use in this case was the **negative log-likelihood**. Minimizing this would yield the maximum likelihood estimate for the training data, $\hat{\bs{\theta}}$. 

For neural networks, we typically use **==cross entropy==**. Cross entropy is a measure of dissimilarity between two discrete probability distributions. As this is a binary classification problem, we have a Bernoulli-distributed output variable for each sample:
$$
\text{Output/Predicted:}\qquad \hat{y}^{(i)} \sim \mathrm{Bernoulli}\l(p_1^{(i)}\r)
$$

> **Where**: 
>
> - $p_1^{(i)}=\cp{\hat{y}^{(i)}=1}{\b{x}^{(i)};\bs{\theta}}=\sigma\l(\bs{\theta}^\T\b{x}^{(i)}\r)$ represents the probability of the output variable $\hat{y}^{(i)}$ taking the value $1$.<br/>**Note**: For binary classification, $p_0^{(i)}+p_1^{(i)}=1$ and therefore $p_0^{(i)}=1-p_1^{(i)}$.
> - $\hat{y}^{(i)}$ is a random variable representing the **predicted output** for the $i$^th^ training sample, $\b{x}^{(i)}$ such that $\hat{y}^{(i)}\in\set{p_0^{(i)},p_1^{(i)}}$.

In binary classification problems, we use an average of the per-example **binary cross entropies (BCE)** as the cost function:
$$
\begin{align}
C(\bs{\theta})
&=\frac{1}{N}\sum_{i=1}^N H\l(y^{(i)},\hat{y}^{(i)}\r)\\
&=-\frac{1}{N}\sum_{i=1}^N \l[\big(1-y^{(i)}\big) \log p_0^{(i)} + y^{(i)} \log p_1^{(i)}\r]\\
&=-\frac{1}{N}\sum_{i=1}^N \l[\big(1-y^{(i)}\big) \log \big(1-p_1^{(i)}\big) + y^{(i)} \log p_1^{(i)}\r]\\
\end{align}
$$

> **Where**:
>
> - $H(X,Y)$ is the cross entropy function which measures the dissimilarity between random variables $X$ and $Y$.
> - $y^{(i)}$ is a random variable representing the **true output** for the $i$^th^ training sample, $\b{x}^{(i)}$.<br/>**Note**: Unlike $\hat{y}^{(i)}$, the $y^{(i)}$ variable takes the value of the actual binary label since we don't have probabilities for the true outputs.

Observe that this is equivalent to taking the mean of the negative log likelihood function for the Bernoulli distribution:
$$
\begin{align}
	-\frac{1}{N}\mathcal{L}\l(\bs{\theta}; \b{y}\r)
	&=-\frac{1}{N} \log L\l(\bs{\theta}; \b{y}\r)\\
	&=-\frac{1}{N} \log \prod_{i=1}^N \l(1-p_1^{(i)}\r)^{1-y^{(i)}} \l(p_1^{(i)}\r)^{y^{(i)}}\\
	&=-\frac{1}{N} \sum_{i=1}^N \log \l[ \l(1-p_1^{(i)}\r)^{1-y^{(i)}} \l(p_1^{(i)}\r)^{y^{(i)}} \r]\\
	&=-\frac{1}{N} \sum_{i=1}^N \l[ \log\l(1-p_1^{(i)}\r)^{1-y^{(i)}} + \log\l(p_1^{(i)}\r)^{y^{(i)}} \r]\\
	&=-\frac{1}{N}\sum_{i=1}^N \l[ \l(1-y^{(i)}\r)\log\l(1-p_1^{(i)}\r) + y^{(i)}\log\l(p_1^{(i)}\r) \r]
\end{align}
$$

##### Multinomial output $y^{(i)}\in\set{1,\ldots,K}$

For multinomial classification problems, multinomial cross entropy is used as the error function for neural networks. This is a generalization of the previously seen binary cross entropy function, allowing for the use of the softmax function and multiple classes through **one-hot encoding**:
$$
\begin{align}
C(\bs{\Theta})=-\frac{1}{N}\sum_{i=1}^N\sum_{c=1}^K y_c^{(i)} \log p_c^{(i)}
\end{align}
$$

> **Where**:
>
> - $\bs{\Theta}$ is a matrix of weights, with each column representing the weight vector $\bs{\theta}^{(c)}$ for class $c$. Recall that in multinomial classification (as seen in the *Logistic Regression* notes), for each class $k$, we classify a feature vector $\b{x}^{(i)}$ as $k$ or not-$k$ through the use of the **softmax function**, which generates a probability for that class:
>   $$
>   \sigma_c\l(\b{x}^{(i)};\bs{\Theta}\r)=\frac{\exp\l({\bs{\theta}^{(c)\T}\b{x}^{(i)}}\r)}{\sum_{k=1}^K \exp\l({\bs{\theta}^{(k)\T}\b{x}^{(i)}}\r)}
>   $$
>   We assign $\b{x}^{(i)}$ to the class which had the highest probability.
>
> - $p_c^{(i)}=\cp{y^{(i)}=c}{\b{x}^{(i)};\bs{\Theta}}=\sigma_c\l(\b{x}^{(i)};\bs{\Theta}\r)$ represents the probability of feature vector $\b{x}^{(i)}$ being assigned to class $c$.
>
> - $\b{y}^{(i)}=\colv{y^{(i)}}{1}{K}$ is a **==one-hot encoded==** vector representing the actual class of the $i$^th^ training sample. For example, if we have data with $K=6$ classes, and training sample $\b{x}^{(i)}$ is assigned to class $4$, then $y_4^{(i)}$ is set to $1$, and the rest of the elements of $y^{(i)}$ are set to $0$, giving: $\b{y}^{(i)}=\l(0,0,0,1,0,0\r)^\T$. One-hot encoded vectors are frequently seen in machine learning as they allow for selective or conditional calculations, similar to indicator variables.

#### Using the error functions in backpropagation

As shown earlier in _Figure 4_, the modification of a single weight in any layer will have an effect on the output of the final layer. As a result, updating weights through gradient descent as we did in the _Logistic Regression_ notes, will not work in a neural network since we have multiple weight matrices.

Instead, the **==back-propagation==** algorithm is used to extend gradient descent to the context of hidden layers and neurons. The idea of back-propagation is to choose an appropriate cost function and then systematically and sequentially modify the weights of various neurons in order to minimize this cost function.

## Feedforward neural networks



# Resources

- _Charles Sutton, Nigel Goddard (School of Informatics, University of Edinburgh)_<br/>[Introductory Applied Machine Learning: Neural Networks - Training an ANN](https://www.learn.ed.ac.uk/bbcswebdav/pid-3412585-dt-content-rid-6699486_1/courses/INFR100692018-9SV1SEM1/Mlp9.pdf)
- _Hiroshi Shimodaira, Iain Murray, Steve Renals (School of Informatics, University of Edinburgh)_<br/>[Algorithms, Data Structures and Learning: Single Layer Neural Networks](https://www.inf.ed.ac.uk/teaching/courses/inf2b/learnSlides/inf2b-learnlec11-full.pdf)
- *Gordon Ross (School of Mathematics, University of Edinburgh)*<br/>[Statistical Learning: Neural Networks](http://www.drps.ed.ac.uk/19-20/dpt/cxmath10094.htm)
- _Sagar Sharma (Towards Data Science)_<br/>[The Fundamentals of Neural Networks: What the Hell is Perceptron?](https://towardsdatascience.com/what-the-hell-is-perceptron-626217814f53)
- _Rubio95R (Stack Exchange)_<br/>[Logistic Regression with Neural Network mindset vs. a shallow Neural Network](https://stats.stackexchange.com/questions/366707/a-logistic-regression-with-neural-network-mindset-vs-a-shallow-neural-network)
- _Rohan Varma_<br/>[Creating Neural Networks in Tensorflow](https://rohanvarma.me/Neural-Net-Tensorflow/)
- _cdeterman (Stack Exchange)_<br/>[Activation Function for First Layer Nodes in an ANN](https://stats.stackexchange.com/a/188452)
- _SimpliLearn_<br/>[Multilayer Artificial Neural Network](https://www.simplilearn.com/multilayer-artificial-neural-network-tutorial)
- _Sebastian Raschka_<br/>[Machine Learning FAQ: What is the relation between Logistic Regression and Neural Networks and when to use which?](https://sebastianraschka.com/faq/docs/logisticregr-neuralnet.html)
- _James Isaac (Medium)_<br/>[Understanding Deep Neural Networks from First Principles: Logistic Regression](https://medium.com/@melodious/understanding-deep-neural-networks-from-first-principles-logistic-regression-bd2f01c9e263)
- _Jiri Kriz (Nosco)_<br/>[Neural Networks: Forward Propagation](https://www.nosco.ch/ai/ml/nn_forward.php)
- _The Microsoft Cognitive Toolkit_<br/>[CNTK 103: Part B - Logistic Regression with MNIST](https://cntk.ai/pythondocs/CNTK_103B_MNIST_LogisticRegression.html)
- _GeeksForGeeks_<br/>[Activation functions in Neural Networks](https://www.geeksforgeeks.org/activation-functions-neural-networks/)
- _Pablo Ruiz (Towards Data Science)_<br/>[Neural Networks I: Notation and building blocks](https://towardsdatascience.com/neural-networks-i-notation-and-building-blocks-817b1d2ea04b)
- _Andrew Ng, Kian Katanforoosh (Computer Science Department, Stanford University)_<br/>[CS230: Deep Learning Representations](https://cs230.stanford.edu/files/Notation.pdf)
- _Alex S. Holehouse_<br/>[Neural Networks: Representation](http://www.holehouse.org/mlclass/08_Neural_Networks_Representation.html)
- _DeepAI_<br/>[Neural Network](https://deepai.org/machine-learning-glossary-and-terms/neural-network)
- _Wikipedia_<br/>[Activation function](https://en.wikipedia.org/wiki/Activation_function)
- _Jason Brownlee_<br/>[Why Training a Neural Network Is Hard](https://machinelearningmastery.com/why-training-a-neural-network-is-hard/)
- _ML4A (Machine Learning For Artists)_<br/>[How neural networks are trained](https://ml4a.github.io/ml4a/how_neural_networks_are_trained/)
- _Isaac Changhau_<br/>[Loss Functions in Neural Networks](https://isaacchanghau.github.io/post/loss_functions/)
- _Kevin P. Murphy_<br/>[Machine Learning: A Probabilistic Perspective](https://www.cs.ubc.ca/~murphyk/MLbook/)
- __<br/>[](https://blog.metaflow.fr/ml-notes-why-the-log-likelihood-24f7b6c40f83)

https://gluon.mxnet.io/chapter02_supervised-learning/logistic-regression-gluon.html

https://www.perfectlyrandom.org/2019/04/27/bernoulli-distribution-as-a-tiny-nn/

https://bigquant.com/community/t/topic/121439

http://wap.sciencenet.cn/blog-578676-1118819.html