<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The requested representation is the left [coset action](../../../../../coset-action.md)

$$
\rho:G\longrightarrow\operatorname{Sym}(G/H),\qquad
\rho(g)(xH)=gxH.
$$

It is well defined because equal [cosets](../../../../../coset.md) remain equal after multiplication by $g$, and $\rho(gg')=\rho(g)\rho(g')$. It is transitive. For $H=1$ it is the left regular action; for general $H$ it is the associated transitive [coset](../../../../../coset.md) representation.

Its kernel is the [normal core of a subgroup](../../../../../core-group-theory.md)

$$
N=\bigcap_{x\in G}xHx^{-1}.
$$

Indeed, $g$ fixes every $xH$ precisely when $x^{-1}gx\in H$ for every $x$. Thus $N\lhd G$ and $N\leq H$. If $[G:H]=i<\infty$, the image lies in the finite symmetric [group](../../../../../group-split.md) $S_i$, so

$$
\boxed{[G:N]\leq i!,\qquad [H:N]=\frac{[G:N]}i\leq(i-1)!.}
$$

In particular $N$ has finite index in $H$.

For [Higman group as an amalgam of iterated HNN extensions](../../../../../higman-group-as-an-amalgam-of-iterated-hnn-extensions.md), use the cyclic squaring presentation

$$
\mathcal H=\langle a,b,c,d\mid
a^{-1}ba=b^2,\ b^{-1}cb=c^2,\ c^{-1}dc=d^2,\ d^{-1}ad=a^2\rangle.
$$

First form $L=\langle b,c\mid b^{-1}cb=c^2\rangle$, an [HNN extension](../../../../../hnn-extension.md) of the infinite [cyclic group](../../../../../cyclic-group.md) $\langle c\rangle$. Its base embeds, so $c$ has infinite order; $b$ has infinite order as well, since the [homomorphism](../../../../../homomorphism.md) $L\to\mathbb Z$ sending $b\mapsto1,c\mapsto0$ is onto. Consequently $\langle b\rangle$ and $\langle b^2\rangle$ are isomorphic infinite cyclic [subgroups](../../../../../subgroup.md). Adjoining the [stable letter](../../../../../stable-letter.md) $a$ with $a^{-1}ba=b^2$ gives

$$
P=\langle a,b,c\mid a^{-1}ba=b^2,\ b^{-1}cb=c^2\rangle.
$$

We claim $\langle a,c\rangle$ is a rank-two [free group](../../../../../free-group.md). No nonzero power of $c$ belongs to $\langle b\rangle$: applying the map $b\mapsto1,c\mapsto0$ would make that power equal to $1$, contradicting the infinite order of $c$. Thus no nonzero power of $c$ belongs to $\langle b^2\rangle$ either. Any nonempty freely reduced word in $a,c$ that contains $a$ is therefore a reduced HNN sequence: between inverse $a$ letters, a nonzero $c$ power cannot create a pinch. [Britton's lemma](../../../../../britton-s-lemma.md) makes it nonidentity. A word containing only $c$ is nonidentity by the base embedding. This proves the claim.

Likewise

$$
Q=\langle c,d,a\mid c^{-1}dc=d^2,\ d^{-1}ad=a^2\rangle
$$

is obtained from $\langle d,a\mid d^{-1}ad=a^2\rangle$ by adjoining $c$, and its [subgroup](../../../../../subgroup.md) $\langle c,a\rangle$ is free of rank two by the same argument. Form the [amalgamated free product](../../../../../amalgamated-free-product.md) $P*_{\langle a,c\rangle}Q$, identifying these two free [subgroups](../../../../../subgroup.md) generator by generator. Its presentation is exactly that of $\mathcal H$. The component embeddings allowed in the question show that it contains $P$, hence is infinite. It has four [group generators](../../../../../generator-of-a-group.md) and four relators, so it is finitely presented.

To show that this [Higman group](../../../../../higman-group.md) has no nontrivial finite quotient, consider any finite image and the orders of the four generator images. A relation $x^{-1}yx=y^2$ makes $y$ and $y^2$ have the same order, so every generator order is odd. Suppose one is nontrivial, and let $p$ be the smallest prime dividing any of the four orders. Choose a generator $y$ whose order is divisible by $p$, with predecessor $x$ satisfying the displayed relation. Iterating conjugation $|x|$ times gives

$$
y^{2^{|x|}}=y,\qquad 2^{|x|}\equiv1\pmod p.
$$

The [multiplicative order](../../../../../multiplicative-order.md) $d$ of $2$ modulo $p$ thus divides $|x|$. Also $d\mid p-1$ and $d>1$, since $2\not\equiv1\pmod p$. Any prime divisor of $d$ is smaller than $p$ and divides the order of $x$, contradicting minimality of $p$. Hence every generator image is trivial, so every finite image is trivial. A proper finite-index [subgroup](../../../../../subgroup.md) would give a nontrivial transitive finite [coset](../../../../../coset.md) image, which is impossible. Therefore **$\mathcal H$ is infinite and finitely presented, with no proper finite-index [subgroups](../../../../../subgroup.md)**.

A [maximal normal subgroup](../../../../../maximal-normal-subgroup.md) is a proper [normal subgroup](../../../../../normal-subgroup.md) $M\lhd G$ with no [normal subgroup](../../../../../normal-subgroup.md) strictly between $M$ and $G$. To prove that [finitely generated groups have maximal proper normal subgroups](../../../../../finitely-generated-groups-have-maximal-proper-normal-subgroups.md), fix a proper [normal subgroup](../../../../../normal-subgroup.md) $K$ and order the proper [normal subgroups](../../../../../normal-subgroup.md) containing $K$ by inclusion. For a chain, its union is normal and contains $K$. It is still proper: if the union were all of $G$, each element of a finite generating set would lie in some chain member, and the chain order would put all these finitely many [group generators](../../../../../generator-of-a-group.md) in one member. That member would equal $G$, a contradiction. The [Zorn lemma](../../../../../zorn-s-lemma.md) therefore supplies a maximal proper [normal subgroup](../../../../../normal-subgroup.md) $M$ containing $K$.

Apply this to $\mathcal H$ and $K=1$. By the normal-subgroup correspondence, $\mathcal H/M$ is nontrivial and simple. It is finitely generated as a quotient of $\mathcal H$. It cannot be finite, since $\mathcal H$ has no nontrivial finite quotients. Thus

$$
\boxed{\text{there exists an infinite finitely generated simple group}.}
$$

The final assertion for arbitrary proper [subgroups](../../../../../subgroup.md) is false. Take $G=S_3$ and $H=\langle(12)\rangle$. If a [normal subgroup](../../../../../normal-subgroup.md) contained $H$, it would contain all conjugate transpositions, which generate $S_3$, so it would equal $G$. Hence this proper [subgroup](../../../../../subgroup.md) lies in no proper [normal subgroup](../../../../../normal-subgroup.md), and in particular in no maximal [normal subgroup](../../../../../normal-subgroup.md). The maximal-normal existence result requires the starting [subgroup](../../../../../subgroup.md) itself to be normal.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
