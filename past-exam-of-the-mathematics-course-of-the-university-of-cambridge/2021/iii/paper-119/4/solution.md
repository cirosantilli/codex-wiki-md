<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [monad](../../../../../monad.md) on $\mathcal C$ is an endofunctor $T$ with natural transformations

$$
\eta:1_{\mathcal C}\Rightarrow T,
\qquad
\mu:T^2\Rightarrow T
$$

satisfying $\mu\,T\mu=\mu\,\mu T$ and $\mu\,T\eta=1_T=\mu\,\eta T$. Its [Eilenberg-Moore category](../../../../../eilenberg-moore-category.md) $\mathcal C^T$ has [algebras for a monad](../../../../../algebra-for-a-monad.md) $(A,a:TA\to A)$ satisfying

$$
a\eta_A=1_A,
\qquad
aT(a)=a\mu_A,
$$

and [morphisms of algebras for a monad](../../../../../morphism-of-algebras-for-a-monad.md) $f:(A,a)\to(B,b)$ satisfying $fa=bT(f)$.

The [Kleisli category](../../../../../kleisli-category.md) $\mathcal C_T$ has the objects of $\mathcal C$ and

$$
\mathcal C_T(A,B)=\mathcal C(A,TB).
$$

Its identity is $\eta_A$, while the composite of $f:A\to TB$ and $g:B\to TC$ is $\mu_C T(g)f$. The [free functor into a Kleisli category](../../../../../free-functor-into-a-kleisli-category.md) $F_T:\mathcal C\to\mathcal C_T$ is the identity on objects and sends $f:A\to B$ to $\eta_Bf$.

On the [functor category](../../../../../functor-category.md) $[\mathcal D,\mathcal C]$, postcomposition gives the [pointwise monad on a functor category](../../../../../pointwise-monad-on-a-functor-category.md)

$$
T_*(F)=TF,
\qquad
(\eta_*)_F=\eta F,
\qquad
(\mu_*)_F=\mu F.
$$

The monad laws hold componentwise. A $T_*$-algebra is a functor $F:\mathcal D\to\mathcal C$ with a natural transformation $a:TF\to F$ whose components are $T$-algebras. Naturality says precisely that every $F(u)$ is an algebra morphism. Hence sending $(F,a)$ to the lifted functor $\mathcal D\to\mathcal C^T$ gives an isomorphism, and in particular an equivalence,

$$
[\mathcal D,\mathcal C]^{T_*}\simeq[\mathcal D,\mathcal C^T].
$$

On $[\mathcal C,\mathcal D]$, precomposition gives the [precomposition monad on a functor category](../../../../../precomposition-monad-on-a-functor-category.md)

$$
T^*(G)=GT,
\qquad
(\eta^*)_G=G\eta,
\qquad
(\mu^*)_G=G\mu.
$$

A $T^*$-algebra is a natural transformation $a:GT\to G$ satisfying $aG\eta=1_G$ and $a(aT)=aG\mu$. From it define $\bar G:\mathcal C_T\to\mathcal D$ by

$$
\bar G(A)=G(A),
\qquad
\bar G(f:A\to TB)=a_BG(f).
$$

The two algebra laws say exactly that $\bar G$ preserves identities and Kleisli composition, and $\bar G F_T=G$. Conversely, a factorization $G=\bar G F_T$ gives

$$
a_A=\bar G(1_{TA}:TA\to TA),
$$

where $1_{TA}$ represents a Kleisli arrow $TA\to A$. These constructions are inverse on objects and morphisms, so

$$
\boxed{[\mathcal C,\mathcal D]^{T^*}\simeq[\mathcal C_T,\mathcal D].}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
