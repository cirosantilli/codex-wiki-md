<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $V$ have [dimension](../../../../../dimension-vector-space.md) $2m$ over $\mathbb F_q$, with a nondegenerate [alternating bilinear form](../../../../../alternating-bilinear-form.md) $B$. The symplectic [group](../../../../../group-split.md) is

$$
Sp_{2m}(q)=\{g\in GL(V):B(gv,gw)=B(v,w)\}.
$$

It acts freely and transitively on ordered symplectic bases. Choose the first vector $e_1\ne0$ in $q^{2m}-1$ ways, then choose $f_1$ with $B(e_1,f_1)=1$ in $q^{2m-1}$ ways. Their span is nondegenerate, so choose the remaining [symplectic basis](../../../../../symplectic-basis.md) in its [orthogonal complement](../../../../../orthogonal-complement.md). This gives the recurrence

$$
|Sp_{2m}(q)|=(q^{2m}-1)q^{2m-1}|Sp_{2m-2}(q)|,
$$

and therefore

$$
\boxed{|Sp_{2m}(q)|=q^{m^2}\prod_{j=1}^m(q^{2j}-1),\qquad |Sp_4(2)|=2^4(2^2-1)(2^4-1)=720.}
$$

For the [permutation](../../../../../permutation.md) module $\mathbb F_2^r$ with $r$ even, put $\mathbf t=(1,\ldots,1)$ and

$$
W=\left\{x:\sum_i x_i=0\right\}=\mathbf t^\perp.
$$

It is invariant under coordinate [permutations](../../../../../permutation.md) and has codimension one. The [dot product](../../../../../dot-product.md) restricted to $W$ is alternating because $B(x,x)=\sum_i x_i^2=\sum_i x_i=0$. Since the ambient [dot product](../../../../../dot-product.md) is nondegenerate, $W^\perp=\langle\mathbf t\rangle$. Evenness of $r$ ensures $\mathbf t\in W$, so

$$
\boxed{\operatorname{rad}(B|_W)=\langle\mathbf t\rangle.}
$$

Here the word symplectic must be understood as an alternating form before quotienting: a form with a nonzero radical is degenerate. The nondegenerate [symplectic form](../../../../../symplectic-form.md) is induced on $\overline W=W/\langle\mathbf t\rangle$, of [dimension](../../../../../dimension-vector-space.md) $r-2$.

Now put $r=2m+2$. Coordinate [permutations](../../../../../permutation.md) preserve the induced form and give a homomorphism $S_r\to Sp_{r-2}(2)$. To see it is faithful for $r\ge6$, suppose a [permutation](../../../../../permutation.md) $\sigma$ acts trivially on $\overline W$. For every pair of distinct indices,

$$
e_{\sigma(i)}+e_{\sigma(j)}\equiv e_i+e_j\pmod{\langle\mathbf t\rangle}.
$$

The two weight-two vectors could differ by $\mathbf t$ only if the complement of a two-element set also had size two. For $r\ge6$ that is impossible. Thus $\sigma$ preserves every two-element set, and hence fixes every index: intersect two such sets with one common element. Therefore

$$
\boxed{S_{2m+2}\hookrightarrow Sp_{2m}(2)\quad(m\ge2).}
$$

For $m=2$, both [groups](../../../../../group-split.md) have order $720$, and the injection is onto. This proves

$$
\boxed{S_6\cong Sp_4(2).}
$$

The lower bound matters: for $r=4$ the action on the quotient has the [Klein four-group](../../../../../klein-four-group.md) as [group homomorphism kernel](../../../../../kernel-of-a-group-homomorphism.md). The construction is the [deleted permutation module in characteristic two](../../../../../deleted-permutation-module-in-characteristic-two.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
