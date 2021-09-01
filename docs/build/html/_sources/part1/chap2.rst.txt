Chapter 2 Intelligent Agents
============================



2.1 Agents and Environments
---------------------------

An **agent** is anything that can be viewed as perceiving its **environment** 
through **sensors** and acting upon that environment through **actuators**.

We use the term **percept** to refer to the content an agent’s sensors are perceiving. 
An agent’s **percept sequence** is the complete history of everything the agent has ever perceived. 
In general, *an agent’s choice of action at any given instant can depend on its* 
*built-in knowledge and on the entire percept sequence observed to date, but* 
*not on anything it hasn’t perceived*.
Mathematically speaking, we say that an agent’s behavior is described by the 
**agent function** that maps any given percept sequence to an action.

*Internally*, the agent function for an artificial agent will be implemented by an **agent program**. 
It is important to keep these two ideas distinct. 
The agent function is an abstract mathematical description; the agent program is 
a concrete implementation, running within some physical system.

2.2 Good Behavior: The Concept of Rationality
---------------------------------------------

A **rational agent** is one that does the right thing.

2.2.1 Performance measures
^^^^^^^^^^^^^^^^^^^^^^^^^^

Moral philosophy has developed several different notions of the “right thing,” 
but AI has generally stuck to one notion called **consequentialism**: we 
evaluate an agent’s behavior by its consequences.

This notion of desirability is captured by a **performance measure** that 
evaluates any given sequence of environment states.