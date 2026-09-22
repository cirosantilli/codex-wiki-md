<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In coordinates, write $\nabla_{\partial_i}\partial_\ell=\Gamma^k_{i\ell}\partial_k$. The [Riemannian curvature two-form](../../../../../../riemannian-curvature-two-form.md) is defined by the matrices

$$
R^k{}_{\ell ij}=\partial_i\Gamma^k_{j\ell}-\partial_j\Gamma^k_{i\ell}+\Gamma^k_{im}\Gamma^m_{j\ell}-\Gamma^k_{jm}\Gamma^m_{i\ell},
$$

with repeated indices summed. It assigns to $X,Y$ the fiberwise [endomorphism](../../../../../../endomorphism.md) $R(X,Y)$ whose entries are $R^k{}_{\ell ij}X^iY^j$. We can prove both coordinate independence and the required intrinsic identity as follows.

Define an operator on vector fields by $C(X,Y)=[\nabla_X,\nabla_Y]-\nabla_{[X,Y]}$. It is alternating in $X,Y$. For a [smooth function](../../../../../../smooth-function.md) $f$, the identities $[fX,Y]=f[X,Y]-Y(f)X$ and $\nabla_Y(fZ)=Y(f)Z+f\nabla_YZ$ give

$$
C(fX,Y)Z=fC(X,Y)Z;
$$

the two terms involving $Y(f)\nabla_XZ$ cancel. Alternation gives linearity over [smooth functions](../../../../../../smooth-function.md) in $Y$ as well. Expanding in the final argument yields

$$
C(X,Y)(fZ)=fC(X,Y)Z+\bigl(X(Yf)-Y(Xf)-[X,Y]f\bigr)Z=fC(X,Y)Z.
$$

Thus $C$ is tensorial in all three arguments, defining a global [endomorphism](../../../../../../endomorphism.md)-valued two-form.

For coordinate fields $\partial_i,\partial_j$, their bracket is zero. Expand $[\nabla_{\partial_i},\nabla_{\partial_j}]Z$ using $Z=Z^\ell\partial_\ell$. The second derivatives of $Z^\ell$ cancel by equality of mixed partials. The terms containing first derivatives of $Z^\ell$ cancel in pairs, and the remaining coefficient of $Z^\ell\partial_k$ is exactly $R^k{}_{\ell ij}$ above. Hence the coordinate definition equals the global tensor $C$, establishing coordinate independence and proving

$$
\boxed{R(X,Y)=[\nabla_X,\nabla_Y]-\nabla_{[X,Y]}.}
$$

This convention for the [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md) is valid for any [affine connection](../../../../../../affine-connection.md); in particular it applies to the [Levi-Civita connection](../../../../../../levi-civita-connection.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
