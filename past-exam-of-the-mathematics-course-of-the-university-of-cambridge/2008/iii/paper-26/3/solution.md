<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [comma category](../../../../../comma-category.md) $(A\downarrow F)$ has objects $(C,u)$ with $C\in\mathcal C$ and $u:A\to FC$ a set map. A morphism $(C,u)\to(D,v)$ is an arrow $h:C\to D$ such that $Fh\circ u=v$. Composition and identities are those of $\mathcal C$. For $A=1$, this is the [category of elements](../../../../../category-of-elements.md) $E$ of $F$: objects are $(C,x)$ with $x\in FC$ and arrows satisfy $Fh(x)=y$.

Associate to $(C,x)$ the covariant [representable functor](../../../../../representable-functor.md) $H_C=\mathcal C(C,-)$. An arrow $h:(C,x)\to(D,y)$ of $E$ gives, by precomposition, $H_D\to H_C$. Thus this is a diagram $H:E^{\mathrm{op}}\to[\mathcal C,\mathbf{Set}]$. There is a compatible natural map $H_C\to F$ sending $f:C\to B$ to $Ff(x)$.

[Colimits](../../../../../colimit.md) in this [functor category](../../../../../functor-category.md) are pointwise. At an object $B$, the induced map from the [colimit](../../../../../colimit.md) sends a class represented by $(C,x,f:C\to B)$ to $Ff(x)$. It is surjective because $z\in FB$ is represented by $(B,z,1_B)$. It is injective because every representative with value $z$ is identified with that same canonical representative: the arrow $f:(C,x)\to(B,z)$ in $E$ becomes an arrow of the indexing diagram sending $1_B$ to $f$. These bijections are natural in $B$, proving

$$
\boxed{F\cong\operatorname*{colim}_{(C,x)\in E^{\mathrm{op}}}\mathcal C(C,-).}
$$

Smallness of $\mathcal C$ and set-valuedness of $F$ ensure that $E$ is small, so the displayed [colimit](../../../../../colimit.md) is defined. This proves the introductory density request before the three equivalent conditions.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
