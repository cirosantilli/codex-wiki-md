<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $B$ be a [subterminal object](../../../../../subterminal-object.md) in a [Cartesian closed category](../../../../../cartesian-closed-category.md). For every $X$ and $A$, the [exponential object](../../../../../exponential-object.md) adjunction gives

$$
\mathcal C(X,B^A)\cong\mathcal C(X\times A,B).
$$

The set on the right has at most one element because $B$ is subterminal. Hence $B^A$ is subterminal, proving that $\operatorname{Sub}(1)$ is an [exponential ideal](../../../../../exponential-ideal.md).

Now let $\mathcal D\subseteq\mathcal C$ be [reflective](../../../../../reflective-subcategory.md), with reflector $L$ and unit $\eta_A:A\to LA$. Recall the useful form of its universal property: an object $D$ lies in $\mathcal D$ precisely when every map $f:A\to D$ factors uniquely through $\eta_A$.

Suppose first that $\mathcal D$ is an exponential ideal. Reflective subcategories are closed under ambient limits, so $LA\times LB$ lies in $\mathcal D$. Given $f:A\times B\to D$ with $D\in\mathcal D$, curry in the first variable to obtain $A\to D^B$. Since $D^B\in\mathcal D$, this factors uniquely through $\eta_A$ and uncurries to $LA\times B\to D$. Curry once more, now in $B$; since $D^{LA}\in\mathcal D$, the result factors uniquely through $\eta_B$. Thus every $f$ factors uniquely through

$$
\eta_A\times\eta_B:A\times B\longrightarrow LA\times LB.
$$

This makes $LA\times LB$ a reflection of $A\times B$, so uniqueness of reflections gives

$$
L(A\times B)\cong LA\times LB.
$$

Conversely, suppose $L$ preserves binary products, and take $D\in\mathcal D$. To prove $D^A\in\mathcal D$, start with $f:X\to D^A$ and let $\widetilde f:X\times A\to D$ be its transpose. Since $D$ is reflective, $\widetilde f$ factors uniquely through

$$
\eta_{X\times A}:X\times A\longrightarrow L(X\times A)\cong LX\times LA.
$$

Composing the resulting map $LX\times LA\to D$ with $1_{LX}\times\eta_A$ and currying produces an extension $LX\to D^A$ of $f$. Product preservation identifies the unit on $LX\times A$ with $1_{LX}\times\eta_A$, so the same universal property proves uniqueness. Therefore $D^A$ is reflective, and $\mathcal D$ is an exponential ideal. This proves the [reflector product criterion for an exponential ideal](../../../../../reflector-product-criterion-for-an-exponential-ideal.md).

Finally consider the [arrow category](../../../../../arrow-category.md) $[\mathbf2,\mathbf{Set}]$. For arrows $a:A_0\to A_1$ and $b:B_0\to B_1$, let

$$
F=\{(u_0,u_1):u_0:A_0\to B_0, u_1:A_1\to B_1, bu_0=u_1a\}.
$$

Then the exponential $b^a$ is the arrow

$$
F\longrightarrow B_1^{A_1},\qquad (u_0,u_1)\longmapsto u_1.
$$

Indeed, a commutative square from $c:C_0\to C_1$ to this arrow is, after currying, exactly a commutative square $a\times c\to b$. This establishes the required exponential adjunction and proves that $[\mathbf2,\mathbf{Set}]$ is cartesian closed.

If $b$ is injective, two elements $(u_0,u_1)$ and $(u'_0,u_1)$ of $F$ have

$$
bu_0=u_1a=bu'_0,
$$

so injectivity gives $u_0=u'_0$. Hence $F\to B_1^{A_1}$ is injective. The [category of injective functions](../../../../../category-of-injective-functions.md) is therefore an exponential ideal in the arrow category. Its terminal object and binary products are inherited pointwise, so these same exponential objects make $\operatorname{Mono}(\mathbf{Set})$ cartesian closed.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
