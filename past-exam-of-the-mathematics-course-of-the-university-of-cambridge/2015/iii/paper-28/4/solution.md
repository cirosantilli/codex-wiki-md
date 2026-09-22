<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Here a divisor is a [modulus of a number field](../../../../../modulus-of-a-number-field.md), rather than an arbitrary real-weighted divisor. Write

$$
\mathfrak c=\mathfrak c_0\mathfrak c_\infty,\qquad \mathfrak c_0=\prod_{\mathfrak p}\mathfrak p^{m_{\mathfrak p}},
$$

where $\mathfrak c_0$ is a nonzero [integral ideal](../../../../../integral-ideal.md), the finite multiplicities $m_{\mathfrak p}$ are nonnegative integers, and $\mathfrak c_\infty$ is a set of real [Archimedean places](../../../../../archimedean-place.md). The [multiplicity of a place in a modulus](../../../../../multiplicity-of-a-place-in-a-modulus.md) is $m_v(\mathfrak c)=m_{\mathfrak p}$ at the finite place corresponding to $\mathfrak p$, is $1$ at a real place in $\mathfrak c_\infty$, and is $0$ at every other infinite place. In particular complex places have multiplicity $0$.

Let $I_{\mathfrak c}$ be the group of nonzero [fractional ideals](../../../../../fractional-ideal.md) prime to $\mathfrak c_0$. Put

$$
K_{\mathfrak c,1}^{\times}=\{a\in K^{\times}:v_{\mathfrak p}(a-1)\geq m_{\mathfrak p}\text{ for }\mathfrak p\mid\mathfrak c_0,\quad \sigma_v(a)>0\text{ for }v\in\mathfrak c_\infty\}.
$$

Let $P_{\mathfrak c}$ consist of the [principal ideals](../../../../../principal-ideal.md) $(a)$ with $a\in K_{\mathfrak c,1}^{\times}$. The [generalized ideal class group](../../../../../ray-class-group.md) is the [ray class group](../../../../../ray-class-group.md)

$$
\boxed{H_{\mathfrak c}=I_{\mathfrak c}/P_{\mathfrak c}.}
$$

Let $U=\mathcal O_K^{\times}$ be the [unit group](../../../../../unit-group.md), let $U_{\mathfrak c}=U\cap K_{\mathfrak c,1}^{\times}$ be the group of [ray units](../../../../../ray-unit.md), and define the [residue and signature group of a modulus](../../../../../residue-and-signature-group-of-a-modulus.md)

$$
G_{\mathfrak c}=(\mathcal O_K/\mathfrak c_0)^{\times}\times\{\pm1\}^{\mathfrak c_\infty}.
$$

The first factor is omitted when $\mathfrak c_0=\mathcal O_K$. There is a [group homomorphism](../../../../../group-homomorphism.md) $\rho:U\to G_{\mathfrak c}$ recording the unit's finite residues and its signs. Its [kernel](../../../../../kernel-of-a-linear-map.md) is $U_{\mathfrak c}$.

Let $P^{\mathfrak c}$ consist of all [principal fractional ideals](../../../../../principal-fractional-ideal.md) prime to $\mathfrak c_0$, and put $R_{\mathfrak c}=P^{\mathfrak c}/P_{\mathfrak c}$. The two [short exact sequences](../../../../../short-exact-sequence.md) are

$$
\boxed{1\longrightarrow U/U_{\mathfrak c}\xrightarrow{\rho}G_{\mathfrak c}\longrightarrow R_{\mathfrak c}\longrightarrow1,}
$$

and

$$
\boxed{1\longrightarrow R_{\mathfrak c}\longrightarrow H_{\mathfrak c}\longrightarrow\operatorname{Cl}(\mathcal O_K)\longrightarrow1.}
$$

For the first [short exact sequence](../../../../../short-exact-sequence.md), [weak approximation for number fields](../../../../../weak-approximation-for-number-fields.md) realizes every choice of finite unit residues and real signs by some $a\in K^{\times}$ prime to $\mathfrak c_0$. Send that data to the class of $(a)$ in $R_{\mathfrak c}$. Changing $a$ without changing its residues and signs multiplies it by an element of $K_{\mathfrak c,1}^{\times}$, so the map is well-defined. Its [kernel](../../../../../kernel-of-a-linear-map.md) consists exactly of data arising from units: if $(a)=(b)$ with $b\in K_{\mathfrak c,1}^{\times}$, then $a/b\in U$. This gives $R_{\mathfrak c}\cong G_{\mathfrak c}/\rho(U)$. For the second [short exact sequence](../../../../../short-exact-sequence.md), forget the ray conditions. Its [kernel](../../../../../kernel-of-a-linear-map.md) is $R_{\mathfrak c}$, and [weak approximation for number fields](../../../../../weak-approximation-for-number-fields.md) gives a representative prime to $\mathfrak c_0$ for every [ideal class](../../../../../ideal-class.md). These are the two parts of the [ray class exact sequence](../../../../../ray-class-exact-sequence.md).

For $K=\mathbb Q(\sqrt{15})$, the [ring of integers of a quadratic field](../../../../../ring-of-integers-of-a-quadratic-field.md) is $\mathcal O_K=\mathbb Z[\sqrt{15}]$. The finite modulus is trivial and both real places occur, so $H_{\mathfrak c}$ is the [narrow ideal class group](../../../../../narrow-ideal-class-group.md) and $G_{\mathfrak c}=\{\pm1\}^2$. The two [field embeddings](../../../../../field-embedding.md) send $\sqrt{15}$ to $\sqrt{15}$ and $-\sqrt{15}$. The given unit $\epsilon=4+\sqrt{15}$ is positive at both places, since $4-\sqrt{15}>0$; the unit $-1$ is negative at both. Thus the [unit signature map](../../../../../unit-signature-map.md) has image

$$
\rho(U)=\{(+,+),(-,-)\},\qquad |R_{\mathfrak c}|=\frac42=2.
$$

The given [ideal class group](../../../../../ideal-class-group.md) has order $2$. The second [short exact sequence](../../../../../short-exact-sequence.md) therefore gives

$$
\boxed{|H_{\mathfrak c}|=2\cdot2=4.}
$$

To determine the group structure, retain the ideal $\mathfrak p=(2,1+\sqrt{15})$ that generates the ordinary [ideal class group](../../../../../ideal-class-group.md). We have $\mathfrak p^2=(2)$: all generators $4$, $2(1+\sqrt{15})$ and $(1+\sqrt{15})^2$ lie in $(2)$, while

$$
(1+\sqrt{15})^2-2(1+\sqrt{15})-3\cdot4=2
$$

puts $2$ in $\mathfrak p^2$. Since $2$ is [totally positive](../../../../../totally-positive-element-of-a-number-field.md), $[\mathfrak p]^2=1$ in the [narrow ideal class group](../../../../../narrow-ideal-class-group.md). Its image in the ordinary [ideal class group](../../../../../ideal-class-group.md) is nontrivial, so $[\mathfrak p]$ has order exactly $2$.

The class of the [principal ideal](../../../../../principal-ideal.md) $(\sqrt{15})$ is a nontrivial element of $R_{\mathfrak c}$. Its two signs are $(+,-)$, and multiplying by a unit can only reverse both signs or neither, so no generator of this ideal is [totally positive](../../../../../totally-positive-element-of-a-number-field.md). Its square is $(15)$, which does have a [totally positive](../../../../../totally-positive-element-of-a-number-field.md) generator. Thus $[(\sqrt{15})]$ is another element of order $2$, distinct from $[\mathfrak p]$ because its ordinary [ideal class](../../../../../ideal-class.md) is trivial. These two elements are independent and generate all four classes. Consequently

$$
\boxed{H_{\mathfrak c}\cong(\mathbb Z/2\mathbb Z)^2.}
$$

The nontrivial ordinary [ideal class](../../../../../ideal-class.md) already has a lift of order $2$, so the extension in the second [short exact sequence](../../../../../short-exact-sequence.md) splits; it cannot be cyclic of order $4$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
