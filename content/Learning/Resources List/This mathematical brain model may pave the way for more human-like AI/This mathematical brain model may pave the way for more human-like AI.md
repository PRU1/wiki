---
Link: https://thenextweb.com/news/mathematical-brain-model-human-like-ai
ee:
  - EE
---
![[image]]

Last week, Google Research held an online workshop on the conceptual understanding of deep learning. The workshop, which featured presentations by award-winning computer scientists and neuroscientists, discussed how new findings in [deep learning and neuroscience](https://bdtechtalks.com/2020/01/20/neuroscience-artificial-intelligence-synergies/) can help create better artificial intelligence systems.

While all the presentations and discussions were worth watching (and I might revisit them again in the coming weeks), one, in particular, stood out for me: A talk on word representations in the brain by Christos Papadimitriou, professor of computer science at the University of Columbia.

In his presentation, Papadimitriou, a recipient of the Gödel Prize and Knuth Prize, discussed how our growing understanding of information-processing mechanisms in the brain might help create algorithms that are more robust in understanding and engaging in conversations. Papadimitriou presented a simple and efficient model that explains how different areas of the brain inter-communicate to solve cognitive problems.

“What is happening now is perhaps one of the world’s greatest wonders,” Papadimitriou said, referring to how he was communicating with the audience. The brain translates structured knowledge into airwaves that are transferred across different mediums and reach the ears of the listener, where they are again processed and transformed into structured knowledge by the brain.

“There’s little doubt that all of this happens with spikes, neurons, and synapses. But how? This is a huge question,” Papadimitriou said. “I believe that we are going to have a much better idea of the details of how this happens over the next decade.”

![[tnw-newsletter.png]]

The <3 of EU tech

The latest rumblings from the EU tech scene, a story from our wise ol' founder Boris, and some questionable AI art. It's free, every week, in your inbox. Sign up now!

- I agree to allow TNW to store and process my personal data

## Assemblies of neurons in the brain

The cognitive and neuroscience communities are trying to make sense of how neural activity in the brain translates to language, mathematics, logic, reasoning, planning, and other functions. If scientists succeed at formulating the workings of the brain in terms of mathematical models, then they will open a new door to creating [artificial intelligence systems](https://bdtechtalks.com/2020/05/13/what-is-artificial-general-intelligence-agi/) that can emulate the human mind.

![[hqdefault.jpg]]

![[ytplaybtn.png]]

![[ytplaybtn-hover.png]]

A lot of studies focus on activities at the level of single neurons. Until a few decades ago, scientists thought that single neurons corresponded to single thoughts. The most popular example is the “[grandmother cell](https://en.wikipedia.org/wiki/Grandmother_cell)” theory, which claims there’s a single neuron in the brain that spikes every time you see your grandmother. More recent discoveries have refuted this claim and have proven that large groups of neurons are associated with each concept, and there might be overlaps between neurons that link to different concepts.

These groups of brain cells are called “assemblies,” which Papadimitriou describes as “a highly connected, stable set of neurons which represent something: a word, an idea, an object, etc.”

Award-winning neuroscientist György Buzsáki describes assemblies as “the alphabet of the brain.”

## A mathematical model of the brain

To better understand the role of assemblies, Papadimitriou proposes a mathematical model of the brain called “interacting recurrent nets.” Under this model, the brain is divided into a finite number of areas, each of which contains several million neurons. There is recursion within each area, which means the neurons interact with each other. And each of these areas has connections to several other areas. These inter-area connections can be excited or inhibited.

This model provides randomness, plasticity, and inhibition. Randomness means the neurons in each brain area are randomly connected. Also, different areas have random connections between them. Plasticity enables the connections between the neurons and areas to adjust through experience and training. And inhibition means that at any moment, a limited number of neurons are excited.

Papadimitriou describes this as a very simple mathematical model that is based on “the three main forces of life.”

![[brain-assemblies.jpg]]

Along with a group of scientists from different academic institutions, Papadimitriou detailed this model in a [paper](https://www.pnas.org/content/117/25/14464) published last year in the peer-reviewed scientific journal Proceedings of the National Academy of Sciences. Assemblies were the key component of the model and enabled what the scientists called “assembly calculus,” a set of operations that can enable the processing, storing, and retrieval of information.

“The operations are not just pulled out of thin air. I believe these operations are real,” Papadimitriou said. “We can prove mathematically and validate by simulations that these operations correspond to true behaviors… these operations correspond to behaviors that have been observed [in the brain].”

Papadimitriou and his colleagues hypothesize that assemblies and assembly calculus are the correct model that explain cognitive functions of the brain such as reasoning, planning, and language.

“Much of cognition could fit that,” Papadimitriou said in his talk at the Google deep learning conference.

## Natural language processing with assembly calculus

To test their model of the mind, Papadimitriou and his colleagues tried implementing a natural language processing system that uses assembly calculus to parse English sentences. In effect, they were trying to create an artificial intelligence system that simulates areas of the brain that house the assemblies that correspond to lexicon and language understanding.

![[assembly-calculus-natural-language-processing.jpg]]

“What happens is that if a sequence of words excites these assemblies in lex, this engine is going to produce a parse of the sentence,” Papadimitriou said.

The system works exclusively through simulated neuron spikes (as the brain does), and these spikes are caused by assembly calculus operations. The assemblies correspond to areas in the medial temporal lobe, Wernicke’s area, and Broca’s area, three parts of the brain that are highly engaged in language processing. The model receives a sequence of words and produces a syntax tree. And their experiments show that in terms of speed and frequency of neuron spikes, their model’s activity corresponds very closely to what happens in the brain.

The AI model is still very rudimentary and is missing many important parts of language, Papadimitriou acknowledges. The researchers are working on plans to fill the linguistic gaps that exist. But they believe that all these pieces can be added with assembly calculus, a hypothesis that will need to pass the test of time.

![[brain-areas-language-processing.jpg]]

“Can this be the neural basis of language? Are we all born with such a thing in [the left hemisphere of our brain],” Papadimitriou asked. There are still many questions about how language works in the human mind and how it relates to other cognitive functions. But Papadimitriou believes that the assembly model brings us closer to understanding these functions and answering the remaining questions.

Language parsing is just one way to test the assembly calculus theory. Papadimitriou and his collaborators are working on other applications, including learning and planning in the way that children do at a very young age.

“The hypothesis is that the assembly calculus—or something like it—fills the bill for access logic,” Papadimitriou said. “In other words, it is a useful abstraction of the way our brain does computation.”

_This article was originally published by Ben Dickson on_ [_TechTalks_](https://bdtechtalks.com/)_, a publication that examines trends in technology, how they affect the way we live and do business, and the problems they solve. But we also discuss the evil side of technology, the darker implications of new tech, and what we need to look out for. You can read the original article_ [_here_](https://bdtechtalks.com/2021/05/27/artificial-intelligence-neurons-assemblies/)_._

## Get the TNW newsletter

Get the most important tech news in your inbox each week.

- I agree to allow TNW to store and process my personal data
    

## Also tagged with