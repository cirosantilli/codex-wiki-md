<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

An [almost complex structure](../../../../../almost-complex-manifold.md) is a smooth real [vector bundle endomorphism](../../../../../vector-bundle-endomorphism.md) $J:TM\to TM$ satisfying $J^2=-I$. In particular, $M$ has even real dimension $2n$. Extend $J$ complex-linearly to $T_{\mathbb C}M=TM\otimes_{\mathbb R}\mathbb C$. Its minimal polynomial divides $(u-i)(u+i)$, whose roots are distinct, so the [type decomposition of the complexified tangent bundle](../../../../../type-decomposition-of-the-complexified-tangent-bundle.md) is

$$
T_{\mathbb C}M=T^{1,0}M\oplus T^{0,1}M,\qquad
T^{1,0}M=\ker(J-iI),\quad T^{0,1}M=\ker(J+iI).
$$

The smooth projections are $(I-iJ)/2$ and $(I+iJ)/2$. [Complex conjugation](../../../../../complex-conjugation.md) exchanges the two rank-$n$ [eigenbundles](../../../../../eigenbundle.md). A $(1,0)$-covector annihilates $T^{0,1}M$ and a $(0,1)$-covector annihilates $T^{1,0}M$. Thus the [differential forms of type (p, q)](../../../../../differential-form-of-type-p-q.md) are the smooth sections of

$$
\Lambda^{p,q}T^*M=\Lambda^p(T^{1,0}M)^*\otimes\Lambda^q(T^{0,1}M)^*,
\qquad
\Lambda^rT^*_{\mathbb C}M=\bigoplus_{p+q=r}\Lambda^{p,q}T^*M.
$$

Here the tensor product is identified with its image under the [wedge product of differential forms](../../../../../wedge-product-of-differential-forms.md). For a real tangent vector $v$, the vectors $v-iJv$ and $v+iJv$ exhibit the two types directly.

We now construct the [almost complex structure from a decomposable volume form](../../../../../almost-complex-structure-from-a-decomposable-volume-form.md). Locally write $\Omega=\theta_1\wedge\cdots\wedge\theta_n$. The nonvanishing of $\Omega\wedge\overline\Omega$ says that the $2n$ covectors $\theta_1,\ldots,\theta_n,\overline\theta_1,\ldots,\overline\theta_n$ form a complex coframe. In particular, the span of the $\theta_j$ has the intrinsic description

$$
W_x=\{\alpha\in T_x^*M\otimes\mathbb C:\alpha\wedge\Omega_x=0\}.
$$

Indeed, expansion in that coframe shows that every coefficient of a conjugate factor must vanish if $\alpha\wedge\Omega_x=0$. Therefore this span is independent of the chosen local factorization. The local coframes show that $W$ is a smooth rank-$n$ [vector subbundle](../../../../../vector-subbundle.md), and

$$
T^*M\otimes\mathbb C=W\oplus\overline W.
$$

Define $J_\Omega^*$ to be multiplication by $i$ on $W$ and by $-i$ on $\overline W$. It commutes with [complex conjugation](../../../../../complex-conjugation.md), so is the complexification of a real smooth [bundle endomorphism](../../../../../vector-bundle-endomorphism.md), whose dual defines $J_\Omega$ on $TM$. It has square $-I$, and its $(1,0)$-covectors are exactly $W$. Conversely, any such [almost complex structure](../../../../../almost-complex-manifold.md) must have this same action on the entire coframe. Thus **$J_\Omega$ exists globally and is unique**, and every factor in every allowed decomposition is a $(1,0)$-form.

Finally suppose $d\Omega=0$. Since $\theta_j\wedge\Omega=0$, the [exterior derivative](../../../../../exterior-derivative.md) product rule gives

$$
0=d(\theta_j\wedge\Omega)=d\theta_j\wedge\Omega-\theta_j\wedge d\Omega
=d\theta_j\wedge\Omega.
$$

Decompose $d\theta_j$ into types $(2,0)$, $(1,1)$ and $(0,2)$ using $J_\Omega$. The first two wedge products with the $(n,0)$-form $\Omega$ vanish by dimension. On $(0,2)$-forms, wedging with $\Omega$ is injective: the monomials $\Omega\wedge\overline\theta_a\wedge\overline\theta_b$ are linearly independent. For $n=1$ the $(0,2)$ space is zero, so the statement still holds. Hence every $d\theta_j$ has no $(0,2)$ component. For an arbitrary $(1,0)$-form $\alpha=\sum_j a_j\theta_j$, the extra terms $da_j\wedge\theta_j$ likewise have only types $(2,0)$ and $(1,1)$. The [bracket and differential-form criteria for integrability](../../../../../bracket-and-differential-form-criteria-for-integrability.md) proved below now give

$$
\boxed{d\Omega=0\ \Longrightarrow\ J_\Omega\text{ is integrable}.}
$$

Local decomposability has been used essentially; the nonvanishing top-degree product alone does not provide the required coframe.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
