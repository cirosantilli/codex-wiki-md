<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Seek an [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) in the invariant coordinate plane $z=0$ with $x,y\ne0$. Put $U=x^2$ and $W=y^2$. The two nonzero-component equations are

$$
\mu=a(U+W)+cW,\qquad \mu=a(U+W)-eU.
$$

Subtracting gives $eU+cW=0$, so positive $U,W$ require $ce<0$. With $D=a(c-e)-ce$, the solutions are

$$
\boxed{x^2=\frac{\mu c}{D},\qquad y^2=-\frac{\mu e}{D},\qquad z=0.}
$$

They are actual additional [equilibria](../../../../../../equilibrium-point-of-a-dynamical-system.md) when $D$ has the sign of $c$; the signs of $x,y$ are independently free, and cyclic permutation supplies the other two coordinate planes. For example, $a=\mu=c=1$, $e=-1$ gives $D=3$ and $x^2=y^2=1/3$. Thus **additional two-coordinate [equilibria](../../../../../../equilibrium-point-of-a-dynamical-system.md) do exist for suitable opposite-sign cross-couplings**. The inequality $ce<0$ is necessary for this type, but without the positivity conditions on the displayed denominator it need not be sufficient for every coefficient choice.

The isotropy of a generic such point is just $\langle\kappa_z\rangle$, whose fixed-point subspace is two-dimensional. The [Equivariant branching lemma](../../../../../../equivariant-branching-lemma.md) guarantees axial branches with one-dimensional fixed spaces; it does not rule out these lower-symmetry branches. Their existence therefore gives no contradiction.

At fixed $\mu>0$, letting $e$ cross zero with $c\ne0$ sends $x^2\to\mu/a$, $y^2\to0$: the new pair of opposite-$y$ branches meets an axis [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md). Its $y$ [eigenvalue](../../../../../../eigenvalue.md) is $e\mu/a$, so this is a secondary [symmetry-forced pitchfork bifurcation](../../../../../../symmetry-forced-pitchfork-bifurcation.md). Similarly, as $c$ crosses zero with $e\ne0$, the branches meet the $y$ axis, whose $x$ [eigenvalue](../../../../../../eigenvalue.md) is $-c\mu/a$. The cubic formula gives $y^2\sim-\mu e/(ac)$ near the first crossing, and $x^2\sim-\mu c/(ae)$ near the second. Reflections force the two signs of the newly nonzero coordinate, while cyclic symmetry gives the corresponding pitchforks on the other axes. The simultaneous $c=e=0$ case is degenerate and is not a generic single-parameter pitchfork.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
