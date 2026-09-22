<h1 id="m5/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $t>0$, apply [Markov's inequality](../../../../../markov-s-inequality.md) to the nonnegative random variable $e^{tS_n}$. The exponential is then increasing, so

$$
\mathbb P(S_n\geq an)\leq e^{-tan}\mathbb E[e^{tS_n}]
\leq\exp\left[n\left(\frac{t^2}{2}-at\right)\right].
$$

At $t=0$ the right side is one. For $t<0$ it exceeds one because $a>0$, so the same displayed bound remains true trivially; the upper-tail Markov argument itself uses $t>0$.

Complete the square $t^2/2-at=(t-a)^2/2-a^2/2$. Choosing $t=a$ gives the strongest bound from this family, $\mathbb P(S_n\geq an)\leq e^{-na^2/2}$. The distribution is symmetric, so the same bound holds for $S_n\leq-an$. A union bound gives

$$
\boxed{\mathbb P(|S_n|\geq an)\leq2e^{-na^2/2}.}
$$

One may also cap this at one. Its exponential decay is stronger than the [polynomial](../../../../../polynomial-split.md) Chebyshev bound for fixed $a>0$ and large $n$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [M5](../../../m5.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
