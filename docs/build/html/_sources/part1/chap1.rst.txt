Chapter 1 Introduction
======================

1.1 What Is AI?
---------------

Some definitions of artificial intelligence:

* Thinking Humanly
* Acting Humanly
* Thinking Rationally
* Acting Rationally

1.1.1 Acting humanly: The Turing test approach
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The **Turing test**, proposed by Alan Turing, was designed as a thought 
experiment that would sidestep the philosophical vagueness of the question
"Can a machine think?"
The computer would need the following capabilities to pass the Turing test:

* **natural language processing** to communicate successfully in a human language
* **knowledge representation** to store what it knows or hears
* **automated reasoning** to answer questions and to draw new conclusions
* **machine learning** to adapt to new circumstances and to detect and extrapolate patterns

To pass the **total Turing test**, a robot will need

* **computer vision** and speech recognition to perceive the world
* **robotics** to manipulate objects and move about.

1.1.2 Thinking humanly: The cognitive modeling approach
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

We can learn about human thought in three ways:

* **introspection**--trying to catch our own thoughts as they go by
* **psychological experiments**--observing a person in action
* **brain imaging**--observing the brain in action
  
The interdisciplinary field of **cognitive science** brings together computer 
models from AI and experimental techniques from psychology to construct precise
and testable theories of the human mind.

1.1.3 Thinking rationally: The "laws of thought" approach
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Several Greek schools developed various forms of **logic**, which provides a
precise notation for statements bout objects in the world and the relations
among them.

1.1.4 Acting rationally: The rational agent approach
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

An **agent** is just something that acts.
A **rational agent** is one that acts so as to achieve the best outcome or, when 
there is uncertainty, the best expected outcome.

*AI has focused on the study and constructionof agents that* **do the right thing**.
This general paradigm is so pervasive that we might call it the **standard model**.

**Limited rationality**: act appropriately when there is not enough time to do all the computations one might take.

1.1.5 Beneficial machines
^^^^^^^^^^^^^^^^^^^^^^^^^

The standard model has been a useful guide for AI research since its inception, 
but it is probably not the right model in the long run. 
The reason is that the standard model assumes that we will supply a fully specified objective to the machine.

The problem of achieving agreement between our true preferences and the 
objective we put into the machine is called the *value alignment problem**: the 
values or objectives put intothe machine must be aligned with those of the human.

We don’t want machines that are intelligent in the sense of pursuing *their* 
objectives; we want them to pursue *our* objectives.
Ultimately, we want agents that are **provably beneficial** to humans.

1.2 The Foundations of Artificial Intelligence
----------------------------------------------

1.2.1 Philosophy
^^^^^^^^^^^^^^^^

* Can formal rules be used to draw valid conclusions?
* How does the mind arise from a physical brain?
* Where does knowledge come from?
* How does knowledge lead to action?

Descartes was a proponent of **dualism**. 
He held that there is a part of the human mind (or soul or spirit) that is outside of nature, exempt from physical laws. 
Animals, on the other hand, did not possess this dual quality; they could be treated as machines.

An alternative to dualism is **materialism**, which holds that the brain’s 
operation according to the laws of physics constitutes the mind. 
Free will is simply the way that the perception of available choices appears to the choosing entity.

The **empiricism** is characterized by a dictum of John Locke (1632–1704): 
“Nothing is in the understanding, which was not first in the senses.”

The **logical positivism** holds that all knowledge can be characterized by 
logical theories connected, ultimately, to **observation sentences** that 
correspond to sensory inputs; thus logical positivism combines rationalism and 
empiricism.

The **confirmation theory** attempted to analyze the acquisition of knowledge 
from experience by quantifying the degree of belief that should be assigned to 
logical sentences based on their connection to observations that confirm or 
disconfirm them.

**Utilitarianism**: that rational decision making based on maximizing utility 
should apply to all spheres of human activity, including public policy decisions 
made on behalf of many individuals.
Utilitarianism is a specific kind of **consequentialism**: the idea that what is 
right and wrong is determined by the expected outcomes of an action.

In contrast, a theory of rule-based or **deontological ethics**, in which “doing 
the right thing” is determined not by outcomes but by universal social laws that 
govern allowable actions, such as “don’t lie” or “don’t kill.”
Many modern AI systems adopt exactly this approach.

1.2.2 Mathematics
^^^^^^^^^^^^^^^^^

* What are the formal rules to draw valid conclusions?
* What can be computed?
* How do we reason with uncertain information?

The theory of **probability** can be seen as generalizing logic to situations 
with uncertain information—a consideration of great importance for AI.
The formalization of probability, combined with the availability of data, led to 
the emergence of **statistics** as a field.

The history of computation is as old as the history of numbers, but the first 
nontrivial **algorithm** is thought to be Euclid’s algorithm for computing 
greatest common divisors.
The **incompleteness theorem** showed that in any formal theory as strong as 
Peano arithmetic (the elementary theory of natural numbers), there are 
necessarily true statements that have no proof within the theory.

Alan Turing tried to characterize exactly which functions *are* **computable**
—capable of being computed by an effective procedure.
For example, no machine can tell *in general* whether a given program will 
return an answer on a given input or run forever.

Although computability is important to an understanding of computation, the 
notion of **tractability** has had an even greater impact on AI. 
A problem is called intractable if the time required to solve instances of the 
problem grows exponentially with the size of the instances.

The theory of **NP-completeness** provides a basis for analyzing the 
tractability of problems: any problem class to which the class of NP-complete 
problems can be reduced is likely to be intractable.

1.2.3 Economics
^^^^^^^^^^^^^^^

* How should we make decisions in accordance with our preferences?
* How should we do this when others may not go along?
* How should we do this when the payoff may be far in the future?

**Decision theory**, which combines probability theory with utility theory, 
provides a formal and complete framework for individual decisions (economic or 
otherwise) made under uncertainty—that is, in cases where probabilistic 
descriptions appropriately capture the decision maker’s environment.

Models based on **satisficing**—making decisions that are “good enough,” rather
than laboriously calculating an optimal decision—gave a better description of 
actual human behavior.

1.2.4 Neuroscience
^^^^^^^^^^^^^^^^^^

* How do brains process information?

**Neuroscience** is the study of the nervous system, particularly the brain.
*A collection of simple cells can lead to thought, action, and consciousness*.

Even with a computer of virtually unlimited capacity, we still require further 
conceptual breakthroughs in our understanding of intelligence.

1.2.5 Psychology
^^^^^^^^^^^^^^^^

* How do humans and animals think and act?

Wundt insisted on carefully controlled experiments in which his workers would 
perform a perceptual or associative task while introspecting on their thought 
processes.
The **behaviorism** movement rejected any theory involving mental processes on 
the grounds that introspection could not provide reliable evidence.

**Cognitive psychology** views the brain as an information-processing device.
Three key steps of a knowledge-based agent: (1) the stimulus must be translated 
into an internal representation, (2) the representation is manipulated by 
cognitive processes to derive new internal representations, and (3) these are in 
turn retranslated back into action.

**Intelligence augmentation** states that computers should augment human 
abilities rather than automate away human tasks.

1.2.6 Computer engineering
^^^^^^^^^^^^^^^^^^^^^^^^^^

* How can we build an efficient computer?

**Moore’s law** states that performance doubled every 18 months.
**Quantum computing** holds out the promise of far greater accelerations for 
some important subclasses of AI algorithms.

1.2.7 Control theory and cybernetics
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* How can artifacts operate under their own control?

Modern control theory, especially the branch known as stochastic optimal 
control, has as its goal the design of systems that maximize a **cost function** 
over time.

1.2.8 Linguistics
^^^^^^^^^^^^^^^^^

* How does language relate to thought?

Modern linguistics and AI, then, were “born” at about the same time, and grew up 
together, intersecting in a hybrid field called **computational linguistics** or 
**natural language processing**.

1.3 The History of Artificial Intelligence
------------------------------------------

1.3.1 The inception of artificial intelligence (1943-1956)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The first work that is now generally recognized as AI was done by Warren 
McCulloch and Walter Pitts (1943).

1.3.2 Early enthusiasm, great expectations (1952-1969)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The intellectual establishment of the 1950s, by and large, preferred to believe
that "a machine can never do X".
John McCarthy referred to this period as the "Look, Ma, no hands!" era.

1.3.3 A does of reality (1966-1973)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

In almost all cases these early systems failed on more difficult problems.
The illusion of unlimited computational power was not confined to problem-solving programs.

1.3.4 Expert systems (1969-1986)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The picture of problem solving that had arisen during the first decade of AI 
research was of a general-purpose search mechanism trying to string together 
elementary reasoning steps to find complete solutions.
Such approaches have been called **weak methods**.
The alternative to weak methods is to use more powerful, domain-specific 
knowledge that allows larger reasoning steps and can more easily handle 
typically occurring cases in narrow areas of expertise.

1.3.5 The return of neural networks (1986-present)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

In the mid-1980s at least four different groups reinvented the 
**back-propagation** learning algorithm first developed in the early 1960s.

1.3.6 Probabilistic reasoning and machine learning (1987-present)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

In the 1980s, approaches using **hidden Markov models** (HMMs) came to dominate the area.
Pearl’s development of **Bayesian networks** yielded a rigorous and efficient 
formalism for representing uncertain knowledge as well as practical algorithms 
for probabilistic reasoning.

1.3.7 Big data (2001-present)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Remarkable advances in computing power and the creation of the World Wide Web 
have facilitated the creation of very large data sets—a phenomenon sometimes 
known as **big data**.

1.3.8 Deep learning (2011-present)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The term **deep learning** refers to machine learning using multiple layers of simple, adjustable computing elements. 
Experiments were carried out with such networks as far back as the 1970s, and in 
the form of **convolutional neural networks** they found some success in 
handwritten digit recognition in the 1990s.

1.4 The Sate of the Art
-----------------------

**ROBOTIC VEHICLES**

**LEGGED LOCOMOTION**

**AUTONOMOUS PLANNING AND SCHEDULING**

**MACHINE TRANSLATION**

**SPEECH RECOGNITION**

**RECOMMENDATIONS**

**GAME PLAYING**

**IMAGE UNDERSTANDING**

**MEDICINE**

**CLIMATE SCIENCE**

1.5 Risks and Benefits of AI
----------------------------

**LETHAL AUTONOMOUS WEAPONS**

**SURVEILLANCE AND PERSUASION**

**BIASED DECISION MAKING**

**IMPACT ON EMPLOYMENT**

**SAFETY-CRITICAL APPLICATIONS**

**CYBERSECURITY**