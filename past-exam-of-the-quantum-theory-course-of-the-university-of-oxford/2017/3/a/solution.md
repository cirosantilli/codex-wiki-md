<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The given [angular momentum commutation relations](../../../../angular-momentum-commutation-relations.md) imply $[L_3,L_1]=i\hbar L_2$ and $[L_3,L_2]=-i\hbar L_1$. By [linearity](../../../../linearity.md),

$$
[L_3,L_\pm]=i\hbar L_2\pm i(-i\hbar L_1)=\boxed{\pm\hbar L_\pm}.
$$

Similarly,

$$
[L_+,L_-]=-2i[L_1,L_2]=\boxed{2\hbar L_3}.
$$

For the remaining [commutators](../../../../commutator.md), the [commutator product rule](../../../../commutator-product-rule.md) gives, for each $j$,

$$
[L^2,L_j]=\sum_i\left(L_i[L_i,L_j]+[L_i,L_j]L_i\right)=i\hbar\sum_{i,k}\epsilon_{ijk}(L_iL_k+L_kL_i)=0.
$$

The last sum vanishes because the [Levi-Civita symbol](../../../../levi-civita-symbol.md) is antisymmetric under $i\leftrightarrow k$, while $L_iL_k+L_kL_i$ is symmetric. Taking $j=3$ and then linear combinations with $j=1,2$ proves

$$
\boxed{[L^2,L_3]=0=[L^2,L_\pm].}
$$

If $L^2\psi=\lambda\hbar^2\psi$ and $L_3\psi=m\hbar\psi$, these identities yield

$$
L^2L_+\psi=L_+L^2\psi=\lambda\hbar^2L_+\psi,\qquad L_3L_+\psi=(L_+L_3+\hbar L_+)\psi=(m+1)\hbar L_+\psi.
$$

One must also prove that this candidate [eigenstate](../../../../eigenstate.md) is nonzero. Since the [angular momentum operators](../../../../angular-momentum-operator-split.md) are [self-adjoint operators](../../../../self-adjoint-operator.md), $L_+^*=L_-$, and expanding the product gives

$$
L_-L_+=L_1^2+L_2^2+i[L_1,L_2]=L^2-L_3^2-\hbar L_3.
$$

Therefore

$$
\|L_+\psi\|^2=\hbar^2\bigl[\lambda-m(m+1)\bigr]\|\psi\|^2.
$$

This is nonnegative and, by the assumed inequality, nonzero. Hence it is positive. The [angular momentum raising operator](../../../../angular-momentum-raising-operator.md) really does produce a nonzero simultaneous [eigenstate](../../../../eigenstate.md) with the claimed [eigenvalues](../../../../eigenvalue.md).

To prove that raising terminates, let $v$ be any nonzero state reached after $r$ steps, with projection $q=m+r$. Positivity gives

$$
\lambda\hbar^2\|v\|^2=\sum_{i=1}^3\|L_iv\|^2\geq\|L_3v\|^2=q^2\hbar^2\|v\|^2,
$$

so $q^2\leq\lambda$. Thus the sequence cannot remain nonzero for every integer $r\geq0$. At its last nonzero state $v=(L_+)^k\psi$, one has $L_+v=0$, and the squared [norm](../../../../norm.md) identity gives

$$
\boxed{\lambda=(m+k)(m+k+1)\quad\text{for some integer }k\geq0.}
$$

Under the paper's initial inequality the first step is nonzero, so in fact $k\geq1$. An [angular momentum ladder endpoint](../../../../angular-momentum-ladder-endpoint.md) must therefore be reached: bounded projection follows from positivity, and the final raising [norm](../../../../norm.md) fixes the total [angular momentum](../../../../angular-momentum.md) [eigenvalue](../../../../eigenvalue.md). Writing $j=m+k$, the complementary product $L_+L_-=L^2-L_3^2+\hbar L_3$ gives $\|L_-v\|^2=2j\hbar^2\|v\|^2$, also showing $j\geq0$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the quantum theory course of the University of Oxford](../../../split.md)
5. [Quantum theory course of the University of Oxford](../../../../quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
