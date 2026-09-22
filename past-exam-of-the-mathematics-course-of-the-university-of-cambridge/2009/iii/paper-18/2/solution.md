<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $X=\operatorname{Pic}^{g-1}(C)$. The [theta divisor](../../../../../theta-divisor.md) is the effective locus

$$
\Theta=\{[M]\in X:H^0(C,M)\ne0\}=\operatorname{im}\bigl(C^{(g-1)}\longrightarrow X\bigr).
$$

For its [scheme](../../../../../scheme.md) structure, take a fixed effective [Cartier divisor](../../../../../cartier-divisor-split.md) $E$ of degree $e\ge g$ and a universal [line bundle](../../../../../line-bundle.md) $M$ locally on $X$. Both $\pi_*M(E)$ and $\pi_*(M(E)|_E)$ are rank-$e$ [vector bundles](../../../../../vector-bundle.md); the first assertion follows from [Serre duality](../../../../../serre-duality.md) and the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md). Define $\Theta$ by the [determinant](../../../../../determinant.md) of their evaluation map. Its kernel is $H^0(C,M)$, so this is precisely the required locus. Exact sequences for enlarging $E$ cancel an invertible determinant factor, making the [determinant description of the theta divisor](../../../../../determinant-description-of-the-theta-divisor.md) independent of $E$.

This is a genuine irreducible reduced [Cartier divisor](../../../../../cartier-divisor-split.md). Choose $g-1$ points imposing independent conditions on $H^0(C,K_C)$. For their effective [Cartier divisor](../../../../../cartier-divisor-split.md) $D'$, the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) gives $h^0(\mathcal O(D'))=h^1(\mathcal O(D'))=1$. These points form a nonempty open set in the irreducible [symmetric product of a curve](../../../../../symmetric-product-of-a-curve.md) $C^{(g-1)}$; the [Abel map of an algebraic curve](../../../../../abel-map-of-an-algebraic-curve.md) is generically one-to-one there, so its image has dimension $g-1$. At such a class $M$, the first-order change of the evaluation [determinant](../../../../../determinant.md) is the cup-product functional

$$
H^1(C,\mathcal O_C)\longrightarrow\operatorname{Hom}(H^0(C,M),H^1(C,M)).
$$

Under [Serre duality](../../../../../serre-duality.md) its dual is multiplication $H^0(M)\otimes H^0(K_C\otimes M^{-1})\to H^0(K_C)$. The product of two nonzero sections on an integral [algebraic curve](../../../../../algebraic-curve.md) is nonzero. Thus the functional is nonzero and the [determinant](../../../../../determinant.md) has multiplicity one generically. Its irreducible support is consequently the reduced [theta divisor](../../../../../theta-divisor.md).

Now let $L=\mathcal O_C(D)$ have degree $g$. The [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) gives $h^0(L)\ge1$, while evaluation at $P$ gives

$$
H^0(C,L(-P))=\ker\bigl(H^0(C,L)\longrightarrow L|_P\bigr).
$$

If $h^0(L)\ge2$, this kernel is nonzero for every $P$, so the entire image of $\phi_D$ lies in $\Theta$. If $h^0(L)=1$, write $s$ for a nonzero section. The kernel is nonzero exactly at the zeros of $s$, so the image is not contained in $\Theta$. Moreover $h^1(L)=0$, and the family $L(-P)$ is computed by the rank-one evaluation map $H^0(L)\otimes\mathcal O_C\to L$. Its [determinant](../../../../../determinant.md) is $s$ itself. This proves the scheme-theoretic [restriction of the theta divisor to an Abel curve](../../../../../restriction-of-the-theta-divisor-to-an-abel-curve.md):

$$
\boxed{\phi_D(C)\subseteq\Theta\iff h^0(L)\ge2,\qquad \phi_D^*\Theta=\operatorname{div}(s)\text{ when }h^0(L)=1.}
$$

Here the intersection is regarded as a [Cartier divisor](../../../../../cartier-divisor-split.md) on $C$. Since $D$ was specified as a [divisor class](../../../../../divisor-class.md), it means its unique effective representative, with all multiplicities. The map $\phi_D$ is an embedding: distinct points with the same image would give a degree-one map $C\to\mathbb P^1$; its cotangent map is evaluation of canonical differentials, which is surjective because $K_C$ is base-point-free. To see the latter, $h^0(\mathcal O_C(P))=1$ for genus at least one, and the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) gives $h^0(K_C-P)=g-1$. Thus the pullback also describes the intersection on the embedded curve.

It remains to count sections on $X$. Let $s_\Theta$ be the section defining the [theta divisor](../../../../../theta-divisor.md), and take any $s\in H^0(X,\mathcal O_X(\Theta))$. The quotient $r=s/s_\Theta$ is a [rational function](../../../../../rational-function.md). Choose a fixed degree-$2g-1$ [line bundle](../../../../../line-bundle.md) $T$ and the morphism

$$
\beta:C^g\longrightarrow X,\qquad (P_1,\ldots,P_g)\longmapsto[T(-P_1-\cdots-P_g)].
$$

It is surjective: for every $M\in X$, the degree-$g$ bundle $T\otimes M^{-1}$ has a nonzero section by the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md). On a general coordinate curve, put $D=T-\sum_{j\ne i}P_j$. The $g-1$ general points impose independent conditions on the $g$-dimensional space $H^0(C,T)$, leaving $h^0(\mathcal O(D))=1$. This independence follows inductively by choosing each new point away from the common zero set of the remaining nonzero sections. The restriction already proved identifies $\mathcal O_X(\Theta)$ on that coordinate curve with $\mathcal O_C(D)$, whose section space is one-dimensional. Hence $r\circ\beta$ is constant along every general coordinate curve.

A [rational function](../../../../../rational-function.md) on a product of integral curves which is constant in each factor is constant: on a common dense open set, successively varying one coordinate identifies its value with the value at a fixed general tuple. Therefore $r\circ\beta\in k$, and surjectivity of $\beta$ gives $r\in k$. Every $s$ is a scalar multiple of $s_\Theta$, proving

$$
\boxed{\dim H^0(X,\mathcal O_X(\Theta))=1.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
