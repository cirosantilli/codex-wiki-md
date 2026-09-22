<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $K$ be a [number field](../../../../../number-field.md) of degree $d$, and normalize its [absolute values](../../../../../absolute-value.md) so that the [product formula](../../../../../product-formula.md) is $\prod_v|a|_v^{n_v}=1$ for $a\ne0$, where $n_v=[K_v:\mathbb Q_v]$; at a complex place use the ordinary modulus with weight two. For $P=[a_0:\cdots:a_N]$, define

$$
\boxed{H(P)=\prod_{v\in M_K}\max_i|a_i|_v^{n_v/d},\qquad h(P)=\log H(P).}
$$

Only finitely many factors differ from one. Rescaling all coordinates multiplies the local maxima by $|a|_v$, whose weighted product is one, so the [projective height](../../../../../projective-height.md) is well-defined. It is at least one by comparison with any nonzero coordinate. On enlarging $K$ to $L$, the identity $\sum_{w\mid v}[L_w:\mathbb Q_v]=[L:K][K_v:\mathbb Q_v]$ makes the normalized product unchanged. Thus this is an absolute height on algebraic projective points. For coprime rational integer coordinates it is simply their maximum absolute value.

For a projective variety $V/K$ and an embedding $i:V\hookrightarrow\mathbb P^N$, take $h_i=h\circ i$. Changing the basis of the same projective linear system changes the height by a bounded amount: the coordinate transformation and its inverse have fixed local coefficient bounds, equal to one outside finitely many places. If $L$ is ample and $L^m$ is very ample, set $h_L=m^{-1}h_i$ for an embedding from $L^m$, up to a bounded function. A general line bundle can be written $(L\otimes A)\otimes A^{-1}$ with both $A$ and $L\otimes A$ very ample, defining its height as the difference of their embedding heights.

This is the [Weil height machine](../../../../../weil-height-machine.md), with

$$
h_{L\otimes M}=h_L+h_M+O(1),\qquad h_{\phi^*L}=h_L\circ\phi+O(1).
$$

The first relation follows from the Segre embedding, whose local maximum is the product of the two maxima; tensor powers similarly use the Veronese embedding. The second follows by pulling back the defining sections. These constructions make the choices equivalent modulo bounded functions. For a fixed homogeneous morphism with no base point, upper local height bounds come from its coefficients, and lower bounds from the [Projective Nullstellensatz](../../../../../projective-nullstellensatz.md) expressing coordinate powers in the ideal of its defining forms. The constants are one outside a finite set of places. This gives the uniform bounded errors and shows why heights belong to line-bundle classes rather than being independent of every projective embedding.

The [Northcott lemma](../../../../../northcott-theorem.md) states that for fixed $B$ and $D$, the algebraic points of $\mathbb P^N$ with $H(P)\leq B$ and $[\mathbb Q(P):\mathbb Q]\leq D$ form a finite set. In particular the $K$-rational points of bounded projective height are finite. Here is a proof, including the degree bound.

First let $\alpha$ have degree $e\leq D$ and $H(\alpha)=H([1:\alpha])\leq B$. Write its primitive minimal polynomial as $a_e\prod_{j=1}^e(T-\alpha_j)$, with positive integer $a_e$. The [height-Mahler measure formula](../../../../../height-mahler-measure-formula.md) is

$$
H(\alpha)^e=a_e\prod_{j=1}^e\max(1,|\alpha_j|).
$$

Its finite-place part follows from multiplicativity of the nonarchimedean polynomial coefficient norm: a primitive integer polynomial has norm one at each prime, so factoring it bounds the product of the roots' local maxima by the inverse leading-coefficient norm. The archimedean part is the displayed product over conjugates. Combining them with the product formula gives the identity.

Expanding the polynomial now bounds each integer coefficient by

$$
|a_k|\leq\binom ek a_e\prod_j\max(1,|\alpha_j|)\leq2^D B^D.
$$

There are finitely many degrees and finitely many such integer coefficient lists, each with finitely many roots. Hence there are only finitely many possible $\alpha$. This proves the [minimal-polynomial coefficient proof of Northcott finiteness](../../../../../minimal-polynomial-coefficient-proof-of-northcott-finiteness.md) for algebraic numbers.

On the projective chart $a_j\ne0$, each ratio $\alpha_i=a_i/a_j$ has degree at most the point's field degree and

$$
H(\alpha_i)\leq\prod_v\left(\frac{\max_k|a_k|_v}{|a_j|_v}\right)^{n_v/d}=H(P).
$$

The equality uses the product formula. Each coordinate ratio therefore belongs to a finite set, and there are finitely many charts. This proves the projective [Northcott theorem](../../../../../northcott-theorem.md). Restricting to $V$ gives the result for a chosen embedding. For an ample line-bundle height, the comparison $mh_L=h_i+O(1)$ reduces its bounded-height sets to this case.

Both qualifications matter: a degree bound cannot be dropped, since infinitely many [roots of unity](../../../../../root-of-unity.md) have height one; and the finiteness assertion need not hold for a nonample line bundle, such as the trivial bundle's bounded height on a variety with infinitely many rational points.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
