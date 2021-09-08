Chapter 3 Solving Problems by Searching
=======================================

When the correct action to take is not immediately obvious, an agent may need to 
*plan ahead*: to consider a *sequence* of actions that form a path to a goal 
state. 
Such an agent is called a **problem-solving agent**, and the computational process it undertakes is called **search**.

Problem-solving agents use **atomic** representations, that is, states of the 
world are considered as wholes, with no internal structure visible to the
problem-solving algorithms. 
Agents that use **factored** or **structured** representations of states are called **planning agents**.

We distinguish between **informed** algorithms, in which the agent can estimate 
how far it is from the goal, and **uninformed** algorithms, where no such 
estimate is available.

3.1 Problem-Solving Agents
--------------------------

If the agent has no additional information—that is, if the environment is 
**unknown**—then the agent can do no better than to execute one of the actions 
at random.
For now, we assume that our agents always have access to information about the world.
With that information, the agent can follow this four-phase problem-solving process:

* **GOAL FORMULATION**: Goals organize behavior by limiting the objectives and hence the actions to be considered.

* **PROBLEM FORMULATION**: The agent devises a description of the states and 
  actions necessary to reach the goal—an abstract model of the relevant part of 
  the world.

* **SEARCH**: Before taking any action in the real world, the agent simulates 
  sequences of actions in its model, searching until it finds a sequence of 
  actions that reaches the goal.
  Such a sequence is called a **solution**.

* **EXECUTION**: The agent can now execute the actions in the solution, one at a time.

It is an important property that in a fully observable, deterministic, known 
environment, *the solution to any problem is a fixed sequence of actions*.
The **open-loop** system means that ignoring the percepts breaks the loop between agent and environment.
If there is a chance that the model is incorrect, or the environment is 
nondeterministic, then the agent would be safer using a **closed-loop** approach 
that monitors the percepts.

In partially observable or nondeterministic environments, a solution would be a 
branching strategy that recommends different future actions depending on what 
percepts arrive.

3.1.1 Search problems and solutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

A search **problem** can be defined formally as follows:

* A set of possible **states** that the environment can be in. 
  We call this the **state space**.

* The **initial state** that the agent starts in.

* A set of one or more **goal states**.
  We can account for all three of these possibilities by specifying an :math:`Is\-Goal` method for a problem.

* The **actions** available to the agent.
  Given a state :math:`s`, :math:`Actions(s)` returns a finite set of 
  actions that can be executed in :math:`s`.
  We say that each of these actions is **applicable** in :math:`s`.

* A **transition model**, which describes what each action does.
  :math:`Result(s,a)` returns the state that results from doing action :math:`a` in state :math:`s`.

* An **action cost function**, denote by :math:`Action\-Cost(s,a,s\pr)` when we 
  are programming or :math:`c(s,a,s\pr)` when we are doing math, that gives the
  numeric cost of applying action :math:`a` in state :math:`s` to reach state
  :math:`s\pr`.

A sequence of actions forms a **path**, and a **solution** is a path from the 
initial state to a goal state. 
We assume that action costs are additive; that is, the total cost of a path is 
the sum of the individual action costs. 
An **optimal solution** has the lowest path cost among all solutions.

The state space can be represented as a **graph** in which the vertices are 
states and the directed edges between them are actions.

3.1.2 Formulating problems
^^^^^^^^^^^^^^^^^^^^^^^^^^

The process of removing detail from a representation is called **abstraction**.
The abstraction is *valid* if we can elaborate any abstract solution into a 
solution in the more detailed world.
The abstraction is *useful* if carrying out each of the actions in the solution 
is easier than the original problem.
