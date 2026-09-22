<h1 id="34b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With the convention in the question,

$$
T_r=\exp\left(\frac i\hbar r\cdot p\right)
$$

acts as

$$
(T_r\psi)(x)=\psi(x+r).
$$

Although $V(x+r)=V(x)$ for $r\in\Lambda$, the vector potential changes by

$$
A(x+r)=A(x)+\frac12B\times r.
$$

Consequently

$$
T_rHT_r^{-1}
=\frac1{2m}[p-eA(x+r)]^2+V(x)
\ne H
$$

for a nonzero magnetic field in general.

Now let $K=p+eA$. Since

$$
r\cdot K=-i\hbar r\cdot\nabla
+\frac e2r\cdot(B\times x)
$$

and the derivative in the $r$ direction annihilates  
$r\cdot(B\times x)$, the two terms in its exponential commute. The [magnetic translation operator](../../../../../../magnetic-translation.md) therefore acts as

$$
\boxed{
(\mathcal T_r\psi)(x)
=\exp\left(\frac{ie}{2\hbar}
r\cdot(B\times x)\right)\psi(x+r)}.
$$

Part (a) gives $[K_i,p_j-eA_j]=0$, so $\mathcal T_r$ commutes with the kinetic term. Its phase commutes with $V$, while its translation sends $V(x)$ to $V(x+r)=V(x)$. Hence

$$
\boxed{[\mathcal T_r,H]=0\qquad(r\in\Lambda)}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [34B](../../34b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
