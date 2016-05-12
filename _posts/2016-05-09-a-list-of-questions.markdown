---
layout: post
title:  "A list of questions"
date:   2016-05-09
---

Here is a set of issues that I would like to understand better -  a sort of agenda for future posts.

### Parallel computation.
Large brains consist of a vast number of cells which may be considered the individual processing units. To support scaleability, resource usage per processing component (eg. energy usage, wiring length) should remain constant or grow at most logarithmically with the number of components. Similarly running times should remain constant or grow logarithmically. These limitations describe what we shall refer to as the class of scaleable or massively parallel computations.

- What are the basic algorithms of massively parallel computation?
- How does this kind of massive parallelism interact with coarser levels of parallelism in which multiple larger modules or brain regions cooperate on a task?

### Hierarchy.
According to our definition of massively parallel computation, running times and wiring length per component should grow at most logarithmically with system size. A simple arrangement in which these resources remain constant consists of a spatially organised layout of components with local connections, running a message passing algorithm for a constant number of time steps. Such a computation will only propagate information over a finite distance and thus will not allow distant components to communicate.

A natural generalisation which allows communication across the full system in logarithmic time, is to add additional layers of processors at successively coarser scales and to pass messages up and down the resulting tree structure. In this way, scale hierarchies form a natural component of locally organised, parallel computation.

The usefulness of this construction depends on the problem under study, but in many cases the sensory information and the decisions processed by animal brains possess spatial or temporal structure over a range of length scales and are usefully processed in a hierarchical manner. This is reflected in the strongly hierarchical organisation of animal cortices.

- How can we uncover and make use of hierarchical structures present in a sensory signal or decision process?
- How should the different modules in a hierarchical computation exchange information during learning and computation?

### Dynamics.
Animals and robots operate in dynamic environments and need to plan actions in real-time. A large body of research in machine learning and optimization studies static problems and it is of interest to understand which parts carry over to the dynamic setting.

- What are the relationships between algorithms for static and dynamic problems and which types of static algorithm adapt gracefully to a moving target?
- What type of state representations and algorithms are suitable for decision making in a high-dimensional, dynamical setting?

### Unsupervised learning.
Much of the recent success in machine learning has been in supervised learning, in which labelled examples are provided for a classification problem and the aim is to generalise from these. A difficulty with this approach is that the measure of success (correct/incorrect label) cannot be computed without prior access to a solution to the underlying problem and thus intelligent behaviour cannot be bootstrapped in this way. Animals, on the other hand, learn to interact with their environments in a largely unsupervised manner, and the reward signals that they learn to optimise are more primitive than the behaviours that they learn.

- What types of computation are accessible to bootstrapping from more primitive reward signals?
- What are the appropriate training signals for unsupervised learning from sensorimotor information?

### Robustness.
Animal brains have evolved to solve problems in a manner that helps to ensure the survival of the host. Extreme precision, may not be a goal if it comes at the expense of computation time, energy usage or robustness. Indeed the cost to the animal's chances of survival from a single large error may far outweigh the gains from a modest increase in precision.

- How should we measure the robustness of algorithms?
- What types of algorithm display appropriate levels of robustness for decision making in noisy, changing environments?

### Learnability.
Animals learn quickly from novel experiences, whilst machine learning algorithms typically require lengthy training to incorporate new information. Also many machine learning algorithms involve difficult optimisations and extensive tuning of hyperparameters whilst animal learning is extremely robust and needs to work reliably in a range of environments without external tuning.

- What features of learning algorithms support the robustness and rapid adaptation to novel information shown by animal brains?
