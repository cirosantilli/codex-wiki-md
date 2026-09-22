<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The exactness axiom of a [generalized cohomology theory](../../../../../generalized-cohomology-theory.md) gives a natural [long exact sequence](../../../../../long-exact-sequence.md) for each [CW pair](../../../../../cw-pair.md):

$$
\cdots\longrightarrow h^n(X,A)\xrightarrow{j^*}h^n(X)
\xrightarrow{i^*}h^n(A)\xrightarrow{\delta}h^{n+1}(X,A)\longrightarrow\cdots.
$$

For $(X,X)$, the restriction $h^n(X)\to h^n(X)$ is the identity. Its preceding relative-to-absolute map has zero image. The previous connecting map is zero too, since it follows the surjective identity in degree $n-1$. Exactness at the relative group therefore makes its map both injective and zero, giving

$$
\boxed{h^n(X,X)=0\quad\text{for every }n,}
$$

in particular $h^n(x_0,x_0)=0$. No dimension axiom is being used; a generalized theory can have nonzero $h^n(x_0)$ in many degrees.

The wedge-product notation for pairs here means the [smash product of CW pairs](../../../../../smash-product-of-cw-pairs.md),

$$
(X,A)\wedge(Y,B)=\bigl(X\times Y,(A\times Y)\cup(X\times B)\bigr).
$$

Its quotient is the based [smash product](../../../../../smash-product.md) $(X/A)\wedge(Y/B)$. A multiplicative theory has an external product

$$
h^k(X,A)\otimes h^m(Y,B)\longrightarrow
h^{k+m}\bigl(X\times Y,(A\times Y)\cup(X\times B)\bigr).
$$

If the two spaces are the same, pullback by the diagonal gives the [relative cup product](../../../../../relative-cup-product.md) in $h^{k+m}(X,A\cup B)$. This is different from the wedge sum of two based spaces.

First read the covering subcomplexes as pointed subcomplexes, so $x_0\in A_j$. Contractibility makes the inclusion $\{x_0\}\hookrightarrow A_j$ a [homotopy equivalence](../../../../../homotopy-equivalence.md), and thus $h^r(A_j,x_0)=0$ in every degree, by exactness and [homotopy invariance of cohomology](../../../../../homotopy-invariance-of-cohomology.md). The relative exact sequence for the triple $\{x_0\}\subseteq A_j\subseteq X$ gives

$$
h^{r_j}(X,A_j)\longrightarrow h^{r_j}(X,x_0)
\longrightarrow h^{r_j}(A_j,x_0)=0.
$$

Consequently each homogeneous $w_j$ lifts to $v_j\in h^{r_j}(X,A_j)$. Repeated relative multiplication gives

$$
v_1\smile\cdots\smile v_l\in
h^{r_1+\cdots+r_l}\left(X,\bigcup_{j=1}^l A_j\right)=h^{r_1+\cdots+r_l}(X,X)=0.
$$

Naturality maps this product to the product of the $w_j$ in $h^*(X,x_0)$. Therefore

$$
\boxed{w_1\cdots w_l=0.}
$$

For nonhomogeneous classes the same conclusion follows by distributivity. This is [nilpotence from a contractible subcomplex cover](../../../../../nilpotence-from-a-contractible-subcomplex-cover.md).

There is an alternative sufficient convention: if $X$ is path connected, the $A_j$ need not contain $x_0$. The absolute image $\bar w$ of a reduced class restricts to zero at $x_0$, hence at any other point since the point inclusions are homotopic along a path. On a nonempty contractible $A_j$ it therefore restricts to zero, so exactness lifts $\bar w_j$ to $h^*(X,A_j)$. Their relative product vanishes as above. The map $h^*(X,x_0)\to h^*(X)$ is injective: restriction to the basepoint is split surjective by the map $X\to\mathrm{pt}$, making the previous connecting map zero. Thus vanishing of the absolute product gives vanishing of the reduced product too.

Without either the pointed-subcomplex or connectedness convention, the printed conclusion is false. Take $X=\{x_0,x_1\}$ covered by its two singleton subcomplexes and $h^*=H^*(-;\mathbb Z)$. Both subcomplexes are contractible, but $H^0(X,x_0)$ contains the function $w$ with values $0,1$. Pointwise multiplication gives $w^2=w\ne0$. This states precisely the needed interpretation rather than assuming a contractible component lies in the basepoint component.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
