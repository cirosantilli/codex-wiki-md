<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Work over the [finite field](../../../../../finite-field.md) $\mathbb F_2$. The given factorization shows that $g$ divides $X^{23}-1$, so it generates a length-$23$ [cyclic code](../../../../../cyclic-code.md) $C$. Since $\deg g=11$, the vectors represented by

$$
g,\ Xg,\ \ldots,\ X^{11}g
$$

form a [basis](../../../../../basis.md): their distinct leading degrees prove their [linear independence](../../../../../linear-independence.md), and every multiple of $g$ representing a polynomial of degree below $23$ has a multiplier of degree at most $11$. Hence $C$ is a [binary linear code](../../../../../binary-linear-code.md) of [dimension](../../../../../dimension-vector-space.md) $12$, containing $2^{12}$ codewords. The generator has [Hamming weight](../../../../../hamming-weight.md) seven, so the [minimum Hamming distance of a linear code](../../../../../minimum-hamming-distance-of-a-linear-code.md) satisfies $d(C)\leq7$.

The [BCH bound](../../../../../bch-bound.md) used here is the following consecutive-root theorem. If a length-$n$ [cyclic code](../../../../../cyclic-code.md) over $\mathbb F_q$, with $n$ relatively prime to $q$, has a [generator polynomial of a cyclic code](../../../../../generator-polynomial-of-a-cyclic-code.md) vanishing at $\beta^b,\beta^{b+1},\ldots,\beta^{b+\Delta-2}$ for a primitive $n$th root $\beta$, then its [minimum Hamming distance](../../../../../minimum-distance-of-a-code.md) is at least $\Delta$.

Choose a root $\beta$ of $g$ in an [algebraic closure](../../../../../algebraic-closure.md) of $\mathbb F_2$. The factorization implies $\beta^{23}=1$, while $g(1)=1$ in $\mathbb F_2$, so $\beta\neq1$. As $23$ is prime, $\beta$ has order $23$. The [Frobenius endomorphism](../../../../../frobenius-endomorphism.md) preserves the roots of a polynomial with coefficients in $\mathbb F_2$: $g(z^2)=g(z)^2$. Thus every $\beta^{2^j}$ is a root. In particular, $2^8=256\equiv3\pmod{23}$ shows that

$$
\beta,\ \beta^2,\ \beta^3,\ \beta^4
$$

are roots of $g$. These four consecutive roots give $d(C)\geq5$ by the [BCH bound](../../../../../bch-bound.md). A further argument is needed to exclude weights five and six.

Put $S(X)=1+X+\cdots+X^{22}$. Cancelling $X+1$ in the supplied factorization gives $g(X)g^{\mathrm{rev}}(X)=S(X)$. In the [quotient ring](../../../../../quotient-ring.md) $\mathbb F_2[X]/(X^{23}-1)$, $X$ is invertible and every cyclic shift of $S$ equals $S$. Since $g^{\mathrm{rev}}(X)=X^{11}g(X^{-1})$,

$$
g(X)g(X^{-1})=X^{-11}S(X)\equiv S(X)\pmod{X^{23}-1}.
$$

The coefficient of $X^s$ in this circular product is $\sum_{i-j\equiv s\ (23)}g_i g_j$, the binary [inner product](../../../../../inner-product.md) of the coefficient vector of $g$ with a cyclic shift of itself. Every coefficient of $S$ is one. The [circular autocorrelation of the binary Golay generator](../../../../../circular-autocorrelation-of-the-binary-golay-generator.md) therefore implies that all pairs of [basis](../../../../../basis.md) rows $u_i=X^ig$, including equal rows, satisfy

$$
u_i\cdot u_j=1\quad\text{in }\mathbb F_2.
$$

Each $u_i$ has [Hamming weight](../../../../../hamming-weight.md) seven. Append its parity bit, which is one, and write $\widehat u_i=(u_i,1)$. The extended rows have [Hamming weight](../../../../../hamming-weight.md) eight and satisfy $\widehat u_i\cdot\widehat u_j=1+1=0$. Their [linear span](../../../../../linear-span.md) is precisely the [parity extension](../../../../../parity-extension.md) $\widehat C$ of $C$, because the appended coordinate is the linear functional equal to the sum of all coordinates.

These extended generators produce a [doubly even code](../../../../../doubly-even-code.md). To prove this rather than assume it, use

$$
\operatorname{wt}(v+w)=\operatorname{wt}(v)+\operatorname{wt}(w)
-2|\operatorname{supp}(v)\cap\operatorname{supp}(w)|.
$$

All the extended generators have weights divisible by four. A sum of previous generators is orthogonal to the next generator, so the intersection size in this identity is even. Induction proves that every word in $\widehat C$ has [Hamming weight](../../../../../hamming-weight.md) divisible by four; this is the [orthogonal generators of doubly even codes](../../../../../orthogonal-generators-of-doubly-even-codes.md) argument.

An original word of weight five acquires a parity bit and has extended weight six, while a word of weight six acquires a zero parity bit and still has extended weight six. Both contradict divisibility by four. Together with the [BCH bound](../../../../../bch-bound.md) $d(C)\geq5$ and the weight-seven generator, this completes the [BCH and parity-extension proof of the binary Golay distance](../../../../../bch-and-parity-extension-proof-of-the-binary-golay-distance.md):

$$
\boxed{d(C)=7,\qquad C\text{ has parameters }[23,12,7].}
$$

Its radius-three [Hamming balls](../../../../../hamming-ball.md) are disjoint, and their volume is

$$
v_{23}(3)=1+23+\binom{23}{2}+\binom{23}{3}
=1+23+253+1771=2048=2^{11}.
$$

There are $2^{12}$ such balls, so they contain $2^{12}2^{11}=2^{23}$ words, exactly the size of the ambient binary cube. They therefore cover the cube, with every word in exactly one ball. Hence

$$
\boxed{C\text{ is the perfect binary Golay code, correcting every pattern of at most three errors}.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
