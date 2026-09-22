<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [regular category](../../../../../regular-category.md) has [finite limits](../../../../../finite-limit.md), every morphism factors through its [image of a morphism in a regular category](../../../../../image-of-a-morphism-in-a-regular-category.md) as a [regular epimorphism](../../../../../regular-epimorphism.md) followed by a [monomorphism](../../../../../monomorphism.md), and regular epimorphisms are stable under every [pullback in a category](../../../../../pullback-category-theory.md). A cover is a [strong epimorphism](../../../../../strong-epimorphism.md). Every regular epimorphism is strong: if $e$ is the coequalizer of $r,s$ and a square has $e$ on the left and a monomorphism $m$ on the right, monicity shows that the upper arrow coequalizes $r,s$. It therefore factors through $e$, and the epimorphism property of $e$ shows that this factor is the required diagonal. Conversely, factor a strong epimorphism $f$ as $f=me$ with $e$ regular epic and $m$ monic. The lifting property gives a two-sided inverse to $m$, so $m$ is an isomorphism and $f$ is regular epic. Thus regular epimorphisms and covers coincide.

Let $L:\mathcal C\to\mathcal D$ be the left-exact [reflector](../../../../../reflector.md) and let $m:A'\hookrightarrow A$. Since $L$ preserves finite limits, $Lm$ is monic. Define $c_A(A')$ as the pullback

$$
\begin{array}{ccc}
c_A(A')&\longrightarrow&LA'\\
\downarrow&&\downarrow Lm\\
A&\xrightarrow{\eta_A}&LA.
\end{array}
$$

Naturality of the unit supplies a map $A'\to c_A(A')$ over $A$, proving $A'\leq c_A(A')$. A factorization $A'\leq A''$ induces $LA'\leq LA''$ and therefore $c_A(A')\leq c_A(A'')$, so $c_A$ is order-preserving.

Apply $L$ to the defining pullback. Left exactness and the fact that $L\eta_A:LA\to LLA$ is an isomorphism identify $L(c_A(A'))$ with $LA'$. Pulling back once more therefore gives

$$
c_A(c_A(A'))\cong c_A(A').
$$

For a map $f:B\to A$, left exactness identifies $L(f^*A')$ with $(Lf)^*(LA')$. Pasting the two pullback squares then yields

$$
c_B(f^*A')\cong f^*c_A(A'),
$$

so this [closure operation induced by a left-exact reflector](../../../../../closure-operation-induced-by-a-left-exact-reflector.md) commutes with pullback.

Assume $A$ lies in $\mathcal D$, so $\eta_A$ is an isomorphism. If $A'$ also lies in $\mathcal D$, its unit is an isomorphism and the defining square gives $c_A(A')\cong A'$. Conversely, if $A'$ is closed, that square expresses $A'$ as a finite limit of $A$, $LA'$, and $LA$, all fixed by $L$. Fixed objects of a [left-exact reflective subcategory](../../../../../left-exact-reflective-subcategory.md) are closed under finite limits, so $A'$ belongs to $\mathcal D$.

Finally suppose $\mathcal C$ is regular. The fixed objects have finite limits. For $f:A\to B$ in $\mathcal D$, factor it in $\mathcal C$ as

$$
A\xrightarrow{e}I\xrightarrow{m}B.
$$

Applying $L$ gives $A\xrightarrow{Le}LI\xrightarrow{Lm}B$. The map $Le$ is regular epic because a left adjoint preserves the coequalizer presenting $e$, and $Lm$ is monic because $L$ is left exact. Thus $\mathcal D$ has image factorizations. Their image subobject is the closure $c_B(I)$. A map in $\mathcal D$ is regular epic exactly when this closure is all of its codomain. Images in $\mathcal C$ commute with pullback, and the closure operation also commutes with pullback, so this condition is pullback-stable. Hence $\mathcal D$ is regular, as stated by the [left-exact reflective subcategory of a regular category](../../../../../left-exact-reflective-subcategory-of-a-regular-category.md) theorem.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
