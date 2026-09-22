<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose a rational [Borel subgroup](../../../../../../borel-subgroup.md) $B=TU$ with rational [maximal algebraic torus](../../../../../../maximal-algebraic-torus.md) $T$, and use the [Lang map](../../../../../../lang-map.md) $\mathcal L(g)=g^{-1}F(g)$. Conjugating the pair $({}^gB,F({}^gB))$ by $g^{-1}$ gives $(B,{}^{\mathcal L(g)}B)$. Part (a) therefore gives

$$
({}^gB,F({}^gB))\in O(w)\quad\Longleftrightarrow\quad\mathcal L(g)\in B\dot wB.
$$

Moreover $\mathcal L(gb)=b^{-1}\mathcal L(g)F(b)$, and $F(B)=B$, so this inverse image is stable under right multiplication by $B$. The [flag variety](../../../../../../generalized-flag-variety.md) identification consequently restricts to the required isomorphism

$$
\boxed{X(w)\cong\mathcal L^{-1}(B\dot wB)/B.}
$$

**The second printed isomorphism is false as written: it omits a unipotent quotient.** Take $G=\mathrm{SL}_2(\overline{\mathbb F}_q)$ with standard [Frobenius endomorphism of an algebraic group](../../../../../../frobenius-endomorphism-of-an-algebraic-group.md) and $w=1$. Then $X(1)$ consists of the $q+1$ rational lines in $\mathbb F_q^2$, so has dimension zero. Every [Borel subgroup](../../../../../../borel-subgroup.md) $B'$ has one-dimensional [unipotent radical](../../../../../../unipotent-radical.md) $U'$. The [Lang map](../../../../../../lang-map.md) is a finite surjective [étale morphism](../../../../../../etale-morphism.md), so $\mathcal L^{-1}(U')$ has dimension one. Quotienting by the finite group $T'^F$ preserves that dimension. Thus no choices of $T'$ and $B'$ can make the asserted two varieties isomorphic in this example.

Here is the corrected construction, including the missing quotient. Choose $x$ by the [Lang theorem for algebraic groups](../../../../../../lang-theorem-for-algebraic-groups.md) so that $x^{-1}F(x)=\dot w$. Define

$$
T'=xTx^{-1},\qquad U_x=xUx^{-1},\qquad B'=F(xBx^{-1}),\qquad U'=R_u(B')=F(U_x).
$$

Then $F(T')=x\dot wT\dot w^{-1}x^{-1}=T'$, so $T'$ is a [rational maximal torus](../../../../../../rational-maximal-torus.md) contained in $B'$. Put $J=U_x\cap U'=F^{-1}(U')\cap U'$. The correct [unipotent quotient in a Deligne-Lusztig variety](../../../../../../unipotent-quotient-in-a-deligne-lusztig-variety.md) is

$$
\boxed{\mathcal L^{-1}(U')/(J\rtimes T'^F)\cong X(w),\qquad h\longmapsto hxB.}
$$

The semidirect product denotes the subgroup $JT'^F$ acting on the right. Both $U_x$ and $U'$ are normalized by $T'$, so the action is well defined. Also

$$
\mathcal L(hx)=x^{-1}\mathcal L(h)F(x)\in\dot wU\subset B\dot wB
$$

for $h\in\mathcal L^{-1}(U')$, showing directly that the map lands in the [Deligne-Lusztig variety](../../../../../../deligne-lusztig-variety.md).

To prove surjectivity and identify its fibres, use the intermediate variety

$$
Y(\dot w)=\{g:\mathcal L(g)\in U\dot wU\}/U,\qquad F_w(t)=\dot wF(t)\dot w^{-1}\quad(t\in T).
$$

The right $U$-action follows from the twisted-translation identity for the [Lang map](../../../../../../lang-map.md). Right multiplication by $T^{F_w}$ also acts, and $Y(\dot w)/T^{F_w}\cong X(w)$. Indeed if $\mathcal L(g)\in B\dot wB$, write it as $u_1t\dot wu_2$. Replacing $g$ by $ga$, with $a\in T$, changes its torus factor to $a^{-1}tF_w(a)$. Surjectivity of the twisted [Lang map](../../../../../../lang-map.md) on the connected [algebraic torus](../../../../../../algebraic-torus.md) makes this factor one. Once the factor is one, two representatives of the same flag differ by $ua$ with $u\in U$ and $a\in T^{F_w}$. This proves both surjectivity and the asserted finite covering, including its group of fibres.

Now map $Z=\mathcal L^{-1}(U')$ to $Y(\dot w)$ by $h\mapsto hxU$. Given $\mathcal L(g)=u_1\dot wu_2$, replace $g$ by $gu_1$. Then

$$
\mathcal L(gu_1)=\dot wu_2F(u_1)\in\dot wU.
$$

Thus $h=gu_1x^{-1}$ belongs to $Z$ and maps to the original point $gU$. This proves surjectivity. Two preimages have the form $h$ and $hk$, where $k\in U_x$. Since $F(k)\in U'$ and $\mathcal L(h)\in U'$, the identity

$$
\mathcal L(hk)=k^{-1}\mathcal L(h)F(k)
$$

shows that $hk\in Z$ precisely when $k\in U'$, hence precisely when $k\in J$. Therefore the fibres are exactly the right $J$-orbits.

These are isomorphisms of [geometric quotients](../../../../../../geometric-quotient.md), not just bijections on points. The groups $U_x,U'$ contain root subgroups for the same [maximal algebraic torus](../../../../../../maximal-algebraic-torus.md), so their intersection $J$ is smooth. The map $Z\to Y(\dot w)$ is a smooth surjection with fibre $J$: the differential of the [Lang map](../../../../../../lang-map.md) is invertible, and the kernel of the differential of $h\mapsto hxU$ on $Z$ is the translate of $\operatorname{Lie}(U_x)\cap\operatorname{Lie}(U')=\operatorname{Lie}(J)$. This gives $Z/J\cong Y(\dot w)$. Finally $xT^{F_w}x^{-1}=T'^F$, so quotienting the remaining finite torus action gives the displayed corrected formula.

For $w=1$, $J=U_x$ is exactly the affine-line factor in the counterexample. More generally $Z/T'^F\to X(w)$ retains unipotent fibres of dimension $\dim J$; it becomes the printed isomorphism only when this intersection is trivial. The missing factor is also recorded in the quotient construction in [Tiep's lectures, proof of Theorem 5.22](https://viasm.edu.vn/Cms_Data/Contents/viasm/Media/file/viasm_2016.pdf).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
