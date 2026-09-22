<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [complex structure](../../../../../complex-structure.md) on a [complex manifold](../../../../../complex-manifold.md) splits its complexified cotangent bundle into the $+i$ and $-i$ eigenspaces, locally spanned by $dz^j$ and $d\bar z^j$. A [differential form of type (p, q)](../../../../../differential-form-of-type-p-q.md) is a smooth section of $\bigwedge^p(T^{1,0}X)^*\otimes\bigwedge^q(T^{0,1}X)^*$, so in [holomorphic coordinates](../../../../../holomorphic-coordinate.md) it has the expression

$$
\eta=\sum_{|I|=p,\,|J|=q}\eta_{I,J}\,dz^I\wedge d\bar z^J.
$$

Here the increasing multi-indices avoid duplicating alternating factors. The [exterior derivative](../../../../../exterior-derivative.md) has just two type components: the [conjugate Dolbeault operator](../../../../../conjugate-dolbeault-operator.md) $\partial$ and the [Dolbeault operator](../../../../../dolbeault-operator.md) $\bar\partial$. On such a local expression they are

$$
\partial\eta=\sum_{I,J,k}\frac{\partial\eta_{I,J}}{\partial z^k}\,dz^k\wedge dz^I\wedge d\bar z^J,
\qquad
\bar\partial\eta=\sum_{I,J,k}\frac{\partial\eta_{I,J}}{\partial\bar z^k}\,d\bar z^k\wedge dz^I\wedge d\bar z^J.
$$

Holomorphic changes of coordinates preserve these types, so the definitions are intrinsic. Comparing type components of $d^2=0$ gives $\partial^2=\bar\partial^2=0$ and $\partial\bar\partial+\bar\partial\partial=0$.

A [real (p, p)-form](../../../../../real-p-p-form.md) satisfies $\bar\eta=\eta$, where [complex conjugation](../../../../../complex-conjugation.md) acts on both coefficients and differential factors. Conjugation exchanges the two [Dolbeault operators](../../../../../dolbeault-operator.md), so

$$
\partial\eta=\overline{\bar\partial\eta}.
$$

Thus $\bar\partial\eta=0$ forces $\partial\eta=0$ as well. Conversely, if $d\eta=0$, its distinct $(p+1,p)$ and $(p,p+1)$ components both vanish. Therefore

$$
\boxed{d\eta=0\quad\Longleftrightarrow\quad\bar\partial\eta=0\quad\text{for real }\eta\text{ of type }(p,p).}
$$

The assertion remains valid in top degree, when the indicated type components are zero automatically.

For a [holomorphic function](../../../../../holomorphic-function.md) $f$, $\bar\partial f=0$ and $\partial\bar f=0$. Writing its real part as $u=(f+\bar f)/2$ gives

$$
\bar\partial\partial u
=\tfrac12\bar\partial\partial f+\tfrac12\bar\partial\partial\bar f
=-\tfrac12\partial\bar\partial f+0=0.
$$

Hence **the real part of a [holomorphic function](../../../../../holomorphic-function.md) is a [pluriharmonic function](../../../../../pluriharmonic-function.md)**.

For the local exactness assertion, work on a smaller [polydisc](../../../../../polydisc.md) whose closure lies in the original one. The allowed one-variable integral is the [Cauchy-Green operator](../../../../../cauchy-green-operator.md) $T_j$ in coordinate $z_j$. Applied coefficientwise, it satisfies $\partial_{\bar z_j}T_j a=a$ on a smaller disc and commutes with differentiation in all other coordinates; the smooth parameter dependence follows by applying the integral to a smooth compactly supported extension in the integration variable. This extension can be made with a cutoff equal to one on the smaller disc.

Begin with a [Dolbeault operator](../../../../../dolbeault-operator.md) closed form $\varphi$ and decompose it uniquely as $\varphi=d\bar z^1\wedge\alpha+\beta$, where neither $\alpha$ nor $\beta$ contains $d\bar z^1$. Set $\psi_1=T_1\alpha$. The $d\bar z^1$ component of $\bar\partial\psi_1$ is exactly $d\bar z^1\wedge\alpha$, so

$$
\varphi_1=\varphi-\bar\partial\psi_1
$$

has no $d\bar z^1$ factor. It is still $\bar\partial$-closed. The $d\bar z^1$ component of $\bar\partial\varphi_1=0$ now shows that every coefficient of $\varphi_1$ is holomorphic in $z_1$.

Apply the same construction in $z_2$ to remove its antiholomorphic differential factor. The operator $T_2$ preserves holomorphicity in $z_1$, since it commutes with $\partial_{\bar z_1}$. Consequently the second subtraction introduces no previously removed factor. Continue through all $n$ coordinates, shrinking the [polydisc](../../../../../polydisc.md) when necessary. The final remainder has positive antiholomorphic degree but contains none of the $d\bar z^j$, and hence is zero. This [coordinate elimination for local Dolbeault primitives](../../../../../coordinate-elimination-for-local-dolbeault-primitives.md) constructs

$$
\boxed{\psi=\psi_1+\cdots+\psi_n,\qquad
\bar\partial\psi=\varphi|_{U_0}.}
$$

If $q>n$, the original form is already zero, so one can take $\psi=0$.

Finally let $\varphi$ be a smooth $(0,1)$-form on the [complex projective line](../../../../../complex-projective-line.md). Choose $0<r<R$ and the two coordinate neighborhoods $U=\{|z|<R\}$ and $V=\{|z|>r\}\cup\{\infty\}$, the latter expressed in $w=1/z$. They cover the sphere. The one-variable construction, integrating over slightly larger closed discs in each coordinate chart, gives smooth functions $a$ on $U$ and $b$ on $V$ with $\bar\partial a=\varphi|_U$ and $\bar\partial b=\varphi|_V$.

Their difference $h=a-b$ is a [holomorphic function](../../../../../holomorphic-function.md) on the [annulus](../../../../../annulus-mathematics.md) $r<|z|<R$. Its [Laurent series](../../../../../laurent-series.md) splits as

$$
h(z)=h_+(z)+h_-(z),\qquad
h_+=\sum_{m\geq0}c_mz^m,\quad h_-=\sum_{m<0}c_mz^m.
$$

The first series extends holomorphically throughout $U$, while the second extends throughout $V$, including infinity, where it has value zero. Thus $a-h_+$ and $b+h_-$ agree on the overlap and glue to a global smooth function $F$. Both corrections are holomorphic, so

$$
\boxed{\bar\partial F=\varphi,\qquad H^{0,1}_{\bar\partial}(\mathbb P^1)=0.}
$$

This [Laurent gluing of Dolbeault primitives on the projective line](../../../../../laurent-gluing-of-dolbeault-primitives-on-the-projective-line.md) uses no [Hodge theorem](../../../../../hodge-decomposition-theorem.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
