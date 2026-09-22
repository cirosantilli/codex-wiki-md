<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The assertion about all $H_0^1(U)\cap H^k(U)$ is false as printed in the original PDF. Take $U=(0,\pi)$, $L=-d^2/dx^2$, and $u=x(\pi-x)$. This is a nonzero smooth Dirichlet function, but $Lu=2$ and $L^2u=0$. In particular

$$
\boxed{((u,u))_4=\|L^2u\|_2^2=0\quad\text{although }u\ne0.}
$$

Already at $k=3$, $B[Lu,Lu]$ is not defined on its stipulated domain, because $Lu=2\notin H_0^1$. Extending $B$ to $H^1$ for this example would give zero, not an [inner product](../../../../../../../inner-product.md). Additional boundary conditions are essential.

The corrected spaces are the [Sobolev domains of powers of an elliptic Dirichlet operator](../../../../../../../sobolev-domains-of-powers-of-an-elliptic-dirichlet-operator.md). Let $A_D$ be the [Dirichlet realization of an elliptic operator](../../../../../../../dirichlet-realization-of-an-elliptic-operator.md), and set

$$
\boxed{X_0=L^2(U),\qquad
X_k=\left\{u\in H^k(U):T(L^ju)=0,
\quad0\leq j\leq\left\lfloor\frac{k-1}{2}\right\rfloor\right\}\quad(k\geq1).}
$$

In particular $X_1=H_0^1$, $X_2=H^2\cap H_0^1$, and $X_3$ also requires $T(Lu)=0$. The formulas in the question define [inner products](../../../../../../../inner-product.md) on these spaces.

Here is the norm-equivalence proof on the corrected domains. The base cases are the $L^2$ [inner product](../../../../../../../inner-product.md) at $k=0$ and part (i) at $k=1$. Standard Dirichlet [elliptic regularity](../../../../../../../elliptic-regularity.md), together with invertibility from the [Lax-Milgram theorem](../../../../../../../lax-milgram-theorem.md), gives for every integer $r\geq0$

$$
\|u\|_{H^{r+2}}\leq C_r\|Lu\|_{H^r},\qquad
\|Lu\|_{H^r}\leq C'_r\|u\|_{H^{r+2}}.
$$

The first estimate applies when $Tu=0$; invertibility absorbs the usual lower-order $L^2$ term. Moreover, $A_D:X_{r+2}\to X_r$ is an isomorphism. To see surjectivity, solve $Lu=f$ with zero Dirichlet trace for $f\in X_r$; regularity gives $u\in H^{r+2}$, and $T(L^ju)=T(L^{j-1}f)=0$ for each further required trace. The formulas satisfy

$$
((u,u))_{r+2}=((Lu,Lu))_r.
$$

Induction therefore gives

$$
\boxed{c_k\|u\|_{H^k}^2\leq((u,u))_k\leq C_k\|u\|_{H^k}^2\qquad(u\in X_k).}
$$

Injectivity of each iterate of $A_D$ gives positive definiteness. These spaces are $D(A_D^{k/2})$; the [spectral characterization of elliptic Dirichlet domains](../../../../../../../spectral-characterization-of-elliptic-dirichlet-domains.md) in the next part makes the half-powers precise. On the paper's uncorrected spaces the claim is valid at $k=0,1,2$, but fails in general beyond them.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
