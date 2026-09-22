<h1 id="9f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Given $Z_i=n$, the probability of no friendship among people sharing day $i$ is $2^{-n(n-1)/2}$. The day counts are independent, so

$$
\boxed{\mathbb P(\text{no matching friend pair})
=\left[
 e^{-1}\sum_{n=0}^\infty\frac{2^{-n(n-1)/2}}{n!}
\right]^{365}
=\left(\frac{2+C}{e}\right)^{365}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
