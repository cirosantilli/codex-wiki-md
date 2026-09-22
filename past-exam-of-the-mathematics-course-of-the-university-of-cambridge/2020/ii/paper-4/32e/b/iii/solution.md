<h1 id="32e/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The map $F$ itself has a horseshoe only for $\mu=2$. Indeed, its [Lipschitz constant](../../../../../../../lipschitz-constant.md) is $\mu$. If two intervals $J_0,J_1$ form a horseshoe and their convex hull has length $L$, then

$$
L\leq\mu|J_i|\quad(i=0,1),
\qquad
|J_0|+|J_1|\leq L,
$$

which forces $\mu\geq2$. At $\mu=2$, take $J=(-1,1)$, $K_0=(-1,0)$ and $K_1=(0,1)$; both $K_i$ map onto $J$.

The [Lipschitz constant](../../../../../../../lipschitz-constant.md) of $F^2$ is $\mu^2$, so the same length argument makes $\mu\geq\sqrt2$ necessary for an $F^2$ horseshoe. It is sufficient. Put

$$
a=\frac1{1+\mu},\qquad b=\frac{\mu+2}{\mu(1+\mu)}.
$$

For $\mu\geq\sqrt2$, one has $a<1/\mu\leq b\leq1$. With

$$
J=(a,1),\qquad K_0=(a,1/\mu),\qquad K_1=(1/\mu,b),
$$

the two relevant monotone branches satisfy

$$
F^2(a)=F^2(b)=a,
\qquad
F^2(1/\mu)=1.
$$

Thus $K_0,K_1\subset J$ are disjoint and $F^2(K_0)=F^2(K_1)=J$. Therefore

$$
\boxed{F\text{ has a horseshoe iff }\mu=2,\qquad F^2\text{ has one iff }\mu\geq\sqrt2}.
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [32E](../../../32e.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
