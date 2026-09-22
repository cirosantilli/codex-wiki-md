<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Normalization makes the derivative of the additive $1$ in $\delta F/\delta P=V+\log P+1$ vanish. Using $\dot P=-\nabla\cdot J$, the no-flux boundary condition, and integration by parts gives

$$
\dot F=\int(V+\log P+1)(-\nabla\cdot J)\,dx
=\int\nabla(V+\log P)\cdot J\,dx.
$$

Substituting the gradient current,

$$
\boxed{\dot F=-\int P\,
\nabla(V+\log P)^TD\nabla(V+\log P)\,dx\leq0}.
$$

Positive definiteness makes equality possible only when $\nabla(V+\log P)=0$, equivalently $J=0$. Thus $F$ is a strict [Fokker--Planck free-energy functional](../../../../../../../fokker-planck-free-energy-functional.md) away from stationarity.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 353](../../../../paper-353-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
