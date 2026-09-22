<h1 id="1/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [inflow transport boundary condition](../../../../../../../inflow-transport-boundary-condition.md), the [weak formulation](../../../../../../../weak-formulation.md) is

$$
\int_0^\infty\!\int_0^\infty u(\varphi_t+a\varphi_x)\,dx\,dt+\int_0^\infty u_0(x)\varphi(0,x)\,dx+a\int_0^\infty f(t)\varphi(t,0)\,dt=0.
$$

Here $\varphi$ is a smooth compactly supported [test function](../../../../../../../test-function.md) on the closed quadrant. Put $z=x-at$ and $\psi(t,z)=\varphi(t,z+at)$. The transformed region is $t>\tau(z):=\max(0,-z/a)$. The formula in the preceding solution is $v(t,z)=b(z)$, with $b(z)=u_0(z)$ for $z\ge0$ and $b(z)=f(-z/a)$ for $z<0$. Consequently the first integral equals $-\int b(z)\psi(\tau(z),z)\,dz$. Its positive-$z$ portion cancels the initial integral; the substitution $z=-at$ in its negative-$z$ portion cancels the inflow integral, including the factor $a$. This proves weak existence for arbitrary bounded data without corner compatibility.

For uniqueness, subtract two [weak solutions](../../../../../../../weak-solution.md). Interior [test functions](../../../../../../../test-function.md) in these [characteristic coordinates](../../../../../../../characteristic-coordinate.md) give $\partial_t v=0$ distributionally, so $v(t,z)=b(z)$ on each vertical ray. This follows first on rectangles compactly contained in $t>\tau(z)$ using tensor [test functions](../../../../../../../test-function.md), and then on the whole region by overlapping rectangles. In the full [weak formulation](../../../../../../../weak-formulation.md) the remaining lower-boundary term is $-\int b(z)\psi(\tau(z),z)\,dz=0$. Arbitrary smooth traces supported separately on $z>0$ and $z<0$ force $b=0$ there. The single point $z=0$ has zero measure. Thus **the two-branch formula is the unique bounded weak solution**.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [1](../../../1.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
