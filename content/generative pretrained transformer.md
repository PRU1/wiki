- bots that generate text
- model learned through a bunch of data
- "pre" means that it can be fine tuned
- Transformer: core invention in the boom of AI

trained to take in a piece of text, and produce a prediction for what comes next in the passage (probability distribution)

Split input into pieces of text called tokens
- for images or sound? little passages of image or sound
you associate the token as a vector
- words with similar meaning land on each other 

attention block: talk to eachother and pass information between them
	i.e. attention block figures out which words are relevent to other words
	![[Pasted image 20240401180600.png]]
	then run through MLP
	then put through Attention block
	hope is that meaning is baked into last vector in the list
		- generates probability distribution of next word 

Deep learning: a set of algorithms that scales very well for LOTS of input (i.e. 175billion)