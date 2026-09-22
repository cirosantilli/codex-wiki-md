<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In coordinates, write a [differential form](../../../../../differential-form-split.md) as $\eta=\sum_I\eta_I\,dx^{i_1}\wedge\cdots\wedge dx^{i_r}$. Its [exterior derivative](../../../../../exterior-derivative.md) is

$$
d\eta=\sum_I d\eta_I\wedge dx^{i_1}\wedge\cdots\wedge dx^{i_r}.
$$

For $r=0$ this is the ordinary differential $df$. The [chain rule](../../../../../chain-rule.md), together with cancellation of symmetric second derivatives against the exterior product, proves that these formulas agree under coordinate changes. They give an $\mathbb R$-linear map $d:\Omega^r(M)\to\Omega^{r+1}(M)$ with $d^2=0$ and $d(\alpha\wedge\beta)=d\alpha\wedge\beta+(-1)^r\alpha\wedge d\beta$ when $\alpha$ has degree $r$.

For a [differential one-form](../../../../../one-form.md) $\omega=\sum_j\omega_jdx^j$, evaluation gives

$$
d\omega(X,Y)=\sum_{i,j}\partial_i\omega_j(X^iY^j-Y^iX^j).
$$

Expanding $X(\omega(Y))-Y(\omega(X))$ gives these coefficient derivatives plus $\sum_j\omega_j\sum_i(X^i\partial_iY^j-Y^i\partial_iX^j)$. The latter is $\omega([X,Y])$ by the [Lie bracket of vector fields](../../../../../lie-bracket-of-vector-fields.md) formula. Hence

$$
\boxed{d\omega(X,Y)=X(\omega(Y))-Y(\omega(X))-\omega([X,Y]).}
$$

A [connection on a vector bundle](../../../../../connection-vector-bundle.md) is an $\mathbb R$-linear map $D:\Gamma(E)\to\Omega^1(M;E)$ satisfying $D(f\sigma)=df\otimes\sigma+fD\sigma$. Evaluation on a [vector field](../../../../../vector-field.md) gives $D_X\sigma$, which is $C^\infty$-linear in $X$ and satisfies $D_X(f\sigma)=X(f)\sigma+fD_X\sigma$. The [covariant exterior derivative](../../../../../exterior-covariant-derivative.md) extends this to bundle-valued forms by

$$
d^E(\alpha\otimes\sigma)=d\alpha\otimes\sigma+(-1)^r\alpha\wedge D\sigma,\qquad\alpha\in\Omega^r(M).
$$

This respects $(f\alpha)\otimes\sigma=\alpha\otimes(f\sigma)$: applying the rule on either side gives the same extra term $df\wedge\alpha\otimes\sigma$. It therefore defines an operator on bundle-valued forms independently of their local tensor representations. In a local frame with connection matrix $A$, its coefficient-column formula is $d^E=d+A\wedge$.

Define the [curvature form of a connection](../../../../../curvature-form.md) by $R\sigma=(d^E)^2\sigma$. The extra terms in $(d^E)^2(f\sigma)$ cancel, so this equals $f(d^E)^2\sigma$. Equivalently the local formula is

$$
R=dA+A\wedge A,
$$

which acts fibrewise on the section coefficients. Thus curvature is a smooth endomorphism-valued two-form, a section of $\Lambda^2T^*M\otimes\operatorname{End}(E)$.

For an $E$-valued one-form $a$, applying the ordinary one-form formula in a frame gives

$$
(d^Ea)(X,Y)=D_X(a(Y))-D_Y(a(X))-a([X,Y]).
$$

Taking $a=D\sigma$ proves the required curvature identity

$$
\boxed{R(X,Y)\sigma=D_XD_Y\sigma-D_YD_X\sigma-D_{[X,Y]}\sigma.}
$$

The bracket correction is what makes the right side tensorial in the vector fields and the section.

Now define the [endomorphism bundle connection](../../../../../endomorphism-bundle-connection.md) by $(\widetilde D_X\alpha)(s)=D_X(\alpha s)-\alpha(D_Xs)$. This expression is $C^\infty$-linear in $s$: the two terms involving $X(f)\alpha(s)$ cancel when $s$ is replaced by $fs$. It is therefore a smooth bundle endomorphism. It is $C^\infty$-linear in $X$, and

$$
\widetilde D_X(f\alpha)=X(f)\alpha+f\widetilde D_X\alpha.
$$

These identities prove it is a [connection on a vector bundle](../../../../../connection-vector-bundle.md). In a local frame it reads $\widetilde D_X\alpha=X(\alpha)+[A(X),\alpha]$.

For the full [commutator identity for an endomorphism connection](../../../../../commutator-identity-for-an-endomorphism-connection.md), expand once more:

$$
(\widetilde D_X\widetilde D_Y\alpha)(s)=D_XD_Y(\alpha s)-D_X(\alpha D_Ys)-D_Y(\alpha D_Xs)+\alpha D_YD_Xs.
$$

Subtracting the expression with $X,Y$ interchanged cancels both middle terms. Thus

$$
\boxed{([\widetilde D_X,\widetilde D_Y]\alpha)(s)=[D_X,D_Y](\alpha s)-\alpha([D_X,D_Y]s).}
$$

Here $D_X,D_Y$ are differential operators on sections, and the square brackets are their operator commutators. In general they are not fibrewise bundle endomorphisms; the curvature operator becomes fibrewise linear after subtracting $D_{[X,Y]}$.

Subtracting $\widetilde D_{[X,Y]}\alpha$ from this identity gives the [curvature of an endomorphism bundle connection](../../../../../curvature-of-an-endomorphism-bundle-connection.md):

$$
(\widetilde R(X,Y)\alpha)(s)=R(X,Y)(\alpha s)-\alpha(R(X,Y)s),\qquad\widetilde R(X,Y)\alpha=[R(X,Y),\alpha].
$$

Consequently $\widetilde R=0$ precisely when every $R_p(X,Y)$ commutes with every endomorphism of $E_p$. Arbitrary such endomorphisms can be extended locally in a frame, so this is a fibrewise assertion. A matrix commuting with all diagonal matrix units is diagonal; commuting also with all off-diagonal matrix units forces all its diagonal entries to coincide. The centre of the full endomorphism algebra therefore consists of scalar matrices. For rank $k>0$, define the smooth two-form $\omega=k^{-1}\operatorname{tr}R$. We obtain the [scalar-curvature criterion for a flat endomorphism connection](../../../../../scalar-curvature-criterion-for-a-flat-endomorphism-connection.md)

$$
\boxed{\widetilde R=0\quad\Longleftrightarrow\quad R=\omega\otimes\operatorname{id}_E.}
$$

The converse follows immediately because scalar endomorphisms commute with all endomorphisms. For the zero bundle both curvatures vanish and one can take $\omega=0$. Scalar curvature here means the scalar endomorphism-valued curvature of this bundle connection, not the scalar trace curvature of a Riemannian manifold.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
