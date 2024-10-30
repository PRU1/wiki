neural networks use data from a single input value
and link that to an output 

but how can you find patterns in a sequence of data?

use a recurrent network
the output of a neuron can be reused as an input. you can repeat  same neural network on this output - but what happens to next input? 
## the language problem
the meaning of language is based on the sequence words are ordered in.
Feed forward networks assume "simultaneous access" meaning input -> output, and the order of the inputs does not influence the order of the output.
**recurrent neural networks** allow a model's decision to be based on words from the past
![[Pasted image 20240327053400.png]]

specialized to process a sequence of values $x^{(1)},...,x^{\tau}$. Most RNNs can process sequence of variable length

paramater sharing: extend and apply the model to examples of different lengths
- this essentially links inputs together
so if your input was "I went to Nepal in 2009" vs "In 2009, I went to Nepal", parameter sharing would create a link between going and 2009, and be able to extract the year 2009 if you ask the model to, whether it's the 2nd word or the 6th word

convolutions in a way, have parameter sharing: convolution is applied to a patch of data
parameter sharing works differently with RNNs
- each member of the output is a function of previous members of the input
![[Pasted image 20240327055456.png]]

the system can be described as: 
$$ s^{(t)}=f(s^{(t-1)};\pmb{\theta})$$
this says that the output of a neuron depends on shared parameters $\pmb\theta$ and the previous state $s^{t-1}$
![[Pasted image 20240327060149.png]]
it's a recursive function! you can unfold an RNN
![[Pasted image 20240327060452.png]]

NOTE: this is not Markovian because the output depends on all previous states, not just the most recent previous state.
![[Pasted image 20240327080039.png]]
The loop in RNNs are just unrolled neural networks
source code for an RNN: [Minimal character-level language model with a Vanilla Recurrent Neural Network, in Python/numpy (github.com)](https://gist.github.com/karpathy/d4dee566867f8291f086)

## RNNs as language models
language models let us assign conditional probability to every possible next word.
for example, if we had part of a sentence `I like`
you can assign a conditional probability that finds the likelihood of: `dogs` or `cats`
$P(\text{dog}\mid \text{I like})$
![[Pasted image 20240327071300.png]]

the loss function is calculated on the probability the network assigns the correct next word. use [[cross entropy loss]] (note to self, figure out what this is)
$$ L_{CE}(\hat{y_t},y_{t}) = -\log \hat{y}_t[w_{t+1}]$$

## Problems with RNN
- gradient EXPLODING and gradient vanishing
- use [[LSTM]]

in theory are good at finding "long term dependencies"
![[Pasted image 20240327080229.png]]

better way for NLP is [[generative pretrained transformer]]
