<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $W$ be the [event](../../../../../../event.md) that $H$ wins, and $F$ the [event](../../../../../../event.md) that his first toss is a tail. For a nontrivial starting state $1\le i\le n-1$, a first tail has [probability](../../../../../../probability.md) $1/2$ and changes his holding to $i-1$. By the [chain rule for probabilities](../../../../../../chain-rule-for-probabilities.md),

$$
\mathbb P(F\cap W)=\frac12p_{i-1}=\frac{i-1}{2n}.
$$

Since $\mathbb P(W)=i/n>0$, the definition of [conditional probability](../../../../../../conditional-probability.md) gives

$$
\boxed{\mathbb P(F\mid W)=\frac{i-1}{2i}.}
$$

In particular, when $i=1$, losing the first coin would end the game in defeat, so the conditional answer is zero. At $i=0$ conditioning on victory is undefined, while at $i=n$ the game has already ended and no first toss occurs.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Calculus, probability, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../../calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
5. [2003](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
