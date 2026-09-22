<h1 id="29e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For smooth periodic initial data, Fourier expansion reduces the equation to $\dot{\widehat u}(m,t)=-(1+m^2)\widehat u(m,t)$. Therefore define the [Fourier multiplier](../../../../../../fourier-multiplier.md) solution operators by

$$
\widehat{S(t)u_0}(m)=e^{-(1+m^2)t}\widehat u_0(m).
$$

Their [Sobolev norm](../../../../../../sobolev-norm.md) satisfies $\|S(t)u_0\|_{H^s}^2\leq e^{-2t}\|u_0\|_{H^s}^2\leq\|u_0\|_{H^s}^2$, so they extend to [contractive linear operators](../../../../../../contractive-linear-operator.md) on $H^s_{\rm per}$. Multiplication of the Fourier factors gives $S(t+s)=S(t)S(s)$ and $S(0)=I$. Finally

$$
\|S(t)u-u\|_{H^s}^2=\sum_m(1+m^2)^s|e^{-(1+m^2)t}-1|^2|\widehat u(m)|^2\to0
$$

by [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md), dominated by four times the summable norm terms. This proves a **strongly continuous contraction semigroup** for every requested $s$; the semigroup property extends continuity from zero to other times. For smooth data, termwise derivatives converge and recover the original [Cauchy problem for a partial differential equation](../../../../../../cauchy-problem.md) uniquely.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [29E](../../29e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
