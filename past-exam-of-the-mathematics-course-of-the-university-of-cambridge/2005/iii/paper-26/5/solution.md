<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [filtered category](../../../../../filtered-category.md) is nonempty, any two objects have arrows to a common object, and any parallel pair $u,v:A\rightrightarrows B$ is equalized by some arrow $B\to C$. Equivalently, every finite diagram has a [cocone](../../../../../cocone-under-a-diagram.md): first choose a common target for its finitely many objects, then successively equalize the finitely many discrepancies along its arrows. A [weakly filtered category](../../../../../weakly-filtered-category.md) requires a [cocone](../../../../../cocone-under-a-diagram.md) only for finite nonempty connected diagrams. Equivalently, each [connected component of a category](../../../../../connected-component-of-a-category.md) is filtered. To see this, two objects in one component are joined by a finite zigzag; a [cocone](../../../../../cocone-under-a-diagram.md) on that zigzag gives a common target, and a parallel-pair diagram gives the equalization condition. Conversely a connected diagram lies in one filtered component. An empty category is weakly filtered, since it has no such diagrams.

The unique outgoing-arrow lifting property is precisely that of a [discrete opfibration](../../../../../discrete-opfibration.md). Let $F:\mathcal C\to\mathcal D$ have this property, with $\mathcal D$ weakly filtered. Take a diagram $H:J\to\mathcal C$ with $J$ finite, nonempty and connected, and choose a [cocone](../../../../../cocone-under-a-diagram.md) $\alpha_j:FH(j)\to D$ in $\mathcal D$. Lift each $\alpha_j$ uniquely from $H(j)$, obtaining $\widetilde\alpha_j:H(j)\to C_j$. For an arrow $u:j\to k$, the arrow $\widetilde\alpha_kH(u)$ and the lift $\widetilde\alpha_j$ have the same source and the same image $\alpha_kFH(u)=\alpha_j$. Unique lifting gives equality of the arrows and, importantly, $C_j=C_k$. Connectedness of $J$ makes all targets a single object $C_0$. The lifts are a [cocone](../../../../../cocone-under-a-diagram.md) in $\mathcal C$, so **the domain of a discrete opfibration over a weakly filtered category is weakly filtered**.

Consider [discrete opfibrations](../../../../../discrete-opfibration.md) $F:A\to D$ and $G:B\to D$ and their [pullback in a category](../../../../../pullback-category-theory.md) $E=A\times_D B$. The assumed creation of pullbacks describes its objects as pairs $(a,b)$ with $Fa=Gb$, and its arrows as pairs $(u,v)$ with $Fu=Gv$. There is a canonical map

$$
\Phi:\pi_0(E)\to\pi_0(A)\times_{\pi_0(D)}\pi_0(B),\qquad [(a,b)]\mapsto([a],[b]),
$$

where $\pi_0$ denotes [connected components of a category](../../../../../connected-component-of-a-category.md). Assume the vertices are [weakly filtered categories](../../../../../weakly-filtered-category.md).

For surjectivity, choose components $[a]$ and $[b]$ whose images belong to the same component of $D$. That component is filtered, so there are arrows $Fa\to d$ and $Gb\to d$. Lifting them from $a$ and $b$ gives $a\to a_1$ and $b\to b_1$ with $Fa_1=Gb_1=d$. Thus $(a_1,b_1)\in E$ maps to the chosen component pair.

For injectivity, suppose $(a,b)$ and $(a',b')$ have the same images under $\Phi$. Filteredness of the relevant components upstairs gives arrows

$$
a\xrightarrow{u}a_0\xleftarrow{u'}a',\qquad
b\xrightarrow{v}b_0\xleftarrow{v'}b'.
$$

Write $d=Fa=Gb$ and $d'=Fa'=Gb'$. In $D$ the four arrows $Fu,Gv,Fu',Gv'$ make a finite connected diagram with objects $d,d',Fa_0,Gb_0$. It has a [cocone](../../../../../cocone-under-a-diagram.md), so there are $r:Fa_0\to z$ and $s:Gb_0\to z$ with

$$
rFu=sGv,\qquad rFu'=sGv'.
$$

Lift $r$ from $a_0$ and $s$ from $b_0$, obtaining arrows to $a_1,b_1$ with $Fa_1=Gb_1=z$. Their composites with $(u,v)$ form an arrow $(a,b)\to(a_1,b_1)$ of $E$, and their composites with $(u',v')$ form an arrow $(a',b')\to(a_1,b_1)$. Hence the two representatives lie in the same component. This proves the [connected components of discrete-opfibration pullbacks](../../../../../connected-components-of-discrete-opfibration-pullbacks.md) formula

$$
\boxed{\pi_0(A\times_D B)\cong\pi_0(A)\times_{\pi_0(D)}\pi_0(B)}.
$$

The map is the canonical comparison, so this is preservation of the pullback, not just an accidental bijection of its objects.

Now fix a small [filtered category](../../../../../filtered-category.md) $C$. Every object $D\to C$ of $\mathrm{Disc}/C$ has weakly filtered domain by the lifting argument, and every arrow of this slice is a [discrete opfibration](../../../../../discrete-opfibration.md). Pullbacks in the slice are the created pullbacks above; their resulting domains are weakly filtered as well, since a pullback projection is a [discrete opfibration](../../../../../discrete-opfibration.md) onto a weakly filtered domain. The terminal slice object is $1_C:C\to C$. Because $C$ is nonempty and filtered, it is connected, so $\pi_0(C)$ is a singleton. Thus the component [functor](../../../../../functor.md) preserves the [terminal object](../../../../../terminal-object.md) and pullbacks. These construct every finite [categorical limit](../../../../../categorical-limit.md): binary products are pullbacks over the [terminal object](../../../../../terminal-object.md), and [equalizers](../../../../../equaliser.md) are pullbacks along a diagonal into a binary product. Therefore **the functor from this slice to sets preserves all finite limits**.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
