<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [joint spectrum](../../../../../../joint-spectrum.md) $\operatorname{Spec}(n)$ consists of the tuples of simultaneous [eigenvalues](../../../../../../eigenvalue.md) of $X_1,\ldots,X_n$ occurring in irreducible complex $S_n$-modules. A [Gelfand–Tsetlin basis](../../../../../../gelfand-tsetlin-basis.md) is a [Gelfand–Tsetlin basis](../../../../../../gelfand-tsetlin-basis.md): its vectors lie in the one-dimensional joint eigenspaces selected by successive restrictions. The weight of $v$ is $\alpha=(a_1,\ldots,a_n)$ when $X_jv=a_jv$ for every $j$.

Define $\operatorname{Cont}(n)$ to be the integer tuples satisfying the [content vector of a standard Young tableau](../../../../../../content-vector-of-a-standard-young-tableau.md) conditions: $a_1=0$; for $j>1$, at least one of $a_j-1,a_j+1$ occurs earlier; and between any two occurrences of the same integer $a$, both $a-1$ and $a+1$ occur. We will justify their tableau interpretation in part (iv).

Here is the [local spectral rules for Young–Jucys–Murphy elements](../../../../../../local-spectral-rules-for-young-jucys-murphy-elements.md) calculation used in this question. Average a positive definite [Hermitian inner product](../../../../../../hermitian-form.md) over $S_n$, making the representation unitary. The $X_j$ are commuting self-adjoint operators because [transpositions](../../../../../../transposition-permutation.md) are self-adjoint involutions. Put $s_i=(i\ i+1)$ and $d=a_{i+1}-a_i$. The group-algebra relations are

$$
X_{i+1}s_i-s_iX_i=1,\qquad
X_is_i-s_iX_{i+1}=-1,\qquad
s_iX_j=X_js_i\quad(j\ne i,i+1).
$$

For a unit weight vector $v$, the first relation gives $d\langle v,s_iv\rangle=1$. Thus $d\ne0$, $|d|\geq1$, and

$$
w=s_iv-d^{-1}v
$$

has the weight obtained by swapping $a_i,a_{i+1}$, with $\|w\|^2=1-d^{-2}$. If $d=\pm1$, then $w=0$ and $s_iv=\pm v$. If $|d|>1$, then $w\ne0$, providing an admissible spectral swap in the same [irreducible module](../../../../../../irreducible-module.md).

For the proposed three consecutive weights $(a,a+1,a)$, these rules give $s_iv=v$ and $s_{i+1}v=-v$. But the [braid relation in a Coxeter group](../../../../../../braid-relation-in-a-coxeter-group.md) would imply

$$
s_is_{i+1}s_iv=-v,\qquad
s_{i+1}s_is_{i+1}v=v,
$$

a contradiction. Hence **the proposed tuple is not in $\operatorname{Spec}(n)$**. The same argument, with the signs reversed, excludes $(a,a-1,a)$ as well.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
