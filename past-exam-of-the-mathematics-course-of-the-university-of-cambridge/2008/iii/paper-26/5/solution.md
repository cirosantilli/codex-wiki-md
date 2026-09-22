<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Since the full [endofunctor](../../../../../endofunctor.md) subcategory contains $1$ and is closed under composition, $1,T^2,T^3$ all belong to it. Terminality supplies unique [natural transformations](../../../../../natural-transformation.md) $\eta:1\to T$ and $\mu:T^2\to T$. The [monad](../../../../../monad.md) unit laws compare arrows $T\to T$, both necessarily the unique endomorphism, namely the identity. The associativity law compares arrows $T^3\to T$, again necessarily equal. Every [monad](../../../../../monad.md) structure uses these two unique arrows, so $\boxed{T\text{ has a unique monad structure}}$.

For a [monad](../../../../../monad.md) $S$ with underlying [functor](../../../../../functor.md) in the subcategory, the unique $\alpha:S\to T$ is a [monad morphism](../../../../../monad-morphism.md). Its unit and multiplication compatibility compare, respectively, arrows $1\to T$ and $S^2\to T$ and therefore follow from terminality. A $T$-algebra $a:TX\to X$ restricts to the $S$-algebra $b=a\alpha_X$. The unit law is immediate. For multiplication, naturality and the monad-morphism law give

$$
bSb=aTa\,T\alpha_X\,\alpha_{SX}=a\mu^T_X T\alpha_X\alpha_{SX}=a\alpha_X\mu^S_X=b\mu^S_X.
$$

An algebra morphism for $T$ also commutes with the restricted action by naturality of $\alpha$. Keeping underlying objects and arrows gives the required [functor](../../../../../functor.md) $\mathcal C^T\to\mathcal C^S$.

Now define $TA$ to be the set of [ultrafilters](../../../../../ultrafilter.md) on $A$, and for $f:A\to B$ define

$$
Tf(\mathcal U)=\{V\subseteq B:f^{-1}(V)\in\mathcal U\}.
$$

Inverse images preserve inclusions, intersections and complements, so this is an [ultrafilter](../../../../../ultrafilter.md); composition of inverse images makes $T$ a [functor](../../../../../functor.md). There are no [ultrafilters](../../../../../ultrafilter.md) on the empty set. Every [ultrafilter](../../../../../ultrafilter.md) on a disjoint binary union chooses exactly one summand, and restriction to that summand gives an [ultrafilter](../../../../../ultrafilter.md) there; extension back is inverse to restriction. Hence $T(A\amalg B)\cong TA\amalg TB$ canonically, and $T$ preserves finite [coproducts](../../../../../coproduct.md), including the empty one.

Let $H$ be any other finite-coproduct-preserving [endofunctor](../../../../../endofunctor.md). For $x\in HA$, put

$$
\alpha_A(x)=\{U\subseteq A:x\in\operatorname{im}(H(U\hookrightarrow A))\}.
$$

The decomposition $A=U\amalg U^c$ and [coproduct](../../../../../coproduct.md) preservation show that exactly one of $U,U^c$ belongs. Refining two subsets into the four disjoint parts $U\cap V,U\setminus V,V\setminus U,(U\cup V)^c$ shows that an element lying in both indicated summands lies in their intersection summand. The same refinement for $U\subseteq V$ proves upward closure. Thus $\alpha_A(x)$ is an [ultrafilter](../../../../../ultrafilter.md). For $f:A\to B$, decomposition by $f^{-1}(V)$ and its complement shows

$$
V\in\alpha_B(Hf(x))\iff f^{-1}(V)\in\alpha_A(x),
$$

proving naturality.

For uniqueness, suppose $\beta:H\to T$ is natural. Since $T1$ is a singleton, naturality on the two inclusions $1\to2$ forces $\beta_2$ to send every element in each of the two $H1$ summands of $H2$ to the corresponding [principal ultrafilter](../../../../../principal-ultrafilter.md). Apply naturality to the characteristic map $\chi_U:A\to2$. It gives $U\in\beta_A(x)$ precisely when $H\chi_U(x)$ lies in the selected summand, which by the decomposition is precisely when $x$ lies in $HU\subseteq HA$. Hence $\beta_A=\alpha_A$ for every $A$. Therefore

$$
\boxed{T\text{ is terminal and }TA=\operatorname{Ult}(A).}
$$

This proves [ultrafilter functor](../../../../../ultrafilter-functor.md). For clarity, the resulting unit sends $a$ to its [principal ultrafilter](../../../../../principal-ultrafilter.md); multiplication sends an [ultrafilter](../../../../../ultrafilter.md) $\mathfrak U$ on $\operatorname{Ult}(A)$ to the [ultrafilter](../../../../../ultrafilter.md) whose members are $U$ with $\{\mathcal V:U\in\mathcal V\}\in\mathfrak U$. Naturality and the [monad](../../../../../monad.md) laws for these formulas also follow from the terminal construction.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
