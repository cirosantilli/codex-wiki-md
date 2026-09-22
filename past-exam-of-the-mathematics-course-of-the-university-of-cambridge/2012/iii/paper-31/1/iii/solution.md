<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose real [monic orthogonal polynomials](../../../../../../monic-orthogonal-polynomial.md) $p_j$ of degree $j$, $j=0,1,\ldots$, for $w(x)=x^a e^{-x}$ on $[0,\infty)$, and let

$$
h_j=\int_0^\infty p_j(x)^2w(x)\,dx,\qquad \phi_j(x)=h_j^{-1/2}p_j(x)\sqrt{w(x)}.
$$

Extend each $\phi_j$ by zero to negative $x$. The resulting [functions](../../../../../../function-split.md) form an [orthonormal set](../../../../../../orthonormal-set.md) in $L^2(\mathbb R,dx)$. Define the [orthogonal polynomial projection kernel](../../../../../../orthogonal-polynomial-projection-kernel.md)

$$
\boxed{K_m(x,y)=\sum_{j=0}^{m-1}\phi_j(x)\phi_j(y)=\sqrt{w(x)w(y)}\sum_{j=0}^{m-1}\frac{p_j(x)p_j(y)}{h_j}.}
$$

The formula on the right is for nonnegative arguments; the kernel is zero when either argument is negative. With $\Phi_{ij}=\phi_{j-1}(x_i)$, the kernel evaluation [matrix](../../../../../../matrix.md) is $\Phi\Phi^T$. By the [determinant](../../../../../../determinant.md) multiplication identity and the preceding monic basis change,

$$
\det[K_m(x_i,x_j)]_{i,j=1}^m=\frac{\prod_{i<j}(x_j-x_i)^2\prod_iw(x_i)}{\prod_{j=0}^{m-1}h_j}.
$$

Thus initially $\widehat c_m=c_m\prod_jh_j$.

Use the symmetric labelled [joint probability density](../../../../../../joint-probability-density.md) on the full orthant. Expanding the two copies of $\det\Phi$ into [permutations](../../../../../../permutation.md) and integrating all variables, [orthonormality](../../../../../../orthonormal-set.md) makes a term vanish unless the two [permutations](../../../../../../permutation.md) agree. Each of the $m!$ surviving terms integrates to $1$. Hence

$$
\boxed{f_m(x_1,\ldots,x_m)=\frac1{m!}\det[K_m(x_i,x_j)]_{i,j=1}^m,\qquad c_m=\frac1{m!\prod_{j=0}^{m-1}h_j}.}
$$

If the [eigenvalues](../../../../../../eigenvalue.md) are instead listed in increasing order on a single ordered chamber, that chamber's density is $m!$ times this symmetric density. We keep the full-orthant convention throughout.

An explicit choice is $p_j(x)=(-1)^j j!L_j^{(a)}(x)$ in terms of the [Generalized Laguerre polynomials](../../../../../../generalized-laguerre-polynomial.md). To verify the normalization independently, their [Rodrigues' formula](../../../../../../rodrigues-formula.md) gives

$$
p_j(x)=(-1)^j w(x)^{-1}\frac{d^j}{dx^j}(x^{a+j}e^{-x}).
$$

Integrating by parts $j$ times proves orthogonality to every lower-degree [polynomial](../../../../../../polynomial-split.md). The boundary terms vanish at zero and infinity for $a\geq0$. Taking the other factor to be $p_j$ and using $p_j^{(j)}=j!$ gives $h_j=j!\Gamma(a+j+1)$, where $\Gamma$ is the [Gamma function](../../../../../../gamma-function.md). The [Laguerre projection kernel](../../../../../../laguerre-projection-kernel.md) is therefore

$$
\boxed{K_m(x,y)=(xy)^{a/2}e^{-(x+y)/2}\sum_{j=0}^{m-1}\frac{j!}{\Gamma(a+j+1)}L_j^{(a)}(x)L_j^{(a)}(y)}
$$

for $x,y\geq0$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
