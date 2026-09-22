<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $x\ne0$, the [Strong Markov property](../../../../../../strong-markov-property.md) at the first step gives the discrete mean-value identity

$$
v(x)=\frac16\sum_{|e|=1}v(x+e).
$$

At $x=0$, $v(0)=1$ while the same average is at most one. Thus $v$ is a bounded superharmonic function on $\mathbb Z^3$. Conditioning on the [natural filtration](../../../../../../natural-filtration.md) and using the one-step [Markov property](../../../../../../markov-property.md) gives

$$
\mathbb E[v(X_{n+1})\mid\mathcal F_n]
=\frac16\sum_{|e|=1}v(X_n+e)
\leq v(X_n).
$$

**Therefore $(v(X_n))$ is a nonnegative [supermartingale](../../../../../../supermartingale.md).**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
