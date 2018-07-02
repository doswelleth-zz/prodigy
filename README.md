![prodigylogo](https://user-images.githubusercontent.com/25995735/42149806-a709141a-7da5-11e8-83ae-6bb1a4c006f3.png)


## Vision

    a voluntary world for learning, free markets, and peaceful negotiations

## Mission

    a generation of highly educated and independently wealthy young people

<hr>

## Prodigy
### a peer-to-peer electronic contract system

##### David Oliver Doswell

#### Abstract

Prodigy is a crowdsourcing platform for solving problems. The project uses [discrete log contracts](https://adiabat.github.io/dlc.pdf) on the Bitcoin network to settle the resulting solution. 

Prodigy is a non-cooperative single player game made up of two counterparties: **random players** and **random students**.

Random players design problems for students to solve in exchange for bitcoins. To initialize a contract, each party stakes an equal amount of bitcoins from their personal wallets. This amount is denominated in satoshis, the smallest unit of a bitcoin. 

When a student answers a question correctly, the contract executes and the student receives the random player’s stake. When a student gets the answer wrong, the contract executes and the student loses their stake to the random player.

Each contract has a different value. The harder the problem, the higher the value of the contract and potentially the more satoshis a student can earn. 

Players should be anonymous. Problems that are considered valuable problems by students and fellow players receive the most visibility on a public, corresponding peer-to-peer website. 

This ensures the most potentially important problems get worked on. Contracts are associated by **Groups** under different STEAM-related subjects. 

We expect students around the world to work together to solve problems as random players design them.

<br>

#### Initialization

I am interested in a world where a random person initializes a discrete log contract in the form of a problem that may be solved by another random person in exchange for satoshis.

The problem is a user interface such as 

    “The Sistine Chapel stands on the foundation of what older chapel?" 
    
or 

    “What control valve actuator converts energy into mechanical motion?” 
    

The rigor of the problem is associated with the price of the contract and decided by a random player, the contract initializer.

Prodigy’s problems are STEAM (science, technology, engineering, art, mathematics) focused and have objective answers. In cases where the answer is objective but multitudinous, acceptable answers are scripted in the form of multiple choice.

These answers should be structured in the contract in such a way that the student gets the answer right if the answer is factually correct.

For instance, if the question is “Give an example of a runtime environment for modern web applications,” the answer may be “Javascript Runtime Environment (JRE)” or “.NET Runtime.” Both answers are correct.

However, it is not in the interest of a random player to structure questions in such ways, as the opportunity for students to solve them increases to O(log)n.

A random player's goal isn’t to stump students. The goal is to get students to think, and to be rewarded for thinking and working through problems.

Students are encouraged to work together. Parents are even expected to help students solve problems in exchange for satoshis. For this reason, I encourage students to host their own wallets and control their private keys.

<br>

The complexity of creating an honest game here will not be lost on the astute reader: [principal-agent problem](https://en.wikipedia.org/wiki/Principal–agent_problem).

How might we prevent random players from designing contracts with incorrect answers and stealing satoshis?

Prodigy selects an additional random player, a non-interactive oracle who I call a **random party**, to confirm the random player's answer. 

The random party does not see the answer of a contract: a minimized version of the contract is revealed to randomized parties, namely the contract's title, its problem and answer fields.

The title and problem fields are explicit. The answer field is blank.

The random party owns a one-time [signature](https://en.wikipedia.org/wiki/Digital_signature) which is used to sign the contract by either the student or player when the answer is revealed. This is done by the random party being tasked to solve the problem themselves in exchange for 1% of the contract price.

Random parties risk nothing to solve problems so they earn less. The incentive is satoshis earned for problems solved. 

This ensures initialized contracts get executed and settled.

Players and parties are notably unknown to one another and are self-interestedly invested in settling contracts. 

Random parties may browse the parties section of the website and inspect uninitialized contracts, and work on them for a fee of 1% of a given contract's price.

Our random player must **conform to the contract** to prepare it for initialization by a random party, after a student accepts the contract and submits an answer to its problem:

    1. Problems are verifiable facts reasoned from axioms, as humans understand them.
  
    2. Problems are explicitly phrased in a question/answer format (e.g. What is water’s chemical formula? // H2O)
    
    3. Problems are solvable.
   
    4. A Random Party has been compensated 1% of the contract by the contract initializer for confirming the answer to the contract's problem.
    
    5. A Random Player has paid the initialization threshold of the contract, 1% of the contract’s value, for participating in a free market.


I call this process conforming to the contract.
