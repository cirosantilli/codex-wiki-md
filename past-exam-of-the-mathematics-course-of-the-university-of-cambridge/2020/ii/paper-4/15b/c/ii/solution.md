<h1 id="15b/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [harmonic oscillator](../../../../../../../simple-harmonic-motion.md) Hamiltonian $H=(q^2+p^2)/2$,

$$
q(t)=Q\cos t+P\sin t,
\qquad
p(t)=P\cos t-Q\sin t.
$$

This rotation preserves the [symplectic form](../../../../../../../symplectic-form.md) $dq\wedge dp$, so it is a [canonical transformation](../../../../../../../canonical-transformation.md) for every $t$. Where $\cos t\neq0$, solving for the initial variables gives

$$
Q=q\sec t-P\tan t,
\qquad
p=P\sec t-q\tan t,
$$

and hence the type-2 generator

$$
\boxed{F_2(q,P,t)=qP\sec t-\frac12(q^2+P^2)\tan t}.
$$

Its derivatives give the displayed transformation and $H+\partial_tF_2=0$. At $\cos t=0$ the canonical rotation remains perfectly regular, but its projection to $(q,P)$ is singular, so no type-2 generating function in those variables exists there; another generating-function chart covers those isolated times.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [15B](../../../15b.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
