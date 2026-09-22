<h1 id="9/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For $1\leq i\leq k$, the success [probability](../../../../../../probability.md) is $i/k>0$, and the definition of [conditional expectation](../../../../../../conditional-expectation.md) on an [event](../../../../../../event.md) gives

$$
\mathbb E_i[X\mid J=1]
=\frac{\mathbb E_i[X\mathbf1_{\{J=1\}}]}{\mathbb P_i(J=1)}
=\frac{i(k^2-i^2)/(3k)}{i/k}.
$$

Therefore

$$
\boxed{\mathbb E_i[X\mid\text{reach }k]=\frac{k^2-i^2}{3}\text{ minutes}.}
$$

At $i=k$ the value is zero because the trial has already ended. At the left absorbing state $i=0$, conditioning on success would be undefined because it has zero [probability](../../../../../../probability.md). The formula concerns the successful trajectories, so it need not equal the unconditional mean $i(k-i)$.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
