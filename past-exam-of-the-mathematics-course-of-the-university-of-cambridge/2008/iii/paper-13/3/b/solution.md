<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $u_1=Tv_1$ and $u_2=Tv_2$, linearity of the weak equation makes $\alpha u_1+\beta u_2$ solve the equation with forcing $\alpha v_1+\beta v_2$. Uniqueness therefore gives $T(\alpha v_1+\beta v_2)=\alpha Tv_1+\beta Tv_2$.

Test the equation for $u=Tv$ with $u$ itself. The [Poincaré inequality](../../../../../../poincare-inequality.md) yields

$$
\|Du\|_2^2=-\int vu\leq\|v\|_2\|u\|_2\leq C_P\|v\|_2\|Du\|_2.
$$

If the [gradient](../../../../../../gradient.md) norm is nonzero, divide by it; if it is zero, Poincare gives $u=0$ and the estimate is automatic. In either case

$$
\boxed{\|Tv\|_{W^{1,2}}\leq C_P\sqrt{1+C_P^2}\,\|v\|_2.}
$$

Hence $T:L^2(\Omega)\to W_0^{1,2}(\Omega)$ is a [bounded linear operator](../../../../../../continuous-linear-operator.md). Notice that the energy identity has a minus sign, so $\langle Tv,v\rangle=-\|D(Tv)\|_2^2\leq0$. Testing the equations for $Tv$ and $Tz$ against each other gives $\langle Tv,z\rangle=-\int D(Tv)\cdot D(Tz)=\langle v,Tz\rangle$. Thus the bounded Dirichlet inverse is a negative [self-adjoint operator](../../../../../../self-adjoint-operator.md) on $L^2$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
