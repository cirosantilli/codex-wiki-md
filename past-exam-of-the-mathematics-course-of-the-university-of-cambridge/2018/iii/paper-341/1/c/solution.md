<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Only $-1<\alpha<1$ needs consideration. On the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md), the [amplification polynomial of a multistep method](../../../../../../amplification-polynomial-of-a-multistep-method.md) is $P_z(w)=\rho(w)-z\sigma(w)$, where $z=h\lambda$. [A-stability](../../../../../../a-stability.md) requires all amplification roots to have modulus at most one for every $\operatorname{Re}z\leq0$, with simple unit-modulus roots.

Choose the negative real value $z=-2/(1-\alpha)$. The leading coefficient of $P_z$ is

$$
1-z(\alpha-1)=-1,
$$

whereas $P_z(1)=-z\sigma(1)=4>0$. Hence $P_z(w)\to-\infty$ as real $w\to+\infty$. The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) supplies a real amplification root $w>1$, so this negative test value is unstable. Therefore

$$
\boxed{\text{no parameter makes the method both convergent and A-stable}.}
$$

This is a direct [absolute stability](../../../../../../linear-stability-domain.md) obstruction, independent of the [Second Dahlquist barrier](../../../../../../second-dahlquist-barrier.md), which by itself would not rule out the convergent second-order members.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
