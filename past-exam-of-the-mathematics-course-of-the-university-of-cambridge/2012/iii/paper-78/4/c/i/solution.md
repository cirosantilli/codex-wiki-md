<h1 id="4/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $f,g\in L^2(0,1)$, interchange the integrals in the [inner product](../../../../../../../inner-product.md) of the [Volterra integration operator](../../../../../../../volterra-operator.md):

$$
\langle Af,g\rangle=\int_0^1\int_0^x f(t)\overline{g(x)}\,dt\,dx=\int_0^1f(t)\overline{\int_t^1g(x)\,dx}\,dt.
$$

Thus the [adjoint operator](../../../../../../../adjoint-operator.md) is $A^*g(t)=\int_t^1g(x)\,dx$. The triangular integration kernel is square-integrable, so $A$ is a [Hilbert-Schmidt operator](../../../../../../../hilbert-schmidt-operator.md) and hence a [compact operator](../../../../../../../compact-operator-split.md).

Set $a_n=(n-\tfrac12)\pi$ and $\sigma_n=1/a_n$. Direct integration gives

$$
Au_n(x)=\sqrt2\int_0^x\cos(a_nt)\,dt=\sigma_n\sqrt2\sin(a_nx)=\sigma_nv_n(x),
$$



$$
A^*v_n(x)=\sqrt2\int_x^1\sin(a_nt)\,dt=\sigma_n\sqrt2\cos(a_nx)=\sigma_nu_n(x),
$$

since $\cos a_n=0$. Product-to-sum identities give $\langle u_n,u_j\rangle=\langle v_n,v_j\rangle=\delta_{nj}$. For completeness, $g=A^*Af$ satisfies $g''=-f$, $g'(0)=0$, $g(1)=0$. The associated [Sturm-Liouville problem](../../../../../../../sturm-liouville-problem.md) has precisely the complete mixed-boundary cosine basis $u_n$; $AA^*$ gives the mixed-boundary sine basis $v_n$, with $v_n(0)=0$, $v_n'(1)=0$. Both $A$ and $A^*$ are injective, since differentiation of their zero integrals recovers their inputs. Their singular vectors therefore cover the entire two [Hilbert spaces](../../../../../../../hilbert-space-split.md), rather than just proper orthogonal complements.

**The given functions form the complete [singular value system](../../../../../../../singular-system-of-a-compact-operator.md), with $\sigma_n=2/((2n-1)\pi)$.** This is the [mixed-boundary singular system of the Volterra operator](../../../../../../../mixed-boundary-singular-system-of-the-volterra-operator.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 78](../../../../paper-78-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
