<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [universal cover](../../../../../../universal-cover.md) of $S^1\times S^2$ is

$$
p:\mathbb R\times S^2\longrightarrow S^1\times S^2,
\qquad p(t,z)=(e^{2\pi it},z).
$$

Because $S^3$ is simply connected, any [continuous](../../../../../../continuous-function.md) map $f:S^3\to S^1\times S^2$ lifts to $\tilde f:S^3\to\mathbb R\times S^2$ after choosing a lift of one base point. The [lifting criterion for a covering space](../../../../../../lifting-criterion-for-a-covering-space.md) applies because $f_*\pi_1(S^3)=0$. Equivalently, path lifting defines the lift and simple connectedness makes its value independent of the chosen path.

The cover deformation retracts onto $\{0\}\times S^2$, so $H_3(\mathbb R\times S^2;\mathbb Z)=0$. Since $f=p\circ\tilde f$, functoriality of [homology](../../../../../../homology-split.md) gives

$$
f_*:H_3(S^3;\mathbb Z)\xrightarrow{\tilde f_*}
0\xrightarrow{p_*}H_3(S^1\times S^2;\mathbb Z).
$$

Therefore $\boxed{f_*=0\text{ and }\deg f=0}$, with the last equality using the oriented three-dimensional fundamental classes.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
