<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In a time-homogeneous [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md), a state's [holding time](../../../../../../holding-time.md) is exponential with rate equal to its total outgoing [transition intensity](../../../../../../transition-intensity.md). Converting the specified times to months gives

$$
a+b=\frac1{96},\qquad \frac a{a+b}=\frac12,\qquad c=\frac1{36}.
$$

The exit-type [probability](../../../../../../probability.md) follows by dividing its [transition intensity](../../../../../../transition-intensity.md) by the total exit rate. Therefore

$$
\boxed{a=b=\frac1{192},\quad c=\frac1{36},\quad Q=\begin{pmatrix}-1/96&1/192&1/192\\0&-1/36&1/36\\0&0&0\end{pmatrix}\ \text{month}^{-1}.}
$$

These are starting values for numerical estimation, rather than further observations or constraints on the final fitted rates.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
