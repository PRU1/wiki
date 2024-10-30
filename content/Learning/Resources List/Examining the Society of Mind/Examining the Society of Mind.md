---
Link: https://www.jfsowa.com/ikl/Singh03.htm
ee:
  - EE
---
Author: Push Singh

MIT Media lab

summarizes Society of Mind + introduces author’s own ideas and considers “related developments in AI since the theory’s publication”

  

# introduction

what is the mind and how does it work?

“How do we recognize objects and scenes? How do we use words and language? How do we achieve goals? How do we learn new concepts and skills? How do we understand things? What are feelings and emotions? How does 'common sense' work?”

  

- Minsky proposes that there isn’t a “basic principle” that governs the behaviour of cognitive phenomena
- instead, the mind is a really a “society of mind” —> “a tremendously rich and multifaceted society of structures and processes”
- Agent: simplest individuals in a society of mind
- society of agents performs complicated functions, more than a single agent

# the early development of the Society of Mind theory

origin of “society of mind”

- Minsky and Papert + MIT students were working on a robot that could build blocks
- no single algorithm was good enough to solve assembling a trivial task like building a block of towers
    - conclusion “ this experience impressed on us the idea that only a society of different types of processes could possibly suffice “
- intelligence in the combined activity of societies of specilalized cognitive processes.
- Allan Newell in 1962

> The problem solver should be a single personality, wandering over a goal net much as an explorer wanders over the countryside, having a single context and taking it with him wherever he goes

Implementing idea of societies of interacting agents

- first came up in the 1970s
- Carl Hewitt’s concept of “Actors”.
    
    - you have groups of agents active at the same time
    - solve problems through actors exchanging messages
    - this “greatly [simplified] the control structure of complex programs”
    
    ![[/Untitled 6.png|Untitled 6.png]]
    
      
    

# how do societies of mind work?

- agency: groups of agents that perform complicated tasks
- Minsky argues the mind is a bunch of cognitive processes specialized to perform a specific function —> “expecting, predicting, repairing, remembering, revising, debugging, acting, comparing, generalizing, exemplifying, analogizing, simplifying, and many other such 'ways of thinking'.”
- agent: a part of a cognitive process that is simple enough to understand

## what are the simplest agents

- **K-Lines** : purpose: turn on a set of agents. Agents have interconnections, activating a kline creates a domino effect.
    - simple and powerful way to make a mind work towards problem solving thingies, goals, memories of particular experiences
- There are **nomes and nemes** which are types of **k-lines**
    
    - nemes: represent aspects of the world
    - nomes: control how these aspects are processed
    
    there are two types of nemes
    
    - **polynemes** and **micronemes**
        - polyneme: “invoke partial states within multiple agencies” i.e. polynemes recgonize an apple induces an “apple-polyneme” which has certain properties such as - colour, shape, taste, stuff that creates the Apple Experience
        - polynemes support the idea, the meaning of something is expressed by multiple properties but not a single representation (whatever this means ……)
        - micronemes: “global contextual signals to agencies all across the brain”.
            - things that are too “subtle” for words and that don’t have properties (i.e. polynemes like smells or colours)
        - nemes are organized into ‘ring-closing’ networks
            - used in pattern recognition
            - I don’t get this. Read Minsky’s book on this
    
    - NOMES
        - controls how representations are manipulated
        - Isonames, pronomes, paranomes
        - Isonomes: “sends a signal to different agencies to perform the same cognitive operation” (changed one word)
        - pronomes: controls use of brain RAM representations
            - what is a representation?
        - Paranomes: a set of linked pronomes. a change in one pronome causes other pronomes in a paranome to change too

## how do you combine agents to build larger agencies?

- use a frame
- a frame organizes knowledge representations that are similar/related. slots them all together
- frame arrays: a collection of frames
- Transframes: collection of all events + entities (what are events and entities in the context of mind huhhh) relating to a specific event.
    - slots representing before + after + during + destination of event, how objects of frame are effected.

## how can agents solve problems

- Minsky says there is no single way to solve a problem
- he suggests ways to you can build/organize a problem solving agency
- **difference engine** look at the difference between the current state and the desired state.
- difference-engine looks at these differences and invokes k-lines to try to find a solution. based on Newell and Simon’s early ‘GPS’ problem solver
- **Censors and suppressors:** have knowledge to avoid common bugs + pitfalls. this type of knowledge Minsky calls negative expertise
    - knowledge is embodied in censor and suppressor agents
    - censors: censor stuff; inhibit thoughts that are unproductive/dangerous
    - suppressors: supress unproductive + dangerous thoughts themselves
- A-brains and B-brains: B-brain thinks about world inside the mind (A-brain), notices errors of looping and meandering and fixes these.

## how do agents communicate with each other

- simple agents have a hard time communicating
- “this is not because there are too many meanings, but because there are too few. The fewer things an agent does, the less likely that what another agent does will correspond to any of those things”
- connection lines: agents are not directly connected but communicate through ‘communication lines’. you can think of these communication lines as agents themselves.
- agents communicate through connection lines by connecting k lines. this strategy of random connection was first invented by Calvin Mooers. (a bus is a bundle of wires)
- agents connected to bus need to make guesses have to guess the meaning of the transmitted signal ??? double check this
- **internal language** sometimes you got to communicate complicated things (i.e. complex descriptions of things like when you have a system of linked frames —> frame array?). Minsky says that there is an communication mechanism for this
    - modelled after “re-duplication theory”
    - when receiving a message, an agent will attempt to reconstruct the message in terms of its own “representational system by a sequence of frame retrieval and instantiation operations.”
    - **Paranomes:** no active communication. agents find that information is already available when they need it

## the growth of mental societies

- how do societies of mind “grow up”
- trajectory varies person to person
- **protospecialists:** infant mind has protospecialists which are agencies that make behaviours to solve a person’s first problems (locomotion, food, staying warm, away from predators, etc.). Protospecialists are unskilled but their performance improves through agencies that develop with time
- **predestined learning**: Minsky suggests that there are certain skills that are guaranteed to develop under sufficient internal + external constraints (what is an example of an internal or external constraint?)
- **types of learning** _accumulating:_ remember what you experience. _uniframing_ find a description that explains several examples. _reformulation_ find new ways to describe existing knowledge
- **learning from attachment figures** “a very important type of learning is concerned with the question of how we learn our goals in the first place” —> learn when a specific goal should be adopted, and how to choose which goal to pursue (prioritization)
- **learning mental managers** when and how to use knowledge —> useful in conflict resolution strategies
- **developmental stages** idea that the mind develops in multiple stages. these stages “train” each other,