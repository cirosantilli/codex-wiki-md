<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At state $r$, urn 1 has $r$ red and $n-r$ blue balls, while urn 2 has $n-r$ red and $r$ blue balls. Conditional on the state, the two choices are [independent](../../../../../../independent-random-variables.md), each assigning [probability](../../../../../../probability.md) $1/n$ to every ball. A red–blue exchange decreases $r$; a blue–red exchange increases it; equal colours leave it unchanged. Thus the [conditional probability mass function](../../../../../../conditional-probability-mass-function.md) is

$$
\boxed{\mathbb P(R_{k+1}=s\mid R_k=r)=
\begin{cases}
r^2/n^2,&s=r-1,\\
2r(n-r)/n^2,&s=r,\\
(n-r)^2/n^2,&s=r+1,\\
0,&\text{otherwise}.
\end{cases}}
$$

The three numerators sum to $n^2$. At $r=0$ or $n$, the outward transition has probability zero. These are the transitions of the [Bernoulli-Laplace diffusion model](../../../../../../bernoulli-laplace-diffusion-model.md). The displayed formula is a transition kernel on every state; a literal conditional probability at a particular time requires the conditioning event to have positive probability.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Discrete mathematics, probability and continuous mathematics](../../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
