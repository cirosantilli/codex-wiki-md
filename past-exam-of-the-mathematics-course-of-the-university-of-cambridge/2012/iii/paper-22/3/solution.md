<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [connection difference as an endomorphism-valued one-form](../../../../../connection-difference-as-an-endomorphism-valued-one-form.md) follows because the [graded Leibniz rule](../../../../../graded-leibniz-rule.md) terms cancel:

$$
(D_1-D)(fs)=f(D_1-D)s.
$$

Thus $a=D_1-D$ is a global endomorphism-valued one-form. To define the [endomorphism bundle connection](../../../../../endomorphism-bundle-connection.md), require

$$
(\widetilde D\phi)(s)=D(\phi s)-\phi(Ds).
$$

The right side is $C^\infty$-linear in $s$, so it is indeed an endomorphism-valued one-form, and replacing $\phi$ by $f\phi$ gives $df\otimes\phi+f\widetilde D\phi$. In a frame with [connection matrix](../../../../../connection-one-form.md) $A$, its extension to an endomorphism-valued $k$-form $b$ is

$$
\widetilde D b=db+A\wedge b-(-1)^k b\wedge A.
$$

The [endomorphism-valued exterior product](../../../../../endomorphism-valued-exterior-product.md) combines the wedge of [differential forms](../../../../../differential-form-split.md) with composition in $\operatorname{End}E$. In particular,

$$
(a\wedge a)(u,v)=a(u)a(v)-a(v)a(u),\qquad
\widetilde D a=da+A\wedge a+a\wedge A.
$$

Expanding $d(A+a)+(A+a)\wedge(A+a)$ proves the [curvature difference formula](../../../../../curvature-difference-formula.md):

$$
\boxed{\Theta_{D+a}=\Theta_D+\widetilde D a+a\wedge a.}
$$

The [Chern connection](../../../../../chern-connection.md) is characterized by [metric compatibility](../../../../../metric-compatibility.md) and $D^{0,1}=\bar\partial_E$. Take [Hermitian inner products](../../../../../hermitian-form.md) linear in the first variable. In a [holomorphic local frame](../../../../../holomorphic-local-trivialization.md) write $\langle eu,ev\rangle=v^\dagger Hu$, with $H$ a positive [Hermitian matrix](../../../../../hermitian-operator.md). The second condition forces $A^{0,1}=0$, and [metric compatibility](../../../../../metric-compatibility.md) is

$$
dH=A^\dagger H+HA.
$$

Its $(1,0)$ component determines $A$ uniquely:

$$
\boxed{A=H^{-1}\partial H.}
$$

Conversely this formula and its conjugate transpose satisfy the metric equation. Under a [holomorphic local frame](../../../../../holomorphic-local-trivialization.md) change, $H'=g^\dagger Hg$ and $\partial g^\dagger=0$, so the displayed formula transforms by $A'=g^{-1}Ag+g^{-1}\partial g$. Hence the local matrices patch, proving existence and uniqueness.

Differentiating $H^{-1}$ gives

$$
\partial A=-H^{-1}(\partial H)H^{-1}\wedge\partial H=-A\wedge A.
$$

Therefore the $(2,0)$ [vector-bundle curvature](../../../../../curvature-form.md) is zero. There is no $(0,2)$ component, and

$$
\boxed{\Theta=\bar\partial A\in A^{1,1}(\operatorname{End}E),\qquad
\bar\partial_{\operatorname{End}E}\Theta=0.}
$$

The last equality is $\bar\partial^2 A=0$ in [holomorphic local frames](../../../../../holomorphic-local-trivialization.md), so is intrinsic. This is [Dolbeault closedness of Chern curvature](../../../../../dolbeault-closedness-of-chern-curvature.md). The induced [endomorphism bundle connection](../../../../../endomorphism-bundle-connection.md) is itself the [Chern connection](../../../../../chern-connection.md) for the Hilbert-Schmidt metric on $\operatorname{End}E$: the [tensor product](../../../../../tensor-product.md) of a metric-compatible connection and its dual preserves the induced metric, and its $(0,1)$ part is the induced holomorphic [Dolbeault operator](../../../../../dolbeault-operator.md). These two properties and uniqueness suffice; no further matrix calculation is needed.

For two metrics, both [Chern connections](../../../../../chern-connection.md) have the same $(0,1)$ part, so **$a\in A^{1,0}(\operatorname{End}E)$**. The $(1,1)$ part of the [curvature difference formula](../../../../../curvature-difference-formula.md) is just $\bar\partial_{\operatorname{End}E}a$; the other two terms have type $(2,0)$, which must cancel because both [vector-bundle curvatures](../../../../../curvature-form.md) have type $(1,1)$. Thus

$$
\boxed{\Theta_1-\Theta_0=\bar\partial_{\operatorname{End}E}a.}
$$

By [Dolbeault theorem](../../../../../dolbeault-theorem.md), this proves that the [curvature Dolbeault class](../../../../../curvature-dolbeault-class.md)

$$
\alpha(E)=[\Theta]\in H^1(M,\Omega_M^1\otimes\operatorname{End}E)
$$

is independent of the metric.

Endomorphism composition and [wedge product of differential forms](../../../../../wedge-product-of-differential-forms.md) define the powers in $A^{k,k}(\operatorname{End}E)$, rather than in a [tensor power](../../../../../tensor-power.md) of the [endomorphism](../../../../../endomorphism.md) bundle. The [Dolbeault operator](../../../../../dolbeault-operator.md) is a derivation, so $\bar\partial(\Theta^k)=0$. The noncommutative telescoping identity gives the stronger explicit independence statement

$$
\Theta_1^k-\Theta_0^k
=\sum_{j=0}^{k-1}\Theta_1^j\wedge(\Theta_1-\Theta_0)
\wedge\Theta_0^{k-1-j}
=\bar\partial_{\operatorname{End}E}
\left(\sum_{j=0}^{k-1}\Theta_1^j\wedge a\wedge\Theta_0^{k-1-j}\right).
$$

All powers of [vector-bundle curvature](../../../../../curvature-form.md) have even total degree, so the derivation introduces no extra signs before $a$. Consequently

$$
\boxed{\alpha(E)^k=[\Theta^k]\in H^k(M,\Omega_M^k\otimes\operatorname{End}E)}
$$

is metric independent. For $k>n$, the form space and the resulting class are zero. This proves [metric independence of curvature Dolbeault powers](../../../../../metric-independence-of-curvature-dolbeault-powers.md) without assuming that endomorphism-valued forms commute.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
