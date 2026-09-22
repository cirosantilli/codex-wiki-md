<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For each [algebra for a monad](../../../../../../algebra-for-a-monad.md) $(A,a)$, consider the specific pair in $\mathcal D$

$$
FTA\mathrel{\substack{\xrightarrow{Fa}\\\xrightarrow[\varepsilon_{FA}]{} }}FA.
$$

Then the exact condition is

$$
\boxed{K\text{ has a left adjoint}\quad\Longleftrightarrow\quad
\text{each of these pairs has a coequalizer in }\mathcal D.}
$$

Each pair is reflexive, with common section $F\eta_A$: the two composite identities follow from $a\eta_A=1_A$ and $\varepsilon_{FA}F\eta_A=1_{FA}$. Thus existence of all [reflexive coequalizers](../../../../../../reflexive-coequalizer.md) is sufficient, but the displayed specified pairs give the necessary-and-sufficient condition.

To prove it, take $h:FA\to d$ and its adjoint transpose $x=Gh\eta_A:A\to Gd$. The transpose of $hFa$ is $xa$, by [naturality](../../../../../../naturality.md) of $\eta$. The transpose of $h\varepsilon_{FA}$ is

$$
GhG\varepsilon_{FA}\eta_{TA}=Gh\mu_A\eta_{TA}=Gh.
$$

Moreover counit [naturality](../../../../../../naturality.md) and a triangle identity give

$$
G\varepsilon_d T x
=G\varepsilon_d,GF(Gh\eta_A)
=Gh,G\varepsilon_{FA},GF\eta_A=Gh.
$$

Because transposition is bijective, the coequalizing equation is therefore equivalent to

$$
hFa=h\varepsilon_{FA}\quad\Longleftrightarrow\quad xa=G\varepsilon_d T x.
$$

The right side says exactly that $x:(A,a)\to Kd$ is a [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md).

For sufficiency, choose a [coequalizer](../../../../../../coequalizer.md) $q_a:FA\to L(A,a)$ for every [monad algebra](../../../../../../algebra-for-a-monad.md). Its [universal property](../../../../../../universal-property.md) and the equivalence just proved give [natural bijections](../../../../../../natural-bijection.md)

$$
\mathcal D(L(A,a),d)\cong
\{h:FA\to d:hFa=h\varepsilon_{FA}\}
\cong\mathcal C^T((A,a),Kd).
$$

To see explicitly that the chosen objects form a [functor](../../../../../../functor.md), an [monad algebra](../../../../../../algebra-for-a-monad.md) [morphism](../../../../../../morphism.md) $u:(A,a)\to(B,b)$ makes $q_bFu$ coequalize the pair for $a$: use $ua=bTu$ and [naturality](../../../../../../naturality.md) of the counit. Hence there is a unique $Lu$ with $Lu\,q_a=q_bFu$. Uniqueness proves its identity and composition laws and the [naturality](../../../../../../naturality.md) of the displayed [bijections](../../../../../../bijection.md). Thus $L\dashv K$.

Conversely, suppose $L\dashv K$ with unit $\lambda_{(A,a)}:(A,a)\to KL(A,a)$. Transpose its underlying arrow $A\to GL(A,a)$ through $F\dashv G$ to obtain $q_a:FA\to L(A,a)$. Since the unit is an [monad algebra](../../../../../../algebra-for-a-monad.md) [morphism](../../../../../../morphism.md), the equivalence above shows that $q_a$ coequalizes the specified pair. Any coequalizing $h:FA\to d$ transposes to an [monad algebra](../../../../../../algebra-for-a-monad.md) map $(A,a)\to Kd$, which factors uniquely through the unit by $L\dashv K$. Transposing back gives a unique factorization of $h$ through $q_a$. Thus $q_a$ is the required [coequalizer](../../../../../../coequalizer.md). This proves both directions of the [Left adjoint to the Eilenberg-Moore comparison functor](../../../../../../left-adjoint-to-the-eilenberg-moore-comparison-functor.md) criterion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8](../../8.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
