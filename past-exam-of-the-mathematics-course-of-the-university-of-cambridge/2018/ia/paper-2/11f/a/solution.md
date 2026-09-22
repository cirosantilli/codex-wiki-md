<h1 id="11f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $q_n=\mathbb P(X_n=0)$ for a [Galton-Watson process](../../../../../../galton-watson-process.md) starting from one ancestor. Conditional on $X_1=k$, extinction by generation $n+1$ requires $k$ independent descendant processes to be extinct by generation $n$, so

$$
q_{n+1}=F(q_n),\qquad q_0=0.
$$

Because zero is absorbing, $q_n\uparrow q$, the eventual extinction probability, and continuity gives $q=F(q)$. If $r\geq0$ is any fixed point, monotonicity of $F$ and $q_0\leq r$ give $q_n\leq r$ inductively. Thus $q$ is the smallest nonnegative fixed point.

Here $F(s)=s/4+3s^3/4$. Every individual has at least one child, so **$q=0$**. The offspring mean is $F'(1)=5/2$, hence

$$
\boxed{\mathbb EX_n=(5/2)^n.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
