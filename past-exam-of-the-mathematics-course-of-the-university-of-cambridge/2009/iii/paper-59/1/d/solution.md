<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First use a genuine simple [bivector](../../../../../../bivector.md) of the specified chirality, with spinor part $\phi^{AB}=\alpha^A\alpha^B$. It is a [exterior product](../../../../../../exterior-product.md): choose independent primed spinors $\rho^{A'},\sigma^{A'}$ and take $u^{AA'}=\alpha^A\rho^{A'}$, $v^{BB'}=\alpha^B\sigma^{B'}$. Their antisymmetric product is proportional to $w^{AA'BB'}=\alpha^A\alpha^B\epsilon^{A'B'}$.

For any antisymmetric $w^{ab}$, the [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md) acts on both tensor indices. In the printed curvature convention its complete contraction is

$$
[\nabla_a,\nabla_b]w^{ab}=R_{ab c}{}^a w^{cb}+R_{ab c}{}^b w^{ac}=-R_{bc}w^{cb}+R_{ac}w^{ac}=0,
$$

because the [Ricci tensor](../../../../../../ricci-tensor.md) is symmetric. Substituting the one-chirality [bivector](../../../../../../bivector.md) and the [chiral spinor curvature operator](../../../../../../chiral-spinor-curvature-operator.md) decomposition, the primed-operator term vanishes on contraction with the symmetric $\alpha^A\alpha^B$. The other term is $2\Delta_{AB}(\alpha^A\alpha^B)$. Hence $\Delta_{AB}(\alpha^A\alpha^B)=0$.

Repeat with $\alpha+\beta$ and subtract the identities for $\alpha$ and $\beta$. Linearity leaves twice the mixed symmetric product, giving the [contracted chiral curvature identity](../../../../../../contracted-chiral-curvature-identity.md)

$$
\boxed{\Delta_{AB}\big(\alpha^{(A}\beta^{B)}\big)=0.}
$$

The polarization works for spinor fields as well as pointwise spinors: the [chiral spinor curvature operator](../../../../../../chiral-spinor-curvature-operator.md) is algebraic by the preceding part.

The displayed source expression $\alpha_A\beta_B\epsilon_{A'B'}$ needs this clarification. For independent $\alpha,\beta$ it is not antisymmetric in the spacetime indices. Its antisymmetric part is $\alpha_{(A}\beta_{B)}\epsilon_{A'B'}$, which is generally not simple. The proof above uses a genuinely simple bivector first and then polarization, so it establishes the requested conclusion without relying on the incorrect simplicity assertion.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
