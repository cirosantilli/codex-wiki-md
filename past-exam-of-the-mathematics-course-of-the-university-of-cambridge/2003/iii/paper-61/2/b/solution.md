<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the specified time operator, $N_kE_k=3ikqE_k$, because the derivatives of $e^{i(kx+k^3t)}$ cancel between $\partial_t$ and $\partial_x^3$. Expanding the derivatives of $E_kA_k$ gives

$$
N_k(E_kA_k)=E_k\left[\int_L\frac{N_l\varphi(l)}{k+l}\,d\lambda(l)
+3ik\int_L\frac{M_l\varphi(l)}{k+l}\,d\lambda(l)-3kI_x\right].
$$

For completeness, the extra derivative terms before simplification are $3ikA_{k,xx}-3k^2A_{k,x}+3ikqA_k$. Substituting $\varphi_{xx}+q\varphi=M_l\varphi+il\varphi_x$ turns their derivative contribution into $-3k\int_L\varphi_x\,d\lambda=-3kI_x$.

Applying $N_k$ to the original [linear integral equation](../../../../../../linear-integral-equation.md) and using $I_x=-q$ cancels its right side. Thus

$$
\mathcal F(N\varphi)=3kE_k\int_L\frac{M_l\varphi(l)}{k+l}\,d\lambda(l).
$$

Part (a) gives $E_k\int_LM_l\varphi/(k+l)\,d\lambda=iM_k\varphi$. Therefore the exact requested identity is

$$
\boxed{\mathcal F(N\varphi)=3ikM\varphi.}
$$

Since $M\varphi=0$, this becomes homogeneous too. The same uniqueness argument gives $N\varphi=0$; it is not necessary to assume a separate uniqueness theorem for the differential time equation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
