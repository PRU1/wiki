---
Link: https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full
ee:
  - EE
---
- 1Department of General Psychology, University of Padova, Padova, Italy
- 2Department of Information Engineering, University of Padova, Padova, Italy

As a full-blown research topic, numerical cognition is investigated by a variety of disciplines including cognitive science, developmental and educational psychology, linguistics, anthropology and, more recently, biology and neuroscience. However, despite the great progress achieved by such a broad and diversified scientific inquiry, we are still lacking a comprehensive theory that could explain how numerical concepts are learned by the human brain. In this perspective, I argue that computer simulation should have a primary role in filling this gap because it allows identifying the finer-grained computational mechanisms underlying complex behavior and cognition. Modeling efforts will be most effective if carried out at cross-disciplinary intersections, as attested by the recent success in simulating human cognition using techniques developed in the fields of artificial intelligence and machine learning. In this respect, deep learning models have provided valuable insights into our most basic quantification abilities, showing how numerosity perception could emerge in multi-layered neural networks that learn the statistical structure of their visual environment. Nevertheless, this modeling approach has not yet scaled to more sophisticated cognitive skills that are foundational to higher-level mathematical thinking, such as those involving the use of symbolic numbers and arithmetic principles. I will discuss promising directions to push deep learning into this uncharted territory. If successful, such endeavor would allow simulating the acquisition of numerical concepts in its full complexity, guiding empirical investigation on the richest soil and possibly offering far-reaching implications for educational practice.

## Introduction

Despite the importance of mathematics in modern societies, the cognitive foundations of mathematical learning are still mysterious and hotly debated. At the one end of the bridge, the idealistic view conceives mathematical concepts as purely abstract entities that humans discover using logical reasoning; at the other end, empiricists argue that mathematics is the product of our sensory experiences, and therefore it is essentially an activity of construction ([Brown, 2012](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B8)). A somehow intermediate position is taken by modern neurocognitive theories, which identify a set of “core” brain systems specifically evolved to support basic intuitions about quantity ([Butterworth, 1999](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B9); [Feigenson et al., 2004](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B27); [Piazza, 2010](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B62); [Dehaene, 2011](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B19)) but also acknowledge that higher-level numerical knowledge has materialized only recently, via cultural practices supported by language and symbolic reference ([Núñez, 2017](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B57)).

In recent years, the finding that measures of basic quantification skills correlate to later mathematical achievement (e.g., [Halberda et al., 2008](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B34); [Libertus et al., 2011](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B45); [Starr et al., 2013](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B77)) has led to the hypothesis that our “number sense” might indeed constitute the starting point to learn more complex mathematical concepts. However, the relationship between numerosity perception and symbolic math remains controversial ([Negen and Sarnecka, 2015](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B55); [Schneider et al., 2017](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B71); [Wilkey and Ansari, 2019](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B89)), calling for a deeper theoretical investigation that should be carried out with the support of formal models.

Here I will argue that the quest for artificial intelligence provides an extremely rich soil for the development of a computational theory of mathematical learning. Indeed, although computers largely outperform humans on numerical tasks requiring the mere application of syntactic manipulations (e.g., performing algebraic operations on large numbers, or iteratively computing the value of a function), they are completely blind about the _meaning_ of such operations because they lack a conceptual semantics of number. Grounding abstract symbols into some form of intrinsic meaning is a longstanding issue in artificial intelligence ([Searle, 1980](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B72); [Harnad, 1990](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B36)), and mathematics likely constitutes the most challenging domain for investigating how high-level knowledge could be linked to bottom-up, sensorimotor primitives ([Leibovich and Ansari, 2016](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B44)).

By framing a theory in computational terms, scientists are forced to adopt a precise, formal language, because all the details of the theory should be explicitly stated to simulate it on a computer. Modeling also requires to carefully think about the tasks that are being simulated and the possible ways in which a computational device can (or cannot) solve them. In this perspective article, I will focus in particular on _connectionist_ models, where cognition is conceived as an emergent property of networks of units that self-organize according to physical principles ([Rumelhart and McClelland, 1986](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B66); [Elman et al., 1996](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B25); [McClelland et al., 2010](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B49)). According to this view, knowledge is implicitly stored in the connections among neurons, and learning processes adaptively change the strength of these connections according to experience. Notably, the recent breakthroughs in _deep learning_ ([LeCun et al., 2015](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B43)) have revealed the true potential of this approach, by showing how machines endowed with domain-general learning mechanisms can simulate a variety of high-level cognitive skills, ranging from visual object recognition ([He et al., 2016](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B37)) to natural language understanding ([Devlin et al., 2018](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B21)) and strategic planning ([Silver et al., 2017](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B74)).

### Computational Models of Basic Quantification Skills

According to the “number sense” view, numerical cognition is grounded in basic quantification skills, such as the ability to rapidly estimate the number of items in a visual display ([Dehaene, 2011](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B19)). Numerosity is thus conceived as a primary perceptual attribute ([Anobile et al., 2016](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B3)) processed by a specialized (and possibly innate) system yielding an approximate representation of numerical quantity ([Feigenson et al., 2004](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B27)). The seminal neural network model by [Dehaene and Changeux (1993)](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B20) incorporated these principles: numerosity perception was hardwired in the model, reflecting the assumption that this ability is present at birth. Successive models revisited this nativist stance, by showing that numerosity representations can emerge as a result of learning and sensory experience ([Verguts and Fias, 2004](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B85)). In particular, recent work based on unsupervised deep learning has demonstrated that human-like numerosity perception can emerge in multi-layer neural networks that learn a hierarchical generative model of the sensory data ([Stoianov and Zorzi, 2012](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B78); [Zorzi and Testolin, 2018](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B93); see [Figure 1A](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#F1)).

FIGURE 1

**Figure 1**. Deep learning models. **(A)** Schematic representation of an unsupervised deep learning model that simulates human numerosity perception. Adapted from [Zorzi and Testolin (2018)](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B93). **(B)** Sketch of the proposed modeling framework, which extends the basic numerosity perception model (entirely confined within the agent’s brain) by introducing the ability to interact with the external environment to create and manipulate material representations.

Deep learning models account for a wide range of empirical phenomena in the number sense literature. They can accurately simulate Weber-like responses in numerosity comparison tasks ([Stoianov and Zorzi, 2012](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B78)), also accounting for congruency effects ([Zorzi and Testolin, 2018](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B93)) and for the fine-grained contribution of non-numerical magnitudes in biasing behavioral responses ([Testolin et al., 2019](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B81)). Notably, the number acuity of randomly initialized deep networks rivals that of newborns, and its gradual development follows trajectories similar to those observed in human longitudinal studies ([Testolin et al., 2020](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B83)). Deep networks have also been successfully tested in subitizing ([Wever and Runia, 2019](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B88)) and numerosity estimation tasks ([Chen et al., 2018](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B13)). Last, but not least, artificial neurons often reproduce neurophysiological properties observed in single-cell recording studies, for example by exhibiting number-sensitive tuning functions ([Zorzi and Testolin, 2018](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B93); [Nasr et al., 2019](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B54)).

Several questions remain under investigation: Is it possible to fully disentangle numerosity from continuous magnitudes by only relying on unsupervised learning ([Zanetti et al., 2019](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B91))? Can generative models generalize to unseen numerosities ([Zhao et al., 2018](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B92))? Are there computational limitations in tracking multiple objects in dynamic scenes ([Cenzato et al., 2019](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B12))? What is the contribution of explicit feedback and multi-sensory integration in shaping numerosity representations? How do deep learning models map into the cortical processing hierarchy? Nevertheless, despite these open questions, we can safely argue that deep learning has paved the way toward a computational theory about the origin of our number sense, confirming the appeal of deep networks as models of human sensory processing ([Testolin and Zorzi, 2016](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B80); [Yamins and DiCarlo, 2016](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B90); [Testolin et al., 2017](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B82)). Unfortunately, simulating the transition from approximate to symbolic numbers turns out to be much more challenging, as we discuss in the next section.

### Modeling the Acquisition of Higher-Level Mathematical Concepts

One of the most ambitious questions to be addressed is whether deep learning models could develop even more sophisticated numerical abilities, such as those involving arithmetic and symbolic math. Symbolic reasoning is notoriously difficult for connectionist models ([Marcus, 2003](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B47)), and despite recent progress, deep neural networks still struggle with tasks requiring procedural and compositional knowledge ([Garnelo and Shanahan, 2019](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B29)).

Only a few modeling studies have investigated how arithmetic could be learned by artificial neural networks. Since early attempts, associative memories have been used to simulate mental calculation as a process of storage and retrieval of arithmetic facts ([McCloskey and Lindemann, 1992](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B50)): during the learning phase, the two arguments and the result of a simple operation (e.g., single-digit multiplication) are given as input to an associative memory, whose learning goal is to accurately store them as a global, stable state. During the testing phase, only the operands are given, and the network must recover the missing information (i.e., the result) by gradually settling into the correct configuration. Building on this approach, successive simulations have shown that numerosity-based (“semantic”) representations can facilitate the learning of arithmetic facts ([Zorzi et al., 2005](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B94)) and equivalence problems ([Mickey and McClelland, 2014](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B53)). Others have shown that multi-digit addition and subtraction (but not multiplication) can be acquired through end-to-end supervised learning from pixel-level images ([Hoshen and Peleg, 2015](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B38)). One critical limitation of these approaches, however, is that they conceive arithmetic learning as a mere process of storing and recall, which gradually develops through the massive reiteration of all possible arithmetic facts that need to be learned. Besides being psychologically implausible and computationally unfeasible, this approach does not guarantee that the system will be able to generalize the acquired knowledge to unseen numbers and, even less, to exploit the acquired knowledge to more effectively learn new mathematical concepts.

The challenge of developing learning models that can exhibit algebraic generalization with the robustness and flexibility exhibited by humans is so fundamental that major players in deep learning research are intensively investigating these issues. For example, Google’s DeepMind company has recently evaluated several deep learning models on a set of benchmark problems taken from UK national school mathematics curriculums, covering arithmetic, algebra, elementary calculus, et cetera ([Saxton et al., 2019](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B69)). DeepMind’s best model correctly solved only 14 out of 40 problems, which would be equivalent to an “E” grade. Although such difficulties have led some researchers to argue that neural networks are incapable of exhibiting compositional abilities ([Marcus, 2018](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B46)), others argue for the opposite ([Baroni, 2020](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B4); [Martin and Baggio, 2020](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B48)).

Even the acquisition of the concept of _exact number_ is still out of reach for deep networks, which often cannot generalize outside of the range of numerical values encountered during training ([Trask et al., 2018](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B84)). Integer numbers are one of the pillars of arithmetic, so they constitute the perfect testbed for developing and testing computational models of mathematical learning. Developmental studies show that integers are gradually acquired by children during formal education through the acquisition of number words and counting skills: Indeed, although sequential (item-by-item) enumeration skills are present in animal species ([Platt and Johnson, 1971](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B63); [Beran and Beran, 2004](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B7); [Dacke and Srinivasan, 2008](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B16)), even in humans counting is not culturally universal ([Gordon, 2004](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B32)) and there is evidence that young children and people from cultures lacking number words have an incomplete understanding of what it means for two sets of items to have exactly the same number of items ([Izard et al., 2008](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B39), [2014](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B40)).

Some authors have sought to characterize the acquisition of exact numbers as the semantic induction of a “cardinality principle” ([Sarnecka and Carey, 2008](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B68)). This hypothesis has been exemplified in a computational model based on Bayesian inference, which simulated the stage-like development of counting abilities by relying on a pre-determined set of “core” cognitive operations ([Piantadosi et al., 2012](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B61)). The repertoire of innate abilities included the capacity to exactly identify cardinalities up to 3, perform basic operations on sets (e.g., difference, union, intersection), retrieve the next or previous word from an ordered counting list, and to operate these functions recursively. Although such modeling approach offers a rational interpretation of the process that might underly the acquisition of an abstract cardinality principle, it assumes a certain amount of _a priori_ symbolic knowledge and procedural skills, which is in contrast to empirical data suggesting, for example, that a complete understanding of the successor principle arises only after considerable interaction with the teaching environment ([Davidson et al., 2012](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B17)).

## Toward a Comprehensive Neurocomputational Framework

### The Downplayed Role of External Representations

A central tenet of connectionist models is that semantics intrinsically emerges in a system interacting with its surrounding environment. However, this idea is usually superficially implemented in deep learning models, because the interaction is often limited to _passive_ observation of statistical properties of the world ([Zorzi et al., 2013](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B95)). Taking inspiration from constructivist theories in developmental psychology, here I argue that a step forward will require to build computational models that learn by _actively_ manipulating the environment, that is, by causally interacting with objects in their perceptual space. Crucially, the notion of “environment” should include embodiment ([Lakoff and Núñez, 2000](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B41)) and—most importantly—the social, cultural and educational environment ([Vygotsky, 1980](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B86); [Clark, 2011](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B14)). Indeed, according to the Vygotskyan perspective, students actively construct abstract knowledge through interactions with teachers and peers, gradually moving their dependency on explicit forms of mediation to more implicit (internalized) forms ([Walshaw, 2017](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B87)).

The possibility to manipulate the environment greatly increases the complexity of the learning agent but also enables the functional use of external entities to create powerful representational systems, which can be manipulated in simple ways to get answers to difficult problems. The underlying assumption is that cultural evolution and history are foundational forces for the emergence of superior cognitive functions and that great intellectual achievements (such as the invention of mathematics) have been triggered by our ability to create artifacts serving as physical representations of abstract concepts. Some investigators have recently emphasized the role of material culture in numerical cognition ([Menary, 2015](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B51); [Overmann, 2016](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B58), [2018](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B59)), for example by highlighting that our mental organization of numbers into an ordered “number line” might be related to the linearity of the material forms used to represent and manipulate them ([Núñez, 2011](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B56)). Primitive devices used for representing numbers date back to notched bones in the Paleolithic period ([d’Errico et al., 2018](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B15)) and clay tokens in the Neolithic period ([Schmandt-Besserat, 1992](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B70)), which predated the subsequent diffusion of abaci, positional systems and increasingly more sophisticated numerical notations ([Menninger, 1992](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B52)). However, despite the concept of external representations was foreseen in early connectionist theories[1](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#note1), it has been seldomly explored in practice.

### Learning to Create and Manipulate Symbolic Representations

We can now sketch a concrete proposal for building more realistic simulations of mathematical learning. The computational framework should incorporate the following key components, summarized in [Figure 1B](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#F1).

- **Perceptual system**. This is where computational modeling has been mostly focused (and successful) up to now (see Section “Computational Models of Basic Quantification Skills”). The challenge will be to scale-up the existing models to more realistic sensory input (e.g., naturalistic visual scenes) and to incorporate a larger repertoire of pattern recognition abilities, which should not only allow to approximately represent visual quantities but also to recognize structured configurations of object arrays (e.g., sequences of tally marks, geometric displacements of items, patterns encoded in an abacus, etc.) and symbolic notations (e.g., written digits and operands).
- **Embodiment**. Of particular interest to the development of exact numbers is finger counting ([Butterworth, 1999](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B9); [Andres et al., 2007](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B2); [Domahs et al., 2012](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B23)), which not only helps children to keep track and coordinate the production of number words ([Alibali and DiRusso, 1999](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B1)) but may also allow to organize numbers spatially ([Fischer, 2008](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B28)). Hand-based representations are ubiquitous across cultures ([Bender and Beller, 2012](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B5)) and play a key role in the subsequent acquisition of number words ([Gunderson et al., 2015](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B33); [Gibson et al., 2019](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B31)), possibly influencing symbolic number processing even in adulthood ([Domahs et al., 2010](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B24)). It has been recently shown that neural networks can learn to count the number of items in visual displays and that the ability to sequentially point to individual objects helps in speeding up counting acquisition ([Fang et al., 2018](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B26)). A further step is taken by cognitive developmental robotics, which explores the instantiation of these principles in physically embodied agents ([Di Nuovo and Jay, 2019](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B22)). Interestingly, pointing gestures significantly improved counting accuracy in a humanoid robot, and learning was more effective when both fingers and words were provided as input ([Rucinski et al., 2012](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B65); [De La Cruz et al., 2014](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B18)).
- **Material representations**. The ability to manipulate external objects might be the key missing piece for simulating the acquisition of exact numbers. Indeed, although hand gestures might serve as placeholders to learn more efficient arithmetic strategies ([Siegler and Jenkins, 1989](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B73); for a computational account see [Hansen et al., 2014](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B35)), material representations allow for a much more precise encoding of numerical information. For example, the agent can learn to establish the cardinality of a set by organizing items in regular configurations that promote “groupitizing” ([Starkey and McCandliss, 2014](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B76)), or to exactly compare the cardinality of two sets by disposing of items in one-to-one correspondence. More sophisticated devices such as abaci and Cuisenaire rods further extend our ability to represent exact numbers, for example by exploiting inter-exponential relations to precisely (but compactly) encode large numbers, or to explicitly represent compositionality to promote generalization ([Overmann, 2018](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B59)).
- **Diversified learning signals**. In addition to unsupervised learning, the agent should exploit _reinforcement learning_ ([Sutton and Barto, 1998](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B79)) to predict the outcome of its actions. This learning modality would also play a key role in simulating curiosity-driven behavior and active engagement with material representations. Notably, deep reinforcement learning has recently achieved impressive performance in difficult cognitive tasks, for example by discovering complex strategies in board games ([Silver et al., 2017](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B74)). However, learning through reinforcement can be challenging in the presence of very large action spaces (i.e., the correct action has to be chosen from a wide range of possible actions) and sparse rewards (i.e., feedback is given only once the whole task has been carried out). Taking inspiration from the notions of _transfer learning_ and _curriculum learning_ used in machine learning ([Bengio et al., 2009](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B6)) and from _shaping_ procedures used in animal conditioning ([Skinner, 1953](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B75)), these issues can be mitigated by decomposing the task into simpler sub-tasks. For example, rather than rewarding only the trials where the agent has correctly counted all items in a display, rewards can be initially given every time the agent touches an object, to first promote the acquisition of sequential pointing skills. Similarly, the agent could first be rewarded simply for being able to accurately reproduce the abacus configuration corresponding to a specific number, rather than for being able to correctly manipulate the abacus to solve an addition problem. This idea of “gradually walking the agent through the word” also implies the exploitation of _supervised learning_, because explicit teaching signals must be used to stimulate learning by imitation and adult guidance.

**Linguistic input**. Despite language might not be crucial for the acquisition of elementary numerical concepts ([Gelman and Butterworth, 2005](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B30); [Butterworth et al., 2008](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B10)), it provides useful cues during the development of basic algebraic notions: for example, morphological cues allow single/plural distinction, number words can act as stable placeholders during counting acquisition, and learning natural language quantifiers seems a key step for mastering the ordering principle ([Le Corre, 2014](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B42)). A recent deep learning model has shown that learning quantifiers allows to more easily carry out approximate numerosity judgments ([Pezzelle et al., 2018](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B60)); however, the role of linguistic input for simulating the acquisition of exact numbers has yet to be explored. Furthermore, later in development language becomes the primary medium to acquire higher-level mathematical knowledge, hence it will need to be taken into account to design computational models approaching that level of complexity.

## Discussion

Symbolic numbers are a hallmark of human intelligence, but we are still lacking a comprehensive theory explaining how the brain learns to master them. Here I argued that computational modeling should have a primary role in this enterprise. Taking the acquisition of natural numbers as a case study, I emphasized the role of material representations in supporting the transition from approximate to symbolic numerical concepts. According to this view, exact numbers do not emerge from the mere association between number words and perceptual magnitudes: such mapping is strongly mediated by the acquisition of procedural skills (e.g., finger counting) and the ability to effectively manipulate representational devices ([Leibovich and Ansari, 2016](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B44); [Overmann, 2018](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B59); [Carey and Barner, 2019](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B11)).

In line with the idea that improved problem representation is a key mechanism for the joint development of conceptual and procedural knowledge ([Rittle-Johnson et al., 2001](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B64)), cognitive development in artificial agents must thus be supported by an adequate learning environment, which should provide feedback, teaching signals, and representational media commensurate with the current level of development. Notably, once a procedural skill has been mastered it might become internalized: the agent can simply “imagine” carrying out operations on the material device, without the need to physically operate over it. Some representations might thus serve just as intermediate steps for the acquisition of more abstract and efficient notations: as finger counting allows us to gradually grasp the meaning of number words, manipulating an abacus allows to ground numerical symbols into concrete visuospatial representations. A historical case that illustrates this perspective is the famous dispute between “abacists” and “algorists”, which was undoubtedly won by the latter, who demonstrated the superiority of symbolic notation for carrying out arithmetic operations (see [Figure 2](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#F2)). However, one might wonder whether Boethius could have mastered arithmetic algorithms without first grounding his numerical concepts into a set of more concrete representations.

FIGURE 2

**Figure 2**. Allegory of Arithmetic. Engraving from the encyclopedic book _Margarita Philosophica_ by Gregor Reisch (1503) depicting the “abacists vs. algorists” debate. Arithmetica (female figure) is supervising a calculation contest between Pythagoras (right), represented as using a counting board, and Boethius (left), who embraces algorithmic calculation with Arabic numbers. The struggle of Pythagoras suggests who is going to be the winner. Reproduced from Wikipedia.

In addition to providing a useful framework to interpret empirical findings, the proposed approach can raise important questions that would stimulate further theoretical and experimental work. For example, a critical aspect of our school system is to teach how to effectively discover useful strategies and representational schemes for solving difficult problems. In computational simulations, the necessity for appropriate teacher guidance stems from the fact that it is very difficult to invent new representations for problems we might wish to solve: it may even be that the process of inventing such representations is one of our highest intellectual abilities ([Rumelhart et al., 1986](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B67)). Computational frameworks that allow simulating a more complex interaction between artificial agents and their learning environment might thus eventually provide insights also about the teaching practices that could be most effective to guide numerical development in our children.

## Author Contributions

AT is fully responsible for the content of this article.

## Funding

This work was supported by the STARS grant “DEEPMATH” to AT from the University of Padova (Università degli Studi di Padova).

## Conflict of Interest

The author declares that the research was conducted in the absence of any commercial or financial relationships that could be construed as a potential conflict of interest.

## Acknowledgments

I am grateful to Jay McClelland for the useful discussions that stimulated many ideas elaborated in this article.

## Footnotes

1. [**^**](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#note1a) See for example, the section “External Representations and Formal Reasoning” in [Rumelhart et al. (1986)](https://www.frontiersin.org/articles/10.3389/fnhum.2020.00100/full#B67).

## References

Alibali, M. W., and DiRusso, A. A. (1999). The function of gesture in learning to count: more than keeping track. _Cogn. Dev._ 56, 37–56. doi: 10.1016/s0885-2014(99)80017-3

[CrossRef Full Text](https://doi.org/10.1016/s0885-2014(99)80017-3) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=The+function+of+gesture+in+learning+to+count%3A+more+than+keeping+track&author=Alibali+M.+W.&author=DiRusso+A.+A.&publication_year=1999&journal=Cogn.+Dev.&volume=56&pages=37-56)

Andres, M., Seron, X., and Olivier, E. (2007). Contribution of hand motor circuits to counting. _J. Cogn. Neurosci._ 19, 563–576. doi: 10.1162/jocn.2007.19.4.563

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=17381248) | [CrossRef Full Text](https://doi.org/10.1162/jocn.2007.19.4.563) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Contribution+of+hand+motor+circuits+to+counting&author=Andres+M.&author=Seron+X.&author=Olivier+E.&publication_year=2007&journal=J.+Cogn.+Neurosci.&volume=19&pages=563-576)

Anobile, G., Cicchini, G. M., and Burr, D. C. (2016). Number as a primary perceptual attribute: a review. _Perception_ 45, 5–31. doi: 10.1177/0301006615602599

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=26562858) | [CrossRef Full Text](https://doi.org/10.1177/0301006615602599) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Number+as+a+primary+perceptual+attribute%3A+a+review&author=Anobile+G.&author=Cicchini+G.+M.&author=Burr+D.+C.&publication_year=2016&journal=Perception&volume=45&pages=5-31)

Baroni, M. (2020). Linguistic generalization and compositionality in modern artificial neural networks. _Philos. Trans. R. Soc. B Biol. Sci._ 375:20190307. doi: 10.1098/rstb.2019.0307

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=31840578) | [CrossRef Full Text](https://doi.org/10.1098/rstb.2019.0307) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Linguistic+generalization+and+compositionality+in+modern+artificial+neural+networks&author=Baroni+M.&publication_year=2020&journal=Philos.+Trans.+R.+Soc.+B+Biol.+Sci.&volume=375&pages=20190307)

Bender, A., and Beller, S. (2012). Nature and culture of finger counting: diversity and representational effects of an embodied cognitive tool. _Cognition_ 124, 156–182. doi: 10.1016/j.cognition.2012.05.005

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=22695379) | [CrossRef Full Text](https://doi.org/10.1016/j.cognition.2012.05.005) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Nature+and+culture+of+finger+counting%3A+diversity+and+representational+effects+of+an+embodied+cognitive+tool&author=Bender+A.&author=Beller+S.&publication_year=2012&journal=Cognition&volume=124&pages=156-182)

Bengio, Y., Louradour, J., Collobert, R., and Weston, J. (2009). “Curriculum learning,” in _Proceedings of the 26th Annual International Conference on Machine Learning_ (New York, NY, USA: ACM), 1–8.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Curriculum+learning&author=Bengio+Y.&author=Louradour+J.&author=Collobert+R.&author=Weston+J.&conference=ACM&publication_year=2009)

Beran, M. J., and Beran, M. M. (2004). Chimpanzees remember the results of one-by-one addition of food items to sets over extended time periods. _Psychol. Sci._ 15, 94–99. doi: 10.1111/j.0963-7214.2004.01502004.x

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=14738515) | [CrossRef Full Text](https://doi.org/10.1111/j.0963-7214.2004.01502004.x) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Chimpanzees+remember+the+results+of+one-by-one+addition+of+food+items+to+sets+over+extended+time+periods&author=Beran+M.+J.&author=Beran+M.+M.&publication_year=2004&journal=Psychol.+Sci.&volume=15&pages=94-99)

Brown, J. R. (2012). _Platonism, Naturalism and Mathematical Knowledge._ New York, NY: Routledge.

Butterworth, B. (1999). _The Mathematical Brain._ London, UK: MacMillan.

Butterworth, B., Reeve, R., Reynolds, F., and Lloyd, D. (2008). Numerical thought with and without words: evidence from indigenous Australian children. _Proc. Natl. Acad. Sci. U S A_ 105, 13179–13184. doi: 10.1073/pnas.0806045105

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=18757729) | [CrossRef Full Text](https://doi.org/10.1073/pnas.0806045105) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Numerical+thought+with+and+without+words%3A+evidence+from+indigenous+Australian+children&author=Butterworth+B.&author=Reeve+R.&author=Reynolds+F.&author=Lloyd+D.&publication_year=2008&journal=Proc.+Natl.+Acad.+Sci.+U+S+A&volume=105&pages=13179-13184)

Carey, S., and Barner, D. (2019). Ontogenetic origins of human integer representations. _Trends Cogn. Sci._ 23, 823–835. doi: 10.1016/j.tics.2019.07.004

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=31439418) | [CrossRef Full Text](https://doi.org/10.1016/j.tics.2019.07.004) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Ontogenetic+origins+of+human+integer+representations&author=Carey+S.&author=Barner+D.&publication_year=2019&journal=Trends+Cogn.+Sci.&volume=23&pages=823-835)

Cenzato, A., Testolin, A., and Zorzi, M. (2019). On the difficulty of learning and predicting the long-term dynamics of bouncing objects. _arXiv:1907.13494_ [Preprint].

[Google Scholar](http://scholar.google.com/scholar_lookup?title=On+the+difficulty+of+learning+and+predicting+the+long-term+dynamics+of+bouncing+objects&author=Cenzato+A.&author=Testolin+A.&author=Zorzi+M.&publication_year=2019&journal=arXiv%3A1907.13494)

Chen, S. Y., Zhou, Z., Fang, M., and McClelland, J. L. (2018). “Can generic neural networks estimate numerosity like humans?,” in _Proceedings of the 40th Annual Conference of the Cognitive Science Society_, eds T. T. Rogers, M. Rau, X. Zhu and C. W. Kalish (Austin, TX: Cognitive Science Society), 202–207.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Can+generic+neural+networks+estimate+numerosity+like+humans%3F&author=Chen+S.+Y.&author=Zhou+Z.&author=Fang+M.&author=McClelland+J.+L.&publication_year=2018&pages=202-207)

Clark, A. (2011). _Supersizing the Mind: Embodiment, Action, and Cognitive Extension._ New York, NY: Oxford University Press.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Supersizing+the+Mind%3A+Embodiment,+Action,+and+Cognitive+Extension&author=Clark+A.&publication_year=2011)

d’Errico, F., Doyon, L., Colagé, I., Queffelec, A., Le Vraux, E., Giacobini, G., et al. (2018). From number sense to number symbols. An archaeological perspective. _Philos. Trans. R. Soc. B Biol. Sci._ 373:20160518. doi: 10.1098/rstb.2016.0518

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=29292345) | [CrossRef Full Text](https://doi.org/10.1098/rstb.2016.0518) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=From+number+sense+to+number+symbols.+An+archaeological+perspective&author=d%E2%80%99Errico+F.&author=Doyon+L.&author=Colag%C3%A9+I.&author=Queffelec+A.&author=Le+Vraux+E.&author=Giacobini+G.&+&publication_year=2018&journal=Philos.+Trans.+R.+Soc.+B+Biol.+Sci.&volume=373&pages=20160518)

Dacke, M., and Srinivasan, M. V. (2008). Evidence for counting in insects. _Anim. Cogn._ 11, 683–689. doi: 10.1007/s10071-008-0159-y

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=18504627) | [CrossRef Full Text](https://doi.org/10.1007/s10071-008-0159-y) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Evidence+for+counting+in+insects&author=Dacke+M.&author=Srinivasan+M.+V.&publication_year=2008&journal=Anim.+Cogn.&volume=11&pages=683-689)

Davidson, K., Eng, K., and Barner, D. (2012). Does learning to count involve a semantic induction? _Cognition_ 123, 162–173. doi: 10.1016/j.cognition.2011.12.013

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=22245033) | [CrossRef Full Text](https://doi.org/10.1016/j.cognition.2011.12.013) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Does+learning+to+count+involve+a+semantic+induction%3F&author=Davidson+K.&author=Eng+K.&author=Barner+D.&publication_year=2012&journal=Cognition&volume=123&pages=162-173)

De La Cruz, V. M., Di Nuovo, A., Di Nuovo, S., and Cangelosi, A. (2014). Making fingers and words count in a cognitive robot. _Front. Behav. Neurosci._ 8:13. doi: 10.3389/fnbeh.2014.00013

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=24550795) | [CrossRef Full Text](https://doi.org/10.3389/fnbeh.2014.00013) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Making+fingers+and+words+count+in+a+cognitive+robot&author=De+La+Cruz+V.+M.&author=Di+Nuovo+A.&author=Di+Nuovo+S.&author=Cangelosi+A.&publication_year=2014&journal=Front.+Behav.+Neurosci.&volume=8&pages=13)

Dehaene, S. (2011). _The Number Sense: How the Mind Creates Mathematics._ New York, NY: Oxford University Press.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=The+Number+Sense%3A+How+the+Mind+Creates+Mathematics&author=Dehaene+S.&publication_year=2011)

Dehaene, S., and Changeux, J.-P. J. (1993). Development of elementary numerical abilities: a neuronal model. _J. Cogn. Neurosci._ 5, 390–407. doi: 10.1162/jocn.1993.5.4.390

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=23964915) | [CrossRef Full Text](https://doi.org/10.1162/jocn.1993.5.4.390) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Development+of+elementary+numerical+abilities%3A+a+neuronal+model&author=Dehaene+S.&author=Changeux+J.-P.+J.&publication_year=1993&journal=J.+Cogn.+Neurosci.&volume=5&pages=390-407)

Devlin, J., Chang, M.-W., Lee, K., and Toutanova, K. (2018). BERT: pre-training of deep bidirectional transformers for language understanding. _arXiv:1810.04805_ [Preprint].

[Google Scholar](http://scholar.google.com/scholar_lookup?title=BERT%3A+pre-training+of+deep+bidirectional+transformers+for+language+understanding&author=Devlin+J.&author=Chang+M.-W.&author=Lee+K.&author=Toutanova+K.&publication_year=2018&journal=arXiv%3A1810.04805)

Di Nuovo, A., and Jay, T. (2019). Development of numerical cognition in children and artificial systems: a review of the current knowledge and proposals for multi-disciplinary research. _Cogn. Comput. Syst._ 1, 2–11. doi: 10.1049/ccs.2018.0004

[CrossRef Full Text](https://doi.org/10.1049/ccs.2018.0004) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Development+of+numerical+cognition+in+children+and+artificial+systems%3A+a+review+of+the+current+knowledge+and+proposals+for+multi-disciplinary+research&author=Di+Nuovo+A.&author=Jay+T.&publication_year=2019&journal=Cogn.+Comput.+Syst.&volume=1&pages=2-11)

Domahs, F., Kaufmann, L., and Fischer, M. H. (2012). _Handy Numbers: Finger Counting and Numerical Cognition._ Lausanne: Special Research Topic in Frontiers Media SA.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Handy+Numbers%3A+Finger+Counting+and+Numerical+Cognition&author=Domahs+F.&author=Kaufmann+L.&author=Fischer+M.+H.&publication_year=2012)

Domahs, F., Moeller, K., Huber, S., Willmes, K., and Nuerk, H.-C. (2010). Embodied numerosity: implicit hand-based representations influence symbolic number processing across cultures. _Cognition_ 116, 251–266. doi: 10.1016/j.cognition.2010.05.007

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=20513381) | [CrossRef Full Text](https://doi.org/10.1016/j.cognition.2010.05.007) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Embodied+numerosity%3A+implicit+hand-based+representations+influence+symbolic+number+processing+across+cultures&author=Domahs+F.&author=Moeller+K.&author=Huber+S.&author=Willmes+K.&author=Nuerk+H.-C.&publication_year=2010&journal=Cognition&volume=116&pages=251-266)

Elman, J. L., Bates, E., Johnson, M., Karmiloff-smith, A., Parisi, D., and Plunkett, K. (1996). _Rethinking Innateness: A Connectionist Perspective on Development._ Cambridge, MA: MIT Press.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Rethinking+Innateness%3A+A+Connectionist+Perspective+on+Development&author=Elman+J.+L.&author=Bates+E.&author=Johnson+M.&author=Karmiloff-smith+A.&author=Parisi+D.&author=Plunkett+K.&publication_year=1996)

Fang, M., Zhou, Z., Chen, S. Y., and McClelland, J. L. (2018). “Can a recurrent neural network learn to count things?” in _Proceedings of the 40th Annual Conference of the Cognitive Science Society_, eds T. T. Rogers, M. Rau, X. Zhu, and C. W. Kalish (Austin, TX: Cognitive Science Society), 360–365.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Can+a+recurrent+neural+network+learn+to+count+things%3F&author=Fang+M.&author=Zhou+Z.&author=Chen+S.+Y.&author=McClelland+J.+L.&conference=&publication_year=2018)

Feigenson, L., Dehaene, S., and Spelke, E. S. (2004). Core systems of number. _Trends Cogn. Sci._ 8, 307–314. doi: 10.1016/j.tics.2004.05.002

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=15242690) | [CrossRef Full Text](https://doi.org/10.1016/j.tics.2004.05.002) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Core+systems+of+number&author=Feigenson+L.&author=Dehaene+S.&author=Spelke+E.+S.&publication_year=2004&journal=Trends+Cogn.+Sci.&volume=8&pages=307-314)

Fischer, M. H. (2008). Finger counting habits modulate spatial-numerical associations. _Cortex_ 44, 386–392. doi: 10.1016/j.cortex.2007.08.004

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=18387569) | [CrossRef Full Text](https://doi.org/10.1016/j.cortex.2007.08.004) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Finger+counting+habits+modulate+spatial-numerical+associations&author=Fischer+M.+H.&publication_year=2008&journal=Cortex&volume=44&pages=386-392)

Garnelo, M., and Shanahan, M. (2019). Reconciling deep learning with symbolic artificial intelligence: representing objects and relations. _Curr. Opin. Behav. Sci._ 29, 17–23. doi: 10.1016/j.cobeha.2018.12.010

[CrossRef Full Text](https://doi.org/10.1016/j.cobeha.2018.12.010) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Reconciling+deep+learning+with+symbolic+artificial+intelligence%3A+representing+objects+and+relations&author=Garnelo+M.&author=Shanahan+M.&publication_year=2019&journal=Curr.+Opin.+Behav.+Sci.&volume=29&pages=17-23)

Gelman, R., and Butterworth, B. (2005). Number and language: how are they related? _Trends Cogn. Sci._ 9, 6–10. doi: 10.1016/j.tics.2004.11.004

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=15639434) | [CrossRef Full Text](https://doi.org/10.1016/j.tics.2004.11.004) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Number+and+language%3A+how+are+they+related%3F&author=Gelman+R.&author=Butterworth+B.&publication_year=2005&journal=Trends+Cogn.+Sci.&volume=9&pages=6-10)

Gibson, D. J., Gunderson, E. A., Spaepen, E., Levine, S. C., and Goldin-Meadow, S. (2019). Number gestures predict learning of number words. _Dev. Sci._ 22:e12791. doi: 10.1111/desc.12791

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=30566755) | [CrossRef Full Text](https://doi.org/10.1111/desc.12791) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Number+gestures+predict+learning+of+number+words&author=Gibson+D.+J.&author=Gunderson+E.+A.&author=Spaepen+E.&author=Levine+S.+C.&author=Goldin-Meadow+S.&publication_year=2019&journal=Dev.+Sci.&volume=22&pages=e12791)

Gordon, P. (2004). Numerical cognition without words: evidence from amazonia. _Science_ 306, 496–499. doi: 10.1126/science.1094492

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=15319490) | [CrossRef Full Text](https://doi.org/10.1126/science.1094492) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Numerical+cognition+without+words%3A+evidence+from+amazonia&author=Gordon+P.&publication_year=2004&journal=Science&volume=306&pages=496-499)

Gunderson, E. A., Spaepen, E., Gibson, D., Goldin-Meadow, S., and Levine, S. C. (2015). Gesture as a window onto children’s number knowledge. _Cognition_ 144, 14–28. doi: 10.1016/j.cognition.2015.07.008

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=26210644) | [CrossRef Full Text](https://doi.org/10.1016/j.cognition.2015.07.008) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Gesture+as+a+window+onto+children%27s+number+knowledge&author=Gunderson+E.+A.&author=Spaepen+E.&author=Gibson+D.&author=Goldin-Meadow+S.&author=Levine+S.+C.&publication_year=2015&journal=Cognition&volume=144&pages=14-28)

Halberda, J., Mazzocco, M. M., and Feigenson, L. (2008). Individual differences in non-verbal number acuity correlate with maths achievement. _Nature_ 455, 665–668. doi: 10.1038/nature07246

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=18776888) | [CrossRef Full Text](https://doi.org/10.1038/nature07246) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Individual+differences+in+non-verbal+number+acuity+correlate+with+maths+achievement&author=Halberda+J.&author=Mazzocco+M.+M.&author=Feigenson+L.&publication_year=2008&journal=Nature&volume=455&pages=665-668)

Hansen, S. S., McKenzie, C., and McClelland, J. L. (2014). “Two plus three is five: discovering efficient addition strategies without metacognition,” in _Proceedings of the 36th Annual Conference of the Cognitive Science Society_ (Montreal, QC: Cognitive Science Society), 583–588.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Two+plus+three+is+five%3A+discovering+efficient+addition+strategies+without+metacognition&author=Hansen+S.+S.&author=McKenzie+C.&author=McClelland+J.+L.&conference=&publication_year=2014)

Harnad, S. (1990). The symbol grounding problem. _Phys. D Nonlinar Phenom._ 42, 335–346. doi: 10.1016/0167-2789(90)90087-6

[CrossRef Full Text](https://doi.org/10.1016/0167-2789(90)90087-6) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=The+symbol+grounding+problem&author=Harnad+S.&publication_year=1990&journal=Phys.+D+Nonlinar+Phenom.&volume=42&pages=335-346)

He, K., Zhang, X., Ren, S., and Sun, J. (2016). “Deep residual learning for image recognition,” in _Proceedings of the 2016 IEEE Conference on Computer Vision and Pattern Recognition (CVPR)_, (Las Vegas, NV: IEEE), 770–778.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Deep+residual+learning+for+image+recognition&author=He+K.&author=Zhang+X.&author=Ren+S.&author=Sun+J.&conference=IEEE&publication_year=2016)

Hoshen, Y., and Peleg, S. (2015). “Visual learning of arithmetic operations,” in _Proceedings of the 30th AAAI Conference on Artificial Intelligence_, (Phoenix, AZ: AAAI), 3733–3739.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Visual+learning+of+arithmetic+operations&author=Hoshen+Y.&author=Peleg+S.&conference=&publication_year=2015)

Izard, V., Pica, P., Spelke, E. S., and Dehaene, S. (2008). Exact equality and successor function: two key concepts on the path towards understanding exact numbers. _Philos. Psychol._ 21, 491–505. doi: 10.1080/09515080802285354

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=20165569) | [CrossRef Full Text](https://doi.org/10.1080/09515080802285354) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Exact+equality+and+successor+function%3A+two+key+concepts+on+the+path+towards+understanding+exact+numbers&author=Izard+V.&author=Pica+P.&author=Spelke+E.+S.&author=Dehaene+S.&publication_year=2008&journal=Philos.+Psychol.&volume=21&pages=491-505)

Izard, V., Streri, A., and Spelke, E. S. (2014). Toward exact number: young children use one-to-one correspondence to measure set identity but not numerical equality. _Cogn. Psychol._ 72, 27–53. doi: 10.1016/j.cogpsych.2014.01.004

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=24680885) | [CrossRef Full Text](https://doi.org/10.1016/j.cogpsych.2014.01.004) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Toward+exact+number%3A+young+children+use+one-to-one+correspondence+to+measure+set+identity+but+not+numerical+equality&author=Izard+V.&author=Streri+A.&author=Spelke+E.+S.&publication_year=2014&journal=Cogn.+Psychol.&volume=72&pages=27-53)

Lakoff, G., and Núñez, R. E. (2000). _Where Mathematics Comes From: How the Embodied Mind Brings Mathematics Into Being._ New York, NY: Basic Books.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Where+Mathematics+Comes+From%3A+How+the+Embodied+Mind+Brings+Mathematics+Into+Being&author=Lakoff+G.&author=N%C3%BA%C3%B1ez+R.+E.&publication_year=2000)

Le Corre, M. (2014). Children acquire the later-greater principle after the cardinal principle. _Br. J. Dev. Psychol._ 32, 163–177. doi: 10.1111/bjdp.12029

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=24372336) | [CrossRef Full Text](https://doi.org/10.1111/bjdp.12029) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Children+acquire+the+later-greater+principle+after+the+cardinal+principle&author=Le+Corre+M.&publication_year=2014&journal=Br.+J.+Dev.+Psychol.&volume=32&pages=163-177)

LeCun, Y., Bengio, Y., and Hinton, G. E. (2015). Deep learning. _Nature_ 521, 436–444. doi: 10.1038/nature14539

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=26017442) | [CrossRef Full Text](https://doi.org/10.1038/nature14539) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Deep+learning&author=LeCun+Y.&author=Bengio+Y.&author=Hinton+G.+E.&publication_year=2015&journal=Nature&volume=521&pages=436-444)

Leibovich, T., and Ansari, D. (2016). The symbol-grounding problem in numerical cognition: a review of theory, evidence, and outstanding questions. _Can. J. Exp. Psychol._ 70, 12–23. doi: 10.1037/cep0000070

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=26913782) | [CrossRef Full Text](https://doi.org/10.1037/cep0000070) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=The+symbol-grounding+problem+in+numerical+cognition%3A+a+review+of+theory,+evidence,+and+outstanding+questions&author=Leibovich+T.&author=Ansari+D.&publication_year=2016&journal=Can.+J.+Exp.+Psychol.&volume=70&pages=12-23)

Libertus, M. E., Feigenson, L., and Halberda, J. (2011). Preschool acuity of the approximate number system correlates with school math ability. _Dev. Sci._ 14, 1292–1300. doi: 10.1111/j.1467-7687.2011.01080.x

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=22010889) | [CrossRef Full Text](https://doi.org/10.1111/j.1467-7687.2011.01080.x) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Preschool+acuity+of+the+approximate+number+system+correlates+with+school+math+ability&author=Libertus+M.+E.&author=Feigenson+L.&author=Halberda+J.&publication_year=2011&journal=Dev.+Sci.&volume=14&pages=1292-1300)

Marcus, G. F. (2003). _The Algebraic Mind: Integrating Connectionism and Cognitive Science._ Cambridge, MA: MIT Press.

Marcus, G. F. (2018). Deep learning: a critical appraisal. _arXiv:1801.00631_ [Preprint].

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Deep+learning%3A+a+critical+appraisal&author=Marcus+G.+F.&publication_year=2018&journal=arXiv%3A1801.00631)

Martin, A. E., and Baggio, G. (2020). Modelling meaning composition from formalism to mechanism. _Philos. Trans. R. Soc. B Biol. Sci._ 375:20190298. doi: 10.1098/rstb.2019.0298

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=31840588) | [CrossRef Full Text](https://doi.org/10.1098/rstb.2019.0298) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Modelling+meaning+composition+from+formalism+to+mechanism&author=Martin+A.+E.&author=Baggio+G.&publication_year=2020&journal=Philos.+Trans.+R.+Soc.+B+Biol.+Sci.&volume=375&pages=20190298)

McClelland, J. L., Botvinick, M. M., Noelle, D. C., Plaut, D. C., Rogers, T. T., Seidenberg, M. S., et al. (2010). Letting structure emerge: connectionist and dynamical systems approaches to cognition. _Trends Cogn. Sci._ 14, 348–356. doi: 10.1016/j.tics.2010.06.002

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=20598626) | [CrossRef Full Text](https://doi.org/10.1016/j.tics.2010.06.002) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Letting+structure+emerge%3A+connectionist+and+dynamical+systems+approaches+to+cognition&author=McClelland+J.+L.&author=Botvinick+M.+M.&author=Noelle+D.+C.&author=Plaut+D.+C.&author=Rogers+T.+T.&author=Seidenberg+M.+S.&+&publication_year=2010&journal=Trends+Cogn.+Sci.&volume=14&pages=348-356)

McCloskey, M., and Lindemann, A. M. (1992). Mathnet: preliminary results from a distributed model of arithmetic fact retrieval. _Adv. Psychol._ 91, 365–409. doi: 10.1016/s0166-4115(08)60892-4

[CrossRef Full Text](https://doi.org/10.1016/s0166-4115(08)60892-4) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Mathnet%3A+preliminary+results+from+a+distributed+model+of+arithmetic+fact+retrieval&author=McCloskey+M.&author=Lindemann+A.+M.&publication_year=1992&journal=Adv.+Psychol.&volume=91&pages=365-409)

Menary, R. (2015). Mathematical cognition—a case of encultration. _Open Mind_ 25, 1–20. doi: 10.15502/9783958570818

[CrossRef Full Text](https://doi.org/10.15502/9783958570818) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Mathematical+cognition%E2%80%94a+case+of+encultration&author=Menary+R.&publication_year=2015&journal=Open+Mind&volume=25&pages=1-20)

Menninger, K. (1992). _Number Words and Number Symbols: A Cultural History of Numbers._ New York: Dover Pubns.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Number+Words+and+Number+Symbols%3A+A+Cultural+History+of+Numbers&author=Menninger+K.&publication_year=1992)

Mickey, K. W., and McClelland, J. L. (2014). “A neural network model of learning mathematical equivalence,” in _Proceedings of the 36th Annual Conference of the Cognitive Science Society_, (QC, Canada: Cognitive Science Society), 1012–1017.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=A+neural+network+model+of+learning+mathematical+equivalence&author=Mickey+K.+W.&author=McClelland+J.+L.&conference=&publication_year=2014)

Nasr, K., Viswanathan, P., and Nieder, A. (2019). Number detectors spontaneously emerge in a deep neural network designed for visual object recognition. _Sci. Adv._ 5:eaav7903. doi: 10.1126/sciadv.aav7903

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=31086820) | [CrossRef Full Text](https://doi.org/10.1126/sciadv.aav7903) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Number+detectors+spontaneously+emerge+in+a+deep+neural+network+designed+for+visual+object+recognition&author=Nasr+K.&author=Viswanathan+P.&author=Nieder+A.&publication_year=2019&journal=Sci.+Adv.&volume=5&pages=eaav7903)

Negen, J., and Sarnecka, B. W. (2015). Is there really a link between exact-number knowledge and approximate number system acuity in young children? _Br. J. Dev. Psychol._ 33, 92–105. doi: 10.1111/bjdp.12071

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=25403910) | [CrossRef Full Text](https://doi.org/10.1111/bjdp.12071) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Is+there+really+a+link+between+exact-number+knowledge+and+approximate+number+system+acuity+in+young+children%3F&author=Negen+J.&author=Sarnecka+B.+W.&publication_year=2015&journal=Br.+J.+Dev.+Psychol.&volume=33&pages=92-105)

Núñez, R. E. (2011). No innate number line in the human brain. _J. Cross. Cult. Psychol._ 42, 651–668. doi: 10.1177/0022022111406097

[CrossRef Full Text](https://doi.org/10.1177/0022022111406097) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=No+innate+number+line+in+the+human+brain&author=N%C3%BA%C3%B1ez+R.+E.&publication_year=2011&journal=J.+Cross.+Cult.+Psychol.&volume=42&pages=651-668)

Núñez, R. E. (2017). Is there really an evolved capacity for number? _Trends Cogn. Sci._ 21, 409–424. doi: 10.1016/j.tics.2017.03.005

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=28526128) | [CrossRef Full Text](https://doi.org/10.1016/j.tics.2017.03.005) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Is+there+really+an+evolved+capacity+for+number%3F&author=N%C3%BA%C3%B1ez+R.+E.&publication_year=2017&journal=Trends+Cogn.+Sci.&volume=21&pages=409-424)

Overmann, K. A. (2016). The role of materiality in numerical cognition. _Quat. Int._ 405, 42–51. doi: 10.1016/j.quaint.2015.05.026

[CrossRef Full Text](https://doi.org/10.1016/j.quaint.2015.05.026) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=The+role+of+materiality+in+numerical+cognition&author=Overmann+K.+A.&publication_year=2016&journal=Quat.+Int.&volume=405&pages=42-51)

Overmann, K. A. (2018). Constructing a concept of number. _J. Numer. Cogn._ 4, 464–493. doi: 10.5964/jnc.v4i2.161

[CrossRef Full Text](https://doi.org/10.5964/jnc.v4i2.161) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Constructing+a+concept+of+number&author=Overmann+K.+A.&publication_year=2018&journal=J.+Numer.+Cogn.&volume=4&pages=464-493)

Pezzelle, S., Sorodoc, I.-T., and Bernardi, R. (2018). “Comparatives, quantifiers, proportions: a multi-task model for the learning of quantities from vision,” in _Proceedings of the 2018 Conference of the Association for Computational Linguistics_, (New Orleans, LA: Association for Computational Linguistics), 419–430.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Comparatives,+quantifiers,+proportions%3A+a+multi-task+model+for+the+learning+of+quantities+from+vision&author=Pezzelle+S.&author=Sorodoc+I.-T.&author=Bernardi+R.&conference=Association+for+Computational+Linguistics&publication_year=2018)

Piantadosi, S. T., Tenenbaum, J. B., and Goodman, N. D. (2012). Bootstrapping in a language of thought: a formal model of numerical concept learning. _Cognition_ 123, 199–217. doi: 10.1016/j.cognition.2011.11.005

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=22284806) | [CrossRef Full Text](https://doi.org/10.1016/j.cognition.2011.11.005) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Bootstrapping+in+a+language+of+thought%3A+a+formal+model+of+numerical+concept+learning&author=Piantadosi+S.+T.&author=Tenenbaum+J.+B.&author=Goodman+N.+D.&publication_year=2012&journal=Cognition&volume=123&pages=199-217)

Piazza, M. (2010). Neurocognitive start-up tools for symbolic number representations. _Trends Cogn. Sci._ 14, 542–551. doi: 10.1016/j.tics.2010.09.008

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=21055996) | [CrossRef Full Text](https://doi.org/10.1016/j.tics.2010.09.008) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Neurocognitive+start-up+tools+for+symbolic+number+representations&author=Piazza+M.&publication_year=2010&journal=Trends+Cogn.+Sci.&volume=14&pages=542-551)

Platt, J. R., and Johnson, D. M. (1971). Localization of position within a homogeneous behavior chain: effects of error contingencies. _Learn. Motiv._ 2, 386–414. doi: 10.1016/0023-9690(71)90020-8

[CrossRef Full Text](https://doi.org/10.1016/0023-9690(71)90020-8) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Localization+of+position+within+a+homogeneous+behavior+chain%3A+effects+of+error+contingencies&author=Platt+J.+R.&author=Johnson+D.+M.&publication_year=1971&journal=Learn.+Motiv.&volume=2&pages=386-414)

Rittle-Johnson, B., Siegler, R. S., and Alibali, M. W. (2001). Developing conceptual understanding and procedural skill in mathematics: an iterative process. _J. Educ. Psychol._ 93, 346–362. doi: 10.1037/0022-0663.93.2.346

[CrossRef Full Text](https://doi.org/10.1037/0022-0663.93.2.346) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Developing+conceptual+understanding+and+procedural+skill+in+mathematics%3A+an+iterative+process&author=Rittle-Johnson+B.&author=Siegler+R.+S.&author=Alibali+M.+W.&publication_year=2001&journal=J.+Educ.+Psychol.&volume=93&pages=346-362)

Rucinski, M., Cangelosi, A., and Belpaeme, T. (2012). “Robotic model of the contribution of gesture to learning to count,” in _IEEE International Conference on Development and Learning and Epigenetic Robotics_ (San Diego, CA, USA: IEEE), 1–6. doi: 10.1109/DevLrn.2012.6400579

[CrossRef Full Text](https://doi.org/10.1109/DevLrn.2012.6400579) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Robotic+model+of+the+contribution+of+gesture+to+learning+to+count&author=Rucinski+M.&author=Cangelosi+A.&author=Belpaeme+T.&conference=&publication_year=2012)

Rumelhart, D. E., and McClelland, J. L. (1986). _Parallel Distributed Processing: Explorations in the Microstructure of Cognition. Volume 1: Foundations_. Cambridge, MA: MIT Press.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Parallel+Distributed+Processing%3A+Explorations+in+the+Microstructure+of+Cognition.+Volume+1%3A+Foundations&author=Rumelhart+D.+E.&author=McClelland+J.+L.&publication_year=1986)

Rumelhart, D. E., Smolensky, P., McClelland, J. L., and Hinton, G. E. (1986). “Schemata and sequential thought processes in PDP models,” in _Parallel Distributed Processing: Explorations in the Microstructure of Cognition Volume 2: Psychological and Biological Models_ eds J. L. McClelland and D. E. Rumelhart (Cambridge, MA: MIT Press), 7–57.

Sarnecka, B. W., and Carey, S. (2008). How counting represents number: what children must learn and when they learn it. _Cognition_ 108, 662–674. doi: 10.1016/j.cognition.2008.05.007

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=18572155) | [CrossRef Full Text](https://doi.org/10.1016/j.cognition.2008.05.007) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=How+counting+represents+number%3A+what+children+must+learn+and+when+they+learn+it&author=Sarnecka+B.+W.&author=Carey+S.&publication_year=2008&journal=Cognition&volume=108&pages=662-674)

Saxton, D., Grefenstette, E., Hill, F., and Kohli, P. (2019). “Analysing mathematical reasoning abilities of neural models,” in _International Conference on Learning Representations_, (New Orleans, LA: ICLR), 1–17.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Analysing+mathematical+reasoning+abilities+of+neural+models&author=Saxton+D.&author=Grefenstette+E.&author=Hill+F.&author=Kohli+P.&conference=&publication_year=2019)

Schmandt-Besserat, D. (1992). _Before Writing: From Counting to Cuneiform._ Austin, TX: University of Texas Press.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Before+Writing%3A+From+Counting+to+Cuneiform&author=Schmandt-Besserat+D.&publication_year=1992)

Schneider, M., Beeres, K., Coban, L., Merz, S., Susan Schmidt, S., Stricker, J., et al. (2017). Associations of non-symbolic and symbolic numerical magnitude processing with mathematical competence: a meta-analysis. _Dev. Sci._ 20:e12372. doi: 10.1111/desc.12372

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=26768176) | [CrossRef Full Text](https://doi.org/10.1111/desc.12372) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Associations+of+non-symbolic+and+symbolic+numerical+magnitude+processing+with+mathematical+competence%3A+a+meta-analysis&author=Schneider+M.&author=Beeres+K.&author=Coban+L.&author=Merz+S.&author=Susan+Schmidt+S.&author=Stricker+J.&+&publication_year=2017&journal=Dev.+Sci.&volume=20&pages=e12372)

Searle, J. R. (1980). Minds, brains, and programs. _Behav. Brain Sci._ 3, 417–424. doi: 10.1017/S0140525X00005756

[CrossRef Full Text](https://doi.org/10.1017/S0140525X00005756) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Minds,+brains,+and+programs&author=Searle+J.+R.&publication_year=1980&journal=Behav.+Brain+Sci.&volume=3&pages=417-424)

Siegler, R. S., and Jenkins, E. (1989). _How Children Discover New Strategies._ New York, NY: Psychology Press.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=How+Children+Discover+New+Strategies&author=Siegler+R.+S.&author=Jenkins+E.&publication_year=1989)

Silver, D., Schrittwieser, J., Simonyan, K., Antonoglou, I., Huang, A., Guez, A., et al. (2017). Mastering the game of Go without human knowledge. _Nature_ 550, 354–359. doi: 10.1038/nature24270

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=29052630) | [CrossRef Full Text](https://doi.org/10.1038/nature24270) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Mastering+the+game+of%E2%80%88+Go+without+human+knowledge&author=Silver+D.&author=Schrittwieser+J.&author=Simonyan+K.&author=Antonoglou+I.&author=Huang+A.&author=Guez+A.&+&publication_year=2017&journal=Nature&volume=550&pages=354-359)

Skinner, B. (1953). _Science and Human Behavior._ New York, NY: MacMillan.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Science+and+Human+Behavior&author=Skinner+B.&publication_year=1953)

Starkey, G. S., and McCandliss, B. D. (2014). The emergence of “groupitizing” in children’s numerical cognition. _J. Exp. Child Psychol._ 126, 120–137. doi: 10.1016/j.jecp.2014.03.006

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=24926937) | [CrossRef Full Text](https://doi.org/10.1016/j.jecp.2014.03.006) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=The+emergence+of+%E2%80%9Cgroupitizing%E2%80%9D+in+children%27s+numerical+cognition&author=Starkey+G.+S.&author=McCandliss+B.+D.&publication_year=2014&journal=J.+Exp.+Child+Psychol.&volume=126&pages=120-137)

Starr, A., Libertus, M. E., and Brannon, E. M. (2013). Number sense in infancy predicts mathematical abilities in childhood. _Proc. Natl. Acad. Sci. U S A_ 110, 18116–18120. doi: 10.1073/pnas.1302751110

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=24145427) | [CrossRef Full Text](https://doi.org/10.1073/pnas.1302751110) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Number+sense+in+infancy+predicts+mathematical+abilities+in+childhood&author=Starr+A.&author=Libertus+M.+E.&author=Brannon+E.+M.&publication_year=2013&journal=Proc.+Natl.+Acad.+Sci.+U+S+A&volume=110&pages=18116-18120)

Stoianov, I., and Zorzi, M. (2012). Emergence of a “visual number sense” in hierarchical generative models. _Nat. Neurosci._ 15, 194–196. doi: 10.1038/nn.2996

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=22231428) | [CrossRef Full Text](https://doi.org/10.1038/nn.2996) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Emergence+of+a+%E2%80%9Cvisual+number+sense%E2%80%9D+in+hierarchical+generative+models&author=Stoianov+I.&author=Zorzi+M.&publication_year=2012&journal=Nat.+Neurosci.&volume=15&pages=194-196)

Sutton, R. S., and Barto, A. G. (1998). _Reinforcement Learning._ Cambridge, MA: MIT Press.

Testolin, A., Dolfi, S., Rochus, M., and Zorzi, M. (2019). Perception of visual numerosity in humans and machines _arXiv:1907.06996_ [Preprint].

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Perception+of+visual+numerosity+in+humans+and+machines&author=Testolin+A.&author=Dolfi+S.&author=Rochus+M.&author=Zorzi+M.&publication_year=2019&journal=arXiv%3A1907.06996)

Testolin, A., Stoianov, I., and Zorzi, M. (2017). Letter perception emerges from unsupervised deep learning and recycling of natural image features. _Nat. Hum. Behav._ 1, 657–664. doi: 10.1038/s41562-017-0186-2

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=31024135) | [CrossRef Full Text](https://doi.org/10.1038/s41562-017-0186-2) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Letter+perception+emerges+from+unsupervised+deep+learning+and+recycling+of+natural+image+features&author=Testolin+A.&author=Stoianov+I.&author=Zorzi+M.&publication_year=2017&journal=Nat.+Hum.+Behav.&volume=1&pages=657-664)

Testolin, A., and Zorzi, M. (2016). Probabilistic models and generative neural networks: towards an unified framework for modeling normal and impaired neurocognitive functions. _Front. Comput. Neurosci._ 10:73. doi: 10.3389/fncom.2016.00073

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=27468262) | [CrossRef Full Text](https://doi.org/10.3389/fncom.2016.00073) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Probabilistic+models+and+generative+neural+networks%3A+towards+an+unified+framework+for+modeling+normal+and+impaired+neurocognitive+functions&author=Testolin+A.&author=Zorzi+M.&publication_year=2016&journal=Front.+Comput.+Neurosci.&volume=10&pages=73)

Testolin, A., Zou, W. Y., and McClelland, J. L. (2020). Numerosity discrimination in deep neural networks: initial competence, developmental refinement and experience statistics. _Dev. Sci._ doi: 10.1111/desc.12940 [Epub ahead of print].

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=31977137) | [CrossRef Full Text](https://doi.org/10.1111/desc.12940%20[Epub%20ahead%20of%20print].) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Numerosity+discrimination+in+deep+neural+networks%3A+initial+competence,+developmental+refinement+and+experience+statistics&author=Testolin+A.&author=Zou+W.+Y.&author=McClelland+J.+L.&publication_year=2020&journal=Dev.+Sci.)

Trask, A., Hill, F., Reed, S., Rae, J., Dyer, C., and Blunsom, P. (2018). Neural arithmetic logic units. _arXiv:1808.00508_ [Preprint].

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Neural+arithmetic+logic+units&author=Trask+A.&author=Hill+F.&author=Reed+S.&author=Rae+J.&author=Dyer+C.&author=Blunsom+P.&publication_year=2018&journal=arXiv%3A1808.00508)

Verguts, T., and Fias, W. (2004). Representation of number in animals and humans: a neural model. _J. Cogn. Neurosci._ 16, 1493–1504. doi: 10.1162/0898929042568497

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=15601514) | [CrossRef Full Text](https://doi.org/10.1162/0898929042568497) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Representation+of+number+in+animals+and+humans%3A+a+neural+model&author=Verguts+T.&author=Fias+W.&publication_year=2004&journal=J.+Cogn.+Neurosci.&volume=16&pages=1493-1504)

Vygotsky, L. S. (1980). _Mind in Society: The Development of Higher Psychological Processes._ Cambridge, MA: Harvard University Press.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Mind+in+Society%3A+The+Development+of+Higher+Psychological+Processes&author=Vygotsky+L.+S.&publication_year=1980)

Walshaw, M. (2017). Understanding mathematical development through Vygotsky. _Res. Math. Educ._ 19, 293–309. doi: 10.1080/14794802.2017.1379728

[CrossRef Full Text](https://doi.org/10.1080/14794802.2017.1379728) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Understanding+mathematical+development+through+Vygotsky&author=Walshaw+M.&publication_year=2017&journal=Res.+Math.+Educ.&volume=19&pages=293-309)

Wever, R., and Runia, T. F. H. (2019). Subitizing with variational autoencoders. _arXiv:1808.00257_ [Preprint].

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Subitizing+with+variational+autoencoders&author=Wever+R.&author=Runia+T.+F.+H.&publication_year=2019&journal=arXiv%3A1808.00257)

Wilkey, E. D., and Ansari, D. (2019). Challenging the neurobiological link between number sense and symbolic numerical abilities. _Ann. N Y Acad. Sci._ doi: 10.1111/nyas.14225 [Epub ahead of print].

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=31549430) | [CrossRef Full Text](https://doi.org/10.1111/nyas.14225%20[Epub%20ahead%20of%20print].) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Challenging+the+neurobiological+link+between+number+sense+and+symbolic+numerical+abilities&author=Wilkey+E.+D.&author=Ansari+D.&publication_year=2019&journal=Ann.+N+Y+Acad.+Sci.)

Yamins, D. L. K., and DiCarlo, J. J. (2016). Using goal-driven deep learning models to understand sensory cortex. _Nat. Neurosci._ 19, 356–365. doi: 10.1038/nn.4244

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=26906502) | [CrossRef Full Text](https://doi.org/10.1038/nn.4244) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Using+goal-driven+deep+learning+models+to+understand+sensory+cortex&author=Yamins+D.+L.+K.&author=DiCarlo+J.+J.&publication_year=2016&journal=Nat.+Neurosci.&volume=19&pages=356-365)

Zanetti, A., Testolin, A., Zorzi, M., and Wawrzynski, P. (2019). Numerosity representation in InfoGAN: an empirical study _Advances in Computational Intelligence. IWANN_, eds I. Rojas, G. Joya and A. Catala (Cham: Springer International Publishing), 49–60.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Numerosity+representation+in+InfoGAN%3A+an+empirical+study&author=Zanetti+A.&author=Testolin+A.&author=Zorzi+M.&author=Wawrzynski+P.&publication_year=2019&pages=49-60)

Zhao, S., Ren, H., Yuan, A., Song, J., Goodman, N., and Ermon, S. (2018). “Bias and generalization in deep generative models: an empirical study,” in _32nd International Conference on Neural Information Processing Systems_ (Montréal, QC: NeurIPS), 10792–10801.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Bias+and+generalization+in+deep+generative+models%3A+an+empirical+study&author=Zhao+S.&author=Ren+H.&author=Yuan+A.&author=Song+J.&author=Goodman+N.&author=Ermon+S.&conference=&publication_year=2018)

Zorzi, M., Stoianov, I., and Umiltà, C. (2005). “Computational modeling of numerical cognition,” in _Handbook of Mathematical Cognition_, ed. J. Campbell (New York, NY: Psychology Press), 67–84.

[Google Scholar](http://scholar.google.com/scholar_lookup?title=Computational+modeling+of+numerical+cognition&author=Zorzi+M.&author=Stoianov+I.&author=Umilt%C3%A0+C.&publication_year=2005&pages=67-84)

Zorzi, M., and Testolin, A. (2018). An emergentist perspective on the origin of number sense. _Philos. Trans. R. Soc. B Biol. Sci._ 373:20170043. doi: 10.1098/rstb.2017.0043

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=29292348) | [CrossRef Full Text](https://doi.org/10.1098/rstb.2017.0043) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=An+emergentist+perspective+on+the+origin+of+number+sense&author=Zorzi+M.&author=Testolin+A.&publication_year=2018&journal=Philos.+Trans.+R.+Soc.+B+Biol.+Sci.&volume=373&pages=20170043)

Zorzi, M., Testolin, A., and Stoianov, I. P. I. P. (2013). Modeling language and cognition with deep unsupervised learning: a tutorial overview. _Front. Psychol._ 4:515. doi: 10.3389/fpsyg.2013.00515

[PubMed Abstract](http://www.ncbi.nlm.nih.gov/sites/entrez?Db=pubmed&Cmd=ShowDetailView&TermToSearch=23970869) | [CrossRef Full Text](https://doi.org/10.3389/fpsyg.2013.00515) | [Google Scholar](http://scholar.google.com/scholar_lookup?title=Modeling+language+and+cognition+with+deep+unsupervised+learning%3A+a+tutorial+overview&author=Zorzi+M.&author=Testolin+A.&author=Stoianov+I.+P.+I.+P.&publication_year=2013&journal=Front.+Psychol.&volume=4&pages=515)

Keywords: computational modeling, artificial neural networks, deep learning, number sense, symbol grounding, mathematical learning, embodied cognition, material culture

Citation: Testolin A (2020) The Challenge of Modeling the Acquisition of Mathematical Concepts. Front. Hum. Neurosci. 14:100. doi: 10.3389/fnhum.2020.00100

Received: 13 November 2019; Accepted: 04 March 2020;

Published: 20 March 2020.

Edited by:

[Elise Klein](https://loop.frontiersin.org/people/35071/overview), University of Tübingen, Germany

Reviewed by:

[Xinlin Zhou](https://loop.frontiersin.org/people/96337/overview), Beijing Normal University, China

[Tom Verguts](https://loop.frontiersin.org/people/25620/overview), Ghent University, Belgium

Copyright © 2020 Testolin. This is an open-access article distributed under the terms of the [Creative Commons Attribution License (CC BY)](http://creativecommons.org/licenses/by/4.0/). The use, distribution or reproduction in other forums is permitted, provided the original author(s) and the copyright owner(s) are credited and that the original publication in this journal is cited, in accordance with accepted academic practice. No use, distribution or reproduction is permitted which does not comply with these terms.

Disclaimer: All claims expressed in this article are solely those of the authors and do not necessarily represent those of their affiliated organizations, or those of the publisher, the editors and the reviewers. Any product that may be evaluated in this article or claim that may be made by its manufacturer is not guaranteed or endorsed by the publisher.