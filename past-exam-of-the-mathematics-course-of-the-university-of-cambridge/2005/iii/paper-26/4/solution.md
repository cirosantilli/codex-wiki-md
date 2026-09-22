<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For an [adjunction](../../../../../adjoint-functors.md) $L:\mathcal C\rightleftarrows\mathcal D:R$, write its [adjunction unit](../../../../../unit-of-an-adjunction.md) as $\eta$ and its [adjunction counit](../../../../../counit-of-an-adjunction.md) as $\varepsilon$. It is an [idempotent adjunction](../../../../../idempotent-adjunction.md) when the induced [monad](../../../../../monad.md) has invertible multiplication $\mu=R\varepsilon L:RLRL\Rightarrow RL$. The dual condition is invertibility of the induced [comonad](../../../../../comonad.md) comultiplication $\delta=L\eta R:LR\Rightarrow LRLR$.

To prove equivalence of these conditions, suppose $\mu$ is invertible. The two unit identities imply $T\eta=\eta T=\mu^{-1}$, where $T=RL$. For any [algebra for a monad](../../../../../algebra-for-a-monad.md) $a:TA\to A$, naturality gives

$$
\eta_Aa=Ta\,\eta_{TA}=Ta\,T\eta_A=T(a\eta_A)=1_{TA},
$$

while $a\eta_A=1_A$. Thus $\eta_A$ is invertible. For each $D\in\mathcal D$, the arrow $R\varepsilon_D:T(RD)\to RD$ is a [monad algebra](../../../../../algebra-for-a-monad.md) action, so $\eta_{RD}$ is invertible. Applying $L$ proves $\delta_D=L\eta_{RD}$ invertible. Apply this implication to the opposite [adjunction](../../../../../adjoint-functors.md), interchanging the roles of the [monad](../../../../../monad.md) and comonad, to obtain the converse. Therefore **idempotence is self-dual**.

The [open-set frame](../../../../../open-set-frame.md) $O(X)$ is ordered by inclusion. Its arbitrary [joins](../../../../../least-upper-bound-in-a-partially-ordered-set.md) are unions; arbitrary [meets](../../../../../greatest-lower-bound-in-a-partially-ordered-set.md) are interiors of intersections. Finite intersections are already open, so finite [meets](../../../../../greatest-lower-bound-in-a-partially-ordered-set.md) are ordinary intersections, including the empty [meet](../../../../../greatest-lower-bound-in-a-partially-ordered-set.md) $X$. Distributivity of intersection over arbitrary unions proves the [frame](../../../../../complete-heyting-algebra.md) law. If $f:X\to Y$ is a [continuous map](../../../../../continuous-map.md), inverse image

$$
f^{-1}:O(Y)\to O(X)
$$

preserves arbitrary unions and finite intersections, including $\varnothing$ and the entire space. It is therefore a [frame homomorphism](../../../../../frame-homomorphism.md). Since $(gf)^{-1}=f^{-1}g^{-1}$ and $1_X^{-1}=1_{O(X)}$, this defines $O:\mathbf{Top}\to\mathbf{Frm}^{\mathrm{op}}$.

Let $\mathbf2=\{0<1\}$ and let $P(A)$ be the set of [points of a frame](../../../../../point-of-a-frame.md) $A$, namely [frame homomorphisms](../../../../../frame-homomorphism.md) $A\to\mathbf2$. For $a\in A$, put $U_a=\{p:p(a)=1\}$. Preservation of [joins](../../../../../least-upper-bound-in-a-partially-ordered-set.md) and finite [meets](../../../../../greatest-lower-bound-in-a-partially-ordered-set.md) gives

$$
U_0=\varnothing,\qquad U_1=P(A),\qquad U_{a\wedge b}=U_a\cap U_b,\qquad U_{\bigvee_i a_i}=\bigcup_iU_{a_i}.
$$

In the last equality, a [join](../../../../../least-upper-bound-in-a-partially-ordered-set.md) in $\mathbf2$ is $1$ precisely when at least one summand is $1$, also covering the empty family. Thus the sets $U_a$ are all the opens of a [topology](../../../../../topology-split.md), rather than merely a proposed basis.

For a [frame homomorphism](../../../../../frame-homomorphism.md) $h:A\to B$, define $P(h):P(B)\to P(A)$ by $p\mapsto p\circ h$. Since $P(h)^{-1}(U_a)=U_{h(a)}$, it is continuous. Composition and identities follow from composition of functions, giving $P:\mathbf{Frm}^{\mathrm{op}}\to\mathbf{Top}$.

The [frame-point adjunction](../../../../../frame-point-adjunction.md) is the natural [bijection](../../../../../bijection.md)

$$
\mathbf{Top}(X,P(A))\cong\mathbf{Frm}(A,O(X))
=\mathbf{Frm}^{\mathrm{op}}(O(X),A).
$$

A [continuous map](../../../../../continuous-map.md) $f:X\to P(A)$ determines $h_f(a)=f^{-1}(U_a)$; the displayed identities for $U_a$ show that $h_f$ is a [frame homomorphism](../../../../../frame-homomorphism.md). Conversely a [frame homomorphism](../../../../../frame-homomorphism.md) $h:A\to O(X)$ determines $f_h(x)(a)=1$ exactly when $x\in h(a)$. Membership in unions and finite intersections proves that $f_h(x)$ is a [frame homomorphism](../../../../../frame-homomorphism.md) to $\mathbf2$, and $f_h^{-1}(U_a)=h(a)$ proves continuity. These constructions are inverse. Precomposing in $X$ becomes inverse image of open sets; precomposing a [frame homomorphism](../../../../../frame-homomorphism.md) becomes composition of [frame](../../../../../complete-heyting-algebra.md) points. Hence the bijection is natural in both arguments and proves $O\dashv P$.

The [adjunction unit](../../../../../unit-of-an-adjunction.md) is

$$
\eta_X:X\to P(O(X)),\qquad \eta_X(x)(V)=1\ \Longleftrightarrow\ x\in V.
$$

The [adjunction counit](../../../../../counit-of-an-adjunction.md) at $A$, regarded as an arrow of $\mathbf{Frm}^{\mathrm{op}}$, is represented by the [frame homomorphism](../../../../../frame-homomorphism.md) $e_A:A\to O(P(A))$, $a\mapsto U_a$. It is surjective because every open of $P(A)$ is of this form. We can compute $P(e_A):P(O(P(A)))\to P(A)$ explicitly: it sends $q$ to $p=q\circ e_A$. For every open $U_a$ of $P(A)$,

$$
\eta_{P(A)}(p)(U_a)=p(a)=q(U_a).
$$

Thus $\eta_{P(A)}P(e_A)=1$. Conversely, evaluation at $p$ sends $U_a$ to $p(a)$, so $P(e_A)\eta_{P(A)}=1$. Both maps are continuous by their definitions. Therefore $P(e_A)$ is a [homeomorphism](../../../../../homeomorphism.md). The multiplication of the induced [monad](../../../../../monad.md) $PO$ at $X$ is $P(e_{O(X)})$, which is invertible by this calculation. Consequently **the frame-point adjunction is idempotent**. This does not assert that every $\eta_X$ is a [homeomorphism](../../../../../homeomorphism.md): it says that applying the point-space construction a second time makes no further change.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
