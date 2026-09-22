<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $t=e^{iz}$ and $|u\rangle=U|b\rangle=p|\xi\rangle+q|\phi\rangle$. The first factor in $G$ is

$$
(1-t)|u\rangle\langle u|-I.
$$

Since $R(\xi,z)|u\rangle=pt|\xi\rangle+q|\phi\rangle$, the coefficient of $|\phi\rangle$ in $G|u\rangle$ is

$$
q\left[(1-t)(p^2t+q^2)-1\right].
$$

It vanishes when

$$
(1-t)(p^2t+q^2)=1,
$$

or, using $p^2+q^2=1$,

$$
t+t^{-1}=\frac{p^2-q^2}{p^2}.
$$

A unit-modulus solution $t=e^{iz}$ exists exactly when the right-hand side lies in $[-2,2]$. The upper bound is automatic, while the lower bound is

$$
q^2\leq3p^2.
$$

Thus exact preparation by one application of $G$ is possible precisely when

$$
\boxed{p\geq\frac12}
\qquad\text{or equivalently}\qquad
\boxed{q\leq\sqrt3\,p}.
$$

One may choose $z$ so that $\cos z=(p^2-q^2)/(2p^2)$. Then $G|u\rangle$ has no $|\phi\rangle$ component and, by unitarity, equals $|\xi\rangle$ up to phase. This is a [phase-matched amplitude amplification](../../../../../../phase-matched-amplitude-amplification.md) step.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
