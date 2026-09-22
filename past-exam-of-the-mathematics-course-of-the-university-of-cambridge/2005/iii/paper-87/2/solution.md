<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Represent a word $(c_0,\ldots,c_{n-1})$ in the [Hamming space](../../../../../hamming-space.md) $H_{n,q}$ by the [polynomial](../../../../../polynomial-split.md) $c(x)=\sum_{j=0}^{n-1}c_jx^j$. A [cyclic code](../../../../../cyclic-code.md) is a [linear code](../../../../../linear-code.md) invariant under the cyclic coordinate shift $(c_0,\ldots,c_{n-1})\mapsto(c_{n-1},c_0,\ldots,c_{n-2})$. Under this identification the shift is multiplication by $x$ modulo $x^n-1$. A shift-invariant [vector subspace](../../../../../vector-subspace.md) is closed under multiplication by every [polynomial](../../../../../polynomial-split.md), since such multiplication is a [linear combination](../../../../../linear-combination.md) of shifts. It is therefore an [ideal](../../../../../ideal.md) of

$$
R=\mathbb F_q[x]/(x^n-1).
$$

Conversely every [ideal](../../../../../ideal.md) of $R$ is a [vector subspace](../../../../../vector-subspace.md) closed under multiplication by $x$, hence a [cyclic code](../../../../../cyclic-code.md). Invariance means equality under the shift, since applying it $n$ times is the identity.

Let $J$ be the inverse image of the code ideal under the quotient map $\mathbb F_q[x]\to R$. It contains $(x^n-1)$ and is nonzero. Choose a nonzero element of $J$ of smallest degree and scale it to a [monic polynomial](../../../../../monic-polynomial.md) $g$. For any $f\in J$, [polynomial division](../../../../../polynomial-division.md) gives $f=ag+r$ with $\deg r<\deg g$. Since $r=f-ag\in J$, minimality forces $r=0$. Thus $J=(g)$ and in particular

$$
\boxed{g\mid x^n-1,\qquad C=(\overline g)\subseteq R.}
$$

This is the required [generator polynomial of a cyclic code](../../../../../generator-polynomial-of-a-cyclic-code.md); the divisibility direction in the printed formula is reversed. The quotient-ring modulus is $x^n-1$, with $1$ denoting the multiplicative identity of the [finite field](../../../../../finite-field.md). If $r=\deg g$, every codeword has a unique representative $ag$ with $\deg a<n-r$. Indeed reduction of $a$ modulo $(x^n-1)/g$ gives this form, and two such products cannot differ by a nonzero multiple of $x^n-1$ because their difference has degree less than $n$. Therefore

$$
\boxed{\dim C=n-r,\qquad g,xg,\ldots,x^{n-r-1}g\text{ form a basis}.}
$$

For the zero code the convention is $g=x^n-1$ and this [basis](../../../../../basis.md) is empty; for the full word space $g=1$.

The [zeros of a cyclic code](../../../../../zero-of-a-cyclic-code.md) are the [polynomial roots](../../../../../root-of-a-polynomial.md) of $g$ in a [splitting field](../../../../../splitting-field.md) $E$ of $x^n-1$. Suppose first that the [characteristic](../../../../../characteristic-of-a-field.md) $p$ of $\mathbb F_q$ does not divide $n$. The [formal derivative](../../../../../formal-derivative.md) of $x^n-1$ is $nx^{n-1}$, which has no common root with $x^n-1$; all roots of $g$ are therefore simple. If they are $\alpha_1,\ldots,\alpha_r$, then $g\mid c$ is equivalent to $c(\alpha_i)=0$ for all $i$. A [root-evaluation parity-check matrix of a cyclic code](../../../../../root-evaluation-parity-check-matrix-of-a-cyclic-code.md), written with checks as rows, is consequently

$$
H_E=\begin{pmatrix}1&\alpha_1&\cdots&\alpha_1^{n-1}\\\vdots&\vdots&&\vdots\\1&\alpha_r&\cdots&\alpha_r^{n-1}\end{pmatrix},\qquad H_Ec^T=0.
$$

Its entries may lie in $E$, rather than in the original [finite field](../../../../../finite-field.md). To obtain a [parity-check matrix](../../../../../parity-check-matrix.md) over $\mathbb F_q$, choose a [basis](../../../../../basis.md) of $E$ over $\mathbb F_q$ and replace each equation by the equations for all of its field coordinates. The resulting matrix has the same kernel $C$, hence [rank](../../../../../rank-one-quadratic-form.md) $r=n-\dim C$; retain any $r$ independent rows. More economically, choose one root from each [Frobenius conjugate](../../../../../frobenius-conjugate.md) orbit. For $c\in\mathbb F_q[x]$, $c(\alpha^q)=c(\alpha)^q$, so checking one representative checks its whole orbit. Expanding that representative's equation in a [basis](../../../../../basis.md) of $\mathbb F_q(\alpha)$ gives precisely the number of checks equal to its orbit length.

No coprimality hypothesis is stated in the question, so the [repeated-root cyclic code](../../../../../repeated-root-cyclic-code.md) case must also be distinguished. Distinct roots alone cannot determine these codes: in $\mathbb F_2[x]/(x^2-1)$, the generators $x+1$ and $(x+1)^2$ have the same zero, but generate codes of [dimensions](../../../../../dimension-vector-space.md) one and zero. In general write $g=\prod_i(x-\alpha_i)^{m_i}$ in $E[x]$. The correct checks are

$$
c^{[\ell]}(\alpha_i)=0\quad(0\leq\ell<m_i),\qquad c^{[\ell]}(x)=\sum_{j\geq\ell}\binom j\ell c_jx^{j-\ell},
$$

using [Hasse derivatives](../../../../../hasse-derivative.md). Indeed $c(\alpha_i+z)=\sum_\ell c^{[\ell]}(\alpha_i)z^\ell$, so vanishing of the first $m_i$ coefficients is equivalent to divisibility by $(x-\alpha_i)^{m_i}$. A [repeated-root parity-check matrix](../../../../../repeated-root-parity-check-matrix.md) over $E$ thus has rows indexed by $(i,\ell)$ and entries

$$
\boxed{(H_E)_{(i,\ell),j}=\begin{cases}\binom j\ell\alpha_i^{j-\ell},&j\geq\ell,\\0,&j<\ell.\end{cases}}
$$

As before, expand to equations over $\mathbb F_q$ and retain $\deg g=\sum_i m_i$ independent rows. The ordinary root-evaluation matrix is exactly the special case $m_i=1$.

For the binary [Hamming code](../../../../../hamming-code.md), let $s\geq2$, $n=2^s-1$, and let $\omega$ generate the [multiplicative group of a finite field](../../../../../multiplicative-group-of-a-finite-field.md) $\mathbb F_{2^s}^{\times}$. This is possible because that group is a [cyclic group](../../../../../cyclic-group.md). Choose a [basis](../../../../../basis.md) of $\mathbb F_{2^s}$ over $\mathbb F_2$. The coordinate columns of $1,\omega,\ldots,\omega^{n-1}$ then run through every nonzero vector of $\mathbb F_2^s$ exactly once. They are a [parity-check matrix](../../../../../parity-check-matrix.md) $H$ for a [Hamming code](../../../../../hamming-code.md), possibly after permuting the columns of a given Hamming matrix. Thus

$$
C=\left\{c\in\mathbb F_2^n:\sum_{j=0}^{n-1}c_j\omega^j=0\right\}=\{c:c(\omega)=0\}
$$

is equivalent to the [Hamming code](../../../../../hamming-code.md). Multiplication by $x$ modulo $x^n-1$ multiplies its evaluation at $\omega$ by $\omega$, so $C$ is a [cyclic code](../../../../../cyclic-code.md).

The [parity-check matrix](../../../../../parity-check-matrix.md) has [rank](../../../../../rank-one-quadratic-form.md) $s$ because its columns contain a [basis](../../../../../basis.md). It has no zero column or repeated column, so no nonzero word of weight one or two is in its kernel. Two distinct nonzero columns have a nonzero sum, which is a third distinct column; these three columns give a word of weight three. Hence $C$ has parameters $[2^s-1,2^s-s-1,3]$.

A [polynomial](../../../../../polynomial-split.md) over $\mathbb F_2$ vanishes at $\omega$ exactly when it is divisible by its [minimal polynomial of an algebraic element](../../../../../minimal-polynomial-of-an-algebraic-element.md) $m_\omega$. The [finite-field Frobenius automorphism](../../../../../finite-field-frobenius-automorphism.md) gives all conjugates of $\omega$ as $\omega^{2^j}$. Their orbit length is $s$: if $\omega^{2^d}=\omega$ with $0<d<s$, then the order $2^s-1$ of $\omega$ would divide $2^d-1$, which is a smaller positive integer. Therefore the [Hamming code as a cyclic code](../../../../../hamming-code-as-a-cyclic-code.md) has

$$
\boxed{g(x)=m_\omega(x)=\prod_{j=0}^{s-1}(x-\omega^{2^j}),\qquad\text{zeros }\omega,\omega^2,\omega^{2^2},\ldots,\omega^{2^{s-1}}.}
$$

The last exponent here is $2^{s-1}$. The printed exponent $2^s-1$ would give $\omega^{2^s-1}=1$, which is not a root of the degree-$s$ irreducible [minimal polynomial of an algebraic element](../../../../../minimal-polynomial-of-an-algebraic-element.md) for $s\geq2$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 87](../../paper-87-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
