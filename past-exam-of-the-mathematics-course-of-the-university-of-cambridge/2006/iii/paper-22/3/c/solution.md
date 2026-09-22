<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By part (b), the [moduli space](../../../../../../moduli-space.md) is $M(T)=SU(2)^2/SU(2)$ under simultaneous conjugation. Regard $SU(2)$ as the [unit quaternions](../../../../../../unit-quaternion.md) and write

$$
A=a+u,\qquad B=b+v,\qquad
|u|^2=1-a^2,\quad |v|^2=1-b^2,
$$

with $u,v\in\mathbb R^3$. Conjugation rotates both imaginary vectors by the same element of $SO(3)$. Their lengths and inner product determine an orbit, even when one vector vanishes or the vectors are collinear: an isometry between the two spanned planes can be extended to an orientation-preserving rotation of $\mathbb R^3$. Thus complete invariants are

$$
(a,b,c),\qquad c=u\cdot v,\qquad
-1\leq a,b\leq1,\quad c^2\leq(1-a^2)(1-b^2).
$$

Every allowed triple is realized by a pair of vectors with the prescribed lengths and dot product. The induced continuous bijection from the compact quotient to this closed subset of $\mathbb R^3$ is a [homeomorphism](../../../../../../homeomorphism.md).

Let $U$ be the subset where $A\ne\pm1$, equivalently $-1<a<1$. It is open and dense because the excluded first holonomies can be approximated by noncentral ones. Rotate $u$ to the positive $i$ axis, so $A=a+\sqrt{1-a^2}\,i$. Its remaining stabilizer rotates the $j,k$ plane. If $B=b+t i+yj+zk$, the orbit is determined by $(b,t)$, and

$$
b^2+t^2\leq1,
$$

with the remaining radius $\sqrt{1-b^2-t^2}$. These coordinates give the corrected result

$$
\boxed{U\cong\overline{\mathbb D}\times(-1,1)
\cong\overline{\mathbb D}\times(0,1).}
$$

Continuity of the inverse follows by taking $y=\sqrt{1-b^2-t^2}$ and $z=0$ as a representative. The complement consists of $A=1$ and $A=-1$, separately. In either case conjugation classes of $B$ are parametrized by its real part $b\in[-1,1]$. Therefore **$M(T)\setminus U$ is two disjoint closed intervals**, as requested.

**The printed $S^2$ factor is incorrect: the factor must be a closed disk.** The stabilizer acts by conjugation, fixing the circle of quaternions $b+ti$; it is not the free Hopf circle action on $S^3$. To rule out a different choice of dense open set with the printed topology, we can also identify the whole space. Replace $c$ by $d=ab+c$. The invariant region becomes

$$
\mathcal C=\left\{(a,b,d):
\begin{pmatrix}1&a&b\\a&1&d\\b&d&1\end{pmatrix}\text{ is positive semidefinite}\right\}.
$$

These are the Gram matrices of the three unit vectors $1,A,B$ in $\mathbb R^4$. Conversely, a positive-semidefinite matrix of this form can be realized by such vectors, hence by the original quaternion data. The set $\mathcal C$ is compact and convex and contains the identity matrix as an interior point in its three coordinates. Radial parametrization of a convex body therefore identifies it with a closed three-ball. Thus

$$
\boxed{M(T)\cong\overline B^3.}
$$

This also agrees with Theorem 6.5 of [the primary character-variety paper](https://arxiv.org/pdf/0807.3317).

An open subset homeomorphic to the boundaryless three-manifold $S^2\times(0,1)$ cannot contain a boundary point of this closed ball. Otherwise a local chart, followed by inclusion into $\mathbb R^3$, would be a continuous injection from an open subset of $\mathbb R^3$ whose image contains a ball-boundary point while staying inside the closed ball, contradicting [invariance of domain](../../../../../../invariance-of-domain.md). Its complement would therefore contain the entire boundary sphere. But a sphere cannot embed in two disjoint intervals: its connected image would lie in one interval and be a nondegenerate compact interval, whose interior points disconnect it, unlike $S^2$. This proves that the literal printed pair of claims is impossible, and supplies the complete corrected [SU2 character variety of the punctured torus](../../../../../../su2-character-variety-of-the-punctured-torus.md) description.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
