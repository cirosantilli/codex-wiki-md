<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume the uniform estimate obtained in the geometric setting of part (i). The limit $g$ is bounded and continuous on the finite-alphabet symbolic space, so $p(x)=e^{g(E(x))}$ is measurable, positive, and bounded. Possible duplicate itineraries at partition endpoints do not affect its [Lebesgue measure](../../../../../../lebesgue-measure.md) density.

For a level-$n$ interval $\Delta_w$, the estimate gives

$$
e^{-C\lambda^{-n}}\frac{\nu(C_w)}{|\Delta_w|}
\leq p(x)\leq
e^{C\lambda^{-n}}\frac{\nu(C_w)}{|\Delta_w|},\qquad x\in\Delta_w.
$$

Fix a level-$m$ cylinder $C_v$ and subdivide its interval into level-$n$ intervals, with $n\geq m$. Integrating these inequalities and summing the subcylinder masses yields

$$
e^{-C\lambda^{-n}}\nu(C_v)\leq\int_{\Delta_v}p(x)\,dx\leq e^{C\lambda^{-n}}\nu(C_v).
$$

Letting $n\to\infty$ proves the exact equality $\int_{\Delta_v}p\,dx=\nu(C_v)$. The same argument on the entire interval gives $\int p=1$. Shrinking cylinders generate the interval Borel sigma-algebra, so the [Monotone class theorem](../../../../../../monotone-class-theorem.md) identifies $p(x)\,dx$ with the pushforward $\pi_*\nu$.

The symbolic [Gibbs measure](../../../../../../gibbs-measure.md) in this setting is shift invariant, and coding satisfies $T\circ\pi=\pi\circ\sigma$ away from the endpoint exceptions. These exceptions form a [null set](../../../../../../null-set.md): bounded $p$ and shrinking cylinders give zero mass to individual endpoints. Therefore, for every [Borel set](../../../../../../borel-set.md) $B$,

$$
(\pi_*\nu)(T^{-1}B)=\nu(\sigma^{-1}\pi^{-1}B)=\nu(\pi^{-1}B)=(\pi_*\nu)(B).
$$

Consequently

$$
\boxed{d\mu(x)=e^{g(E(x))}\,dx}
$$

is an absolutely continuous [invariant measure](../../../../../../invariant-measure.md). This implication uses the uniform cylinder estimate directly and does not rely on naming an invariance theorem in place of the requested argument.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
