<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $q$ be a prime power and let $V=\mathbb F_q^{2m}$ carry a [nondegenerate](../../../../../../nondegenerate-bilinear-form.md) [alternating bilinear form](../../../../../../alternating-bilinear-form.md) $B$. The [symplectic group over a finite field](../../../../../../symplectic-group-over-a-finite-field.md) is

$$
Sp(V,B)=\{g\in GL(V):B(gv,gw)=B(v,w)\text{ for all }v,w\}.
$$

In a [symplectic basis](../../../../../../symplectic-basis.md) its [matrix](../../../../../../matrix.md) description is $g^{\mathsf T}Jg=J$, where $J=\left(\begin{smallmatrix}0&I_m\\-I_m&0\end{smallmatrix}\right)$. The definition is valid in characteristic two: alternating means $B(v,v)=0$, and then the form is also symmetric.

Count ordered [symplectic bases](../../../../../../symplectic-basis.md) $(e_1,f_1,\ldots,e_m,f_m)$ with $B(e_i,f_j)=\delta_{ij}$ and all $e$-$e$ and $f$-$f$ pairings zero. There are $q^{2m}-1$ choices for $e_1\ne0$. Nondegeneracy makes $v\mapsto B(e_1,v)$ a nonzero [linear functional](../../../../../../linear-functional.md), so there are $q^{2m-1}$ choices for $f_1$ satisfying $B(e_1,f_1)=1$.

The span $P=\langle e_1,f_1\rangle$ is [nondegenerate](../../../../../../nondegenerate-bilinear-form.md). Thus $V=P\oplus P^\perp$, and its [bilinear orthogonal complement](../../../../../../orthogonal-complement-for-a-bilinear-form.md) is [nondegenerate](../../../../../../nondegenerate-bilinear-form.md) of dimension $2m-2$. For completeness, a [vector](../../../../../../vector.md) in the [radical of a bilinear form](../../../../../../radical-of-a-bilinear-form.md) of $P^\perp$ is orthogonal both to $P$ and to $P^\perp$, hence to all $V$ and therefore zero. Recursing constructs and counts every [symplectic basis](../../../../../../symplectic-basis.md). If $b_m$ is their number, $b_m=(q^{2m}-1)q^{2m-1}b_{m-1}$ with $b_0=1$.

The [symplectic group over a finite field](../../../../../../symplectic-group-over-a-finite-field.md) acts freely and transitively on [symplectic bases](../../../../../../symplectic-basis.md): there is a unique [linear map](../../../../../../linear-map.md) sending one ordered [basis](../../../../../../basis.md) to another, and its equality of [basis](../../../../../../basis.md) pairings ensures it preserves $B$. Its order is consequently $b_m$, giving

$$
\boxed{|Sp(2m,q)|=\prod_{i=1}^mq^{2i-1}(q^{2i}-1)=q^{m^2}\prod_{i=1}^m(q^{2i}-1).}
$$

The exponent is $1+3+\cdots+(2m-1)=m^2$. The counting is valid for every prime power $q$, including $q=2$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
