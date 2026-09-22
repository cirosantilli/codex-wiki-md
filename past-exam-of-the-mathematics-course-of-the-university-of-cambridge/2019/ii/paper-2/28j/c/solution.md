<h1 id="28j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $N_+=\#\{i:Y_i>0\}$, $N_0=n-N_+$, and $a=1-e^{-\lambda}$. Ignoring factors independent of $\pi$, the likelihood is

$$
L(\pi)\propto\pi^{N_+}(1-a\pi)^{N_0}.
$$

The unconstrained critical point satisfies

$$
\frac{N_+}{\pi}-\frac{aN_0}{1-a\pi}=0,
$$

so, after enforcing $0\leq\pi\leq1$,

$$
\boxed{\widehat\pi_{\rm MLE}
=\min\left\{1,\frac{N_+}{n(1-e^{-\lambda})}\right\}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28J](../../28j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
