[[Deriving transformers neural network]]
Secret behind ChatGPT
- uses Transformers

## Derivation of the Transformer
- based on a CNN
- invented in 2017
- after CNN breakthrough
- tried to put CNN to NLPs
	- analyzing text data
	- CNN were bad and unusable on text
Difference between text and images
- no numeric values
- one hot encoding
	- replace each word with a number encoding
reason for failure: CNN can't handle far away inputs
	solution: pair each word with every other word
		go through each permutation of the words
			ignores order of word
					solution: attach position to one hot encoding vector
	SO MANY PERMUTATIONS --> too computationally intensive
		- sum up vectors so that at max you compute $n^2$ inputs, where $n$ is the input size
		- give each vector an importance score, which details to pay attention to


- associate each token with a vector in high dimensional space
	- similar words are close to each other
	- embeddings
	- transformers goal is to embeddings right between words

## what is attention
![[Pasted image 20240415203027.png]]
- each token of mole has different meaning in the different cases
- attention block calculates what you need to add to move embedding in the right direction for the context
- single head of attention; attention block is multiple heads in parallel