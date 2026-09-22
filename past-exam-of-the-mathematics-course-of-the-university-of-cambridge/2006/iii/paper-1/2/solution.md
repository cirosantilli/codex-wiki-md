<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Work in finite dimension over $\mathbb C$; the characteristic-zero real version follows by complexification. The [Cartan solvability criterion](../../../../../cartan-solvability-criterion.md) is

$$
\boxed{\mathfrak g\text{ is solvable}\quad\Longleftrightarrow\quad B(\mathfrak g,[\mathfrak g,\mathfrak g])=0.}
$$

Its semisimplicity consequence, also often called Cartan's criterion, is **$\mathfrak g$ is semisimple if and only if its [Killing form](../../../../../killing-form.md) is nondegenerate**. We prove both forms.

The auxiliary results used are as follows. The [Lie theorem](../../../../../lie-s-theorem.md) simultaneously triangularizes every finite-dimensional representation of a complex [solvable Lie algebra](../../../../../solvable-lie-algebra.md). The [Engel theorem](../../../../../engel-s-theorem.md) says that a matrix [Lie algebra](../../../../../lie-algebra-split.md) consisting entirely of [nilpotent endomorphisms](../../../../../nilpotent-linear-map.md) has a common annihilated nonzero vector and a [basis](../../../../../basis.md) making all its matrices strictly upper triangular; in particular it is a [nilpotent Lie algebra](../../../../../nilpotent-lie-algebra.md). Nilpotent means that the lower central series terminates, which implies that the derived series terminates as well. Finally, the [Additive Jordan decomposition](../../../../../jordan-chevalley-decomposition.md) writes any complex endomorphism uniquely as $x=x_s+x_n$, where $x_s$ is diagonalizable, $x_n$ is nilpotent and they commute. On a [generalized eigenspace](../../../../../generalized-eigenspace.md) $V_\lambda$, the two parts are $\lambda I$ and $x-\lambda I$, and both are polynomials in $x$. On endomorphisms, $\operatorname{ad}x_s$ is diagonalizable, $\operatorname{ad}x_n$ is nilpotent, and these are the Jordan parts of $\operatorname{ad}x$: the first assertion follows by splitting into maps between eigenspaces, and the second by expanding repeated [commutators](../../../../../commutator.md) with the nilpotent $x_n$.

First prove the linear trace version: if $L\subseteq\mathfrak{gl}(V)$ and

$$
\operatorname{tr}(ab)=0\quad(a\in L,\ b\in[L,L]),
$$

then $L$ is solvable. Fix $x\in[L,L]$ and let $V=\bigoplus V_\lambda$ be its [generalized eigenspace](../../../../../generalized-eigenspace.md) decomposition. Define $y$ to act on $V_\lambda$ by the scalar $\overline\lambda$. We do not assume that $y$, $x_s$ or $x_n$ belongs to $L$.

On $\operatorname{Hom}(V_\mu,V_\lambda)$, $\operatorname{ad}x$ has the form $(\lambda-\mu)I+N$ with $N$ nilpotent, whereas $\operatorname{ad}y$ is multiplication by $\overline{\lambda-\mu}$. Choose a polynomial $q$ with $q(d)=\bar d$ for every occurring [eigenvalue](../../../../../eigenvalue.md) difference $d$, and with all its derivatives of positive order up to the relevant nilpotency index zero at $d$. Such a polynomial exists by Hermite interpolation, or the Chinese remainder theorem for the pairwise coprime powers of $(t-d)$. At $d=0$ its value is zero, so $q(0)=0$. Expanding $q(dI+N)$ now gives

$$
\operatorname{ad}y=q(\operatorname{ad}x).
$$

Because $x\in L$ and $[L,L]$ is an ideal, every positive power of $\operatorname{ad}x$ sends $L$ into $[L,L]$. The zero constant term therefore gives $[y,L]\subseteq[L,L]$.

Express $x$ as a sum of [commutators](../../../../../commutator.md) $\sum_j[a_j,b_j]$ with $a_j,b_j\in L$. Cyclicity of trace and the hypothesis imply

$$
\operatorname{tr}(xy)=\sum_j\operatorname{tr}([a_j,b_j]y)
=\sum_j\operatorname{tr}(a_j[b_j,y])=0.
$$

But on $V_\lambda$, $xy$ has trace $\dim(V_\lambda)|\lambda|^2$, since the nilpotent part has trace zero. Hence

$$
0=\operatorname{tr}(xy)=\sum_\lambda\dim(V_\lambda)|\lambda|^2,
$$

forcing every [eigenvalue](../../../../../eigenvalue.md) of $x$ to vanish. Thus every member of the [derived algebra](../../../../../derived-algebra.md) $[L,L]$ is a [nilpotent endomorphism](../../../../../nilpotent-linear-map.md). By the [Engel theorem](../../../../../engel-s-theorem.md), $[L,L]$ is nilpotent and therefore solvable; its derived series terminates, and adjoining the initial term $L$ shows that $L$ is solvable.

Conversely, if $L$ is solvable, the [Lie theorem](../../../../../lie-s-theorem.md) makes it upper triangular. [Commutators](../../../../../commutator.md) of upper-triangular matrices have zero diagonal, and multiplying such a [commutator](../../../../../commutator.md) by an upper-triangular matrix still has zero diagonal. Therefore the trace condition holds. Apply this equivalence to $L=\operatorname{ad}\mathfrak g$. Its trace pairing is the [Killing form](../../../../../killing-form.md), and solvability of its image is equivalent to solvability of $\mathfrak g$: the kernel is its abelian centre, so a terminating derived series in the quotient terminates after at most one more step in $\mathfrak g$. This proves the solvability criterion.

For the semisimplicity criterion, let $R$ be the radical of the [Killing form](../../../../../killing-form.md). Invariance makes $R$ a [Lie algebra ideal](../../../../../ideal-of-a-lie-algebra.md). For $x,y\in R$, their adjoint actions on $\mathfrak g/R$ vanish, so computing trace in a [basis](../../../../../basis.md) adapted to $R$ gives $B_R(x,y)=B_{\mathfrak g}(x,y)=0$. The solvability criterion applied to $R$ shows it is a solvable ideal. Thus a [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) has $R=0$ and a nondegenerate [Killing form](../../../../../killing-form.md).

Conversely, any nonzero solvable ideal has a last nonzero term $A$ in its derived series; this is an abelian ideal of $\mathfrak g$. For $x\in A$, $y\in\mathfrak g$, the map $\operatorname{ad}x\operatorname{ad}y$ sends $\mathfrak g$ into $A$ and vanishes on $A$, so has trace zero. Hence $A\subseteq R$. A nondegenerate [Killing form](../../../../../killing-form.md) therefore rules out nonzero solvable ideals, exactly the definition of semisimplicity.

For classification, nondegeneracy of the [Killing form](../../../../../killing-form.md) provides the duality and root-space pairings used to extract a reduced crystallographic [root system](../../../../../root-system.md) from a [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md). Classification then reduces to the finite [Dynkin diagrams](../../../../../dynkin-diagram.md) and reconstruction of the [Lie algebra](../../../../../lie-algebra-split.md) from its [root](../../../../../root-of-a-root-system.md) data.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
