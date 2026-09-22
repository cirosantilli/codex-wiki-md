# Accessible state of a Markov chain

↑ **Parent:** [Communicating class](communicating-class.md)

For a finite, time-homogeneous [Discrete-time Markov chain](discrete-time-markov-chain.md), state $j$ is accessible from $i$ when some finite path of positive [transition probabilities](transition-probability.md) leads from $i$ to $j$. Equivalently, $(P^n)_{ij}>0$ for some $n\geq0$, allowing a zero-step path when $i=j$. Accessibility is reflexive and transitive; [communicating states](communicating-states.md) require accessibility in both directions. See [Ward Whitt's lecture notes of September 24, 2013, classification of states](https://www.columbia.edu/~ww2040/3106F13/lect0924.pdf). In the closed-cycle example in [communicating class](communicating-class.md), $s\to c_2$ despite $P_{s,c_2}=0$, because $P_{s,c_1}P_{c_1,c_2}=1/4>0$; $c_2\to s$ fails at every step count.

## ↑ Ancestors (8)

1. [Communicating class](communicating-class.md)
2. [Markov chain](markov-chain-split.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Communicating class](communicating-class.md)
