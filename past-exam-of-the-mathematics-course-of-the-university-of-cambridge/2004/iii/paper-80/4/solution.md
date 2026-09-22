<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**The printed vanishing claim needs the restriction $i\ge1$.** On $C=\mathbb P^1$ with $\mathcal F=\mathcal O$ and $D=n\{\infty\}$, Question 3 gives $h^0(\mathcal F(D))=n+1$ for every $n\ge0$. Thus no bound on the [degree of a divisor](../../../../../degree-of-a-divisor.md) can force vanishing in degree zero. We prove finiteness in every degree and the corrected vanishing in every positive degree, uniformly over all [divisors on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) of large degree.

First take a [finite morphism](../../../../../finite-morphism.md) $\pi:C\to\mathbb P^1$ as in Question 3 and put $E=\pi_*\mathcal F$. The [direct image sheaf](../../../../../direct-image-sheaf.md) $E$ is coherent: on an affine chart its module is finitely generated over a finite algebra and hence over the chart's coordinate ring. The two affine-cover [Čech cochain complexes](../../../../../cech-cochain-complex.md) for $\mathcal F$ on $C$ and for $E$ on $\mathbb P^1$ are identical. Therefore

$$
H^i(C,\mathcal F)=H^i(\mathbb P^1,E).
$$

We need an elementary presentation of any [coherent sheaf](../../../../../coherent-sheaf.md) $E$ on the [projective line](../../../../../projective-line.md). Choose finitely many generators on each of its two standard affine charts. A generator on the first chart restricts to an element of the second chart's module localized at $t^{-1}$. Multiplication by a sufficiently large power of $t^{-1}$ brings that element into the second chart's module. Since the transition of $\mathcal O(n)$ is $t^n$, this makes the original generator extend to a [global section](../../../../../global-section.md) of $E(n)$. A generator on the second chart similarly extends after clearing its denominator at $t=0$. Use one common exponent for all the finitely many generators. The extended sections generate $E(n)$ on both charts. Untwisting gives a surjection

$$
P=\mathcal O(-n)^{\oplus r}\longrightarrow E
$$

with coherent kernel $K$. The [long exact sequence in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md) and Question 3 show that $H^1(E)$ is a quotient of the finite-dimensional $H^1(P)$, since $H^2(K)=0$. Apply the same presentation argument to $K$ to obtain finiteness of $H^1(K)$. Then the segment $H^0(P)\to H^0(E)\to H^1(K)$ proves finiteness of $H^0(E)$. Higher groups vanish by Question 3. Hence **every $H^i(C,\mathcal F)$ is finite-dimensional.**

Next establish a useful degree estimate without using the duality requested later. A [global regular function](../../../../../global-regular-function.md) on $C$ is constant: a nonconstant one would give a [finite morphism](../../../../../finite-morphism.md) $C\to\mathbb P^1$ by Question 1. Such a morphism is surjective, because its closed image contains the [generic point](../../../../../generic-point.md), but a regular function misses $\infty$, a contradiction. Thus $H^0(C,\mathcal O_C)=k$. Write $g=h^1(C,\mathcal O_C)$, the [genus of a smooth projective curve](../../../../../genus-of-a-smooth-projective-curve.md). For any [divisor on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) $A$ and point $P$, the local [discrete valuation ring](../../../../../discrete-valuation-ring.md) gives

$$
0\longrightarrow\mathcal O_C(A-P)\longrightarrow\mathcal O_C(A)
\longrightarrow k_P\longrightarrow0.
$$

The last term is a length-one [skyscraper sheaf](../../../../../skyscraper-sheaf.md). Additivity of the [Euler characteristic of a coherent sheaf](../../../../../euler-characteristic-of-a-coherent-sheaf.md) and repeated addition or subtraction of points give

$$
\chi(\mathcal O_C(A))=\deg A+1-g,\qquad
h^0(\mathcal O_C(A))\ge\deg A+1-g.
$$

The inequality follows because $h^1$ is nonnegative, and is sufficient for the following argument.

Fix $P\in C$. For $n\ge g+1$ this estimate gives at least two independent sections of $\mathcal O_C(nP)$, one of them the constant section. A nonconstant section is a [rational function on an algebraic variety](../../../../../rational-function-on-an-algebraic-variety.md) whose poles are confined to $P$. It must have a pole there, since a globally regular function is constant. Its extension $C\to\mathbb P^1$ is finite, and its inverse image of $\mathbb A^1$ is exactly $C\setminus\{P\}$. Consequently $U=C\setminus\{P\}$ is affine.

Let $T$ be the torsion subsheaf of $\mathcal F$ and let $V=\mathcal F/T$. The support of $T$ is finite; such a [coherent sheaf](../../../../../coherent-sheaf.md) is a finite direct sum of sheaves supported at points and has zero higher [sheaf cohomology](../../../../../sheaf-cohomology.md). The [torsion-free sheaf](../../../../../torsion-free-sheaf.md) $V$ is [locally free](../../../../../locally-free-sheaf.md): a finitely generated [torsion-free module](../../../../../torsion-free-module.md) over a [discrete valuation ring](../../../../../discrete-valuation-ring.md) is free. Tensoring by any [invertible sheaf](../../../../../line-bundle.md) is exact, so

$$
H^1(C,\mathcal F(D))\cong H^1(C,V(D)).
$$

The inclusions $V(nP)\subset V((n+1)P)$ have point-supported quotients. Their [long exact sequences in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md) therefore give surjections on $H^1$. Moreover

$$
\varinjlim_n V(nP)=j_*(V|_U),\qquad j:U\hookrightarrow C:
$$

a section regular away from $P$ has some finite pole order at $P$. Compute this direct limit on a finite affine cover of $C$. All its intersections with $U$ are affine by Question 2, and localization commutes with filtered direct limits. The [Čech cochain complex](../../../../../cech-cochain-complex.md) consequently gives

$$
\varinjlim_n H^1(C,V(nP))=H^1(U,V|_U)=0.
$$

The maps from $H^1(C,V)$ to these groups are surjective. Choose a finite basis of this starting vector space. Each basis vector becomes zero at some stage in the direct limit; one common stage kills the entire basis. Thus there exists $n_0\ge0$ with $H^1(C,V(n_0P))=0$.

Now let $D$ be any [divisor on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) with $\deg D\ge n_0+g$. The estimate above gives $h^0(\mathcal O_C(D-n_0P))\ge1$. A nonzero section identifies $D-n_0P$ with an effective divisor $E$ up to [linear equivalence of divisors](../../../../../linear-equivalence-of-divisors.md). Hence $V(D)\cong V(n_0P+E)$. Adding $E$ gives a point-supported quotient of $V(n_0P+E)/V(n_0P)$, so its first [sheaf cohomology](../../../../../sheaf-cohomology.md) is a quotient of $H^1(C,V(n_0P))=0$. We have proved [uniform high-degree vanishing on a smooth projective curve](../../../../../uniform-high-degree-vanishing-on-a-smooth-projective-curve.md):

$$
\boxed{H^i(C,\mathcal F(D))=0\quad\text{for every }i\ge1\text{ and every }D\text{ with }\deg D\ge n_0+g.}
$$

This bound concerns all high-degree divisors, not only multiples of a previously chosen divisor.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 80](../../paper-80-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
