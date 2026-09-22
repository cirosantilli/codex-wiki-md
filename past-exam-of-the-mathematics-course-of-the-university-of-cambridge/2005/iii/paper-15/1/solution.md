<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [exterior derivative](../../../../../exterior-derivative.md) is an $\mathbb R$-linear operator $d:\Omega^r(M)\to\Omega^{r+1}(M)$ which agrees with the [differential of a smooth function](../../../../../differential-of-a-smooth-function.md) on degree zero, satisfies $d^2=0$, and obeys the [graded Leibniz rule](../../../../../graded-leibniz-rule.md)

$$
d(\alpha\wedge\beta)=d\alpha\wedge\beta+(-1)^r\alpha\wedge d\beta,
\qquad \alpha\in\Omega^r(M).
$$

For the [uniqueness of the exterior derivative from its axioms](../../../../../uniqueness-of-the-exterior-derivative-from-its-axioms.md), first note that these axioms force locality. If $\alpha$ vanishes near $p$, choose a [smooth bump function](../../../../../smooth-bump-function.md) $\chi$ equal to one near $p$ and supported where $\alpha=0$. Then $0=d(\chi\alpha)=d\chi\wedge\alpha+\chi d\alpha$ gives $d\alpha(p)=0$. Thus $d\alpha(p)$ depends only on the form near $p$.

In a coordinate chart write $\alpha=\sum_I a_I\,dx^{i_1}\wedge\cdots\wedge dx^{i_r}$. Since $d(dx^i)=d^2x^i=0$, the axioms force

$$
d\alpha=\sum_{I,j}\partial_j a_I\,dx^j\wedge dx^{i_1}\wedge\cdots\wedge dx^{i_r}.
$$

This also proves existence. Define $d$ by that formula in each chart. The product rule for [partial derivatives](../../../../../partial-derivative.md) gives the [graded Leibniz rule](../../../../../graded-leibniz-rule.md), and symmetry of mixed [partial derivatives](../../../../../partial-derivative.md) against antisymmetry of the [wedge product of differential forms](../../../../../wedge-product-of-differential-forms.md) gives $d^2=0$. On overlaps it still agrees with the differential of every function, by the [chain rule](../../../../../chain-rule.md), so the preceding uniqueness argument in the second coordinate system makes the formulas agree. They therefore glue to a global [exterior derivative](../../../../../exterior-derivative.md).

For a [differential one-form](../../../../../one-form.md) $\omega=\sum_i a_i dx^i$, the [exterior derivative of a one-form evaluated on vector fields](../../../../../exterior-derivative-of-a-one-form-evaluated-on-vector-fields.md) follows directly:

$$
d\omega(X,Y)=\sum_i\bigl(X(a_i)Y^i-Y(a_i)X^i\bigr).
$$

In $X(\omega(Y))-Y(\omega(X))$, the additional terms are $\sum_i a_i[X(Y^i)-Y(X^i)]=\omega([X,Y])$, where the bracket is the [Lie bracket of vector fields](../../../../../lie-bracket-of-vector-fields.md). Hence

$$
\boxed{d\omega(X,Y)=X\bigl(\omega(Y)\bigr)-Y\bigl(\omega(X)\bigr)-\omega([X,Y])}.
$$

The [de Rham cohomology](../../../../../de-rham-cohomology.md) is

$$
H^r_{\mathrm{dR}}(M)=
\frac{\ker(d:\Omega^r(M)\to\Omega^{r+1}(M))}
{\operatorname{im}(d:\Omega^{r-1}(M)\to\Omega^r(M))},
$$

with zero denominator in degree zero. The [Poincaré lemma](../../../../../poincare-lemma.md) states that a [closed differential form](../../../../../closed-differential-form.md) of positive degree on a star-shaped open subset of Euclidean space is an [exact differential form](../../../../../exact-differential-form.md); consequently every closed positive-degree form is locally exact on a [smooth manifold](../../../../../smooth-manifold.md).

For the [suspension isomorphism for top de Rham cohomology of spheres](../../../../../suspension-isomorphism-for-top-de-rham-cohomology-of-spheres.md), put $U=S^n\setminus\{\text{south pole}\}$ and $V=S^n\setminus\{\text{north pole}\}$. Both are diffeomorphic to $\mathbb R^n$, while $W=U\cap V$ deformation retracts onto the equatorial $S^{n-1}$. The [Mayer--Vietoris sequence for de Rham cohomology](../../../../../mayer-vietoris-sequence-for-de-rham-cohomology.md) comes from the [short exact sequence](../../../../../short-exact-sequence.md) of [cochain complexes](../../../../../cochain-complex.md)

$$
0\longrightarrow\Omega^*(S^n)
\longrightarrow\Omega^*(U)\oplus\Omega^*(V)
\xrightarrow{(\alpha,\beta)\mapsto\alpha|_W-\beta|_W}
\Omega^*(W)\longrightarrow0.
$$

The final map is surjective: a [partition of unity](../../../../../partition-of-unity.md) $\chi_U+\chi_V=1$ lets a form $\eta$ on $W$ be lifted by extending $\chi_V\eta$ to $U$ and $-\chi_U\eta$ to $V$ by zero. The [Poincaré lemma](../../../../../poincare-lemma.md) makes $H^{n-1}(U),H^{n-1}(V),H^n(U),H^n(V)$ vanish when $n>1$. Exactness gives

$$
0\longrightarrow H^{n-1}_{\mathrm{dR}}(W)
\xrightarrow{\delta}H^n_{\mathrm{dR}}(S^n)\longrightarrow0.
$$

If $j:S^{n-1}\hookrightarrow W$ is the equatorial inclusion, [homotopy invariance of de Rham cohomology](../../../../../homotopy-invariance-of-de-rham-cohomology.md) makes $j^*$ an [isomorphism](../../../../../isomorphism.md). Therefore

$$
\boxed{j^*\delta^{-1}:H^n_{\mathrm{dR}}(S^n)\longrightarrow H^{n-1}_{\mathrm{dR}}(S^{n-1})}
$$

is injective, indeed an [isomorphism](../../../../../isomorphism.md). Concretely, choose local primitives $d\alpha_U=\omega|_U$, $d\alpha_V=\omega|_V$, and send $[\omega]$ to $[j^*(\alpha_U-\alpha_V)]$. Their difference is closed; changing either primitive changes it by an exact form, so this agrees with the cohomological construction.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
