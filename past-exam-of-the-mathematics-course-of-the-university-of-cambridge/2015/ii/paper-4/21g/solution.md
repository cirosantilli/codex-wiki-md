<h1 id="21g/solution">Solution</h1>

↑ **Parent:** [21G](../21g.md)

Regard complex matrices as a real vector space of dimension $2n^2$ and Hermitian matrices as a real vector space of dimension $n^2$. Set $F(A)=AA^*$. Its derivative is $DF_A(H)=HA^*+AH^*$. At a unitary $A$, any Hermitian $S$ is reached by $H=SA/2$. Hence $I$ is a [regular value](../../../../../regular-value.md), and the [regular level set theorem](../../../../../regular-level-set-theorem.md) makes $\mathrm U(n)=F^{-1}(I)$ a smooth real [manifold](../../../../../topological-manifold.md) of dimension $\boxed{n^2}$.

The [tangent space](../../../../../tangent-space.md) is the kernel of this derivative. Equivalently,

$$
\boxed{H\in T_A\mathrm U(n)\iff A^*H+H^*A=0\iff H=AK\text{ with }K^*=-K.}
$$

At $I$, therefore, $H$ is skew-Hermitian. The explicit [geodesic](../../../../../geodesic.md) with initial point $I$ and velocity $H$ is $\gamma(t)=e^{tH}$. The [matrix exponential](../../../../../matrix-exponential.md) is unitary because $e^{tH^*}e^{tH}=I$, and $\dot\gamma(0)=H$. Its acceleration is $\gamma H^2$. Since $H^2$ is Hermitian and every tangent vector at $\gamma$ is $\gamma K$ with $K$ skew-Hermitian, the induced real inner product satisfies

$$
\langle\gamma H^2,\gamma K\rangle=\operatorname{Re}\operatorname{tr}(H^2K^*)=0.
$$

Indeed the trace of a Hermitian matrix times a skew-Hermitian matrix is purely imaginary. Its acceleration is therefore always normal to the manifold, which is the [geodesic equation](../../../../../geodesic-equation.md) for an induced Euclidean metric. Diagonalizing $H=W\operatorname{diag}(i\lambda_j)W^*$ gives the equivalent explicit construction $W\operatorname{diag}(e^{it\lambda_j})W^*$.

## ↑ Ancestors (10)

1. [21G](../21g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
