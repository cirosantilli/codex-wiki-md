<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $a_1,\ldots,a_n$ be distinct elements of a [finite field](../../../../../finite-field.md) $\mathbb F_q$, with $1\leq k\leq n$. The [Reed-Solomon code](../../../../../reed-solomon-error-correction.md) consists of the evaluation [vectors](../../../../../vector.md)

$$
\operatorname{RS}_k(a)=\{(f(a_1),\ldots,f(a_n)):f\in\mathbb F_q[X],\ \deg f<k\}.
$$

Evaluation is an [injective](../../../../../injective-function.md) [linear map](../../../../../linear-map.md): a nonzero [polynomial](../../../../../polynomial-split.md) of degree at most $k-1$ cannot vanish at all $n$ distinct points. Thus the [dimension](../../../../../dimension-vector-space.md) is $k$. The same bound on [polynomial roots](../../../../../root-of-a-polynomial.md) shows that every nonzero [codeword](../../../../../codeword.md) has [Hamming weight](../../../../../hamming-weight.md) at least $n-k+1$. Conversely, choosing any $k-1$ evaluation points and taking their product of linear factors gives a [polynomial](../../../../../polynomial-split.md) whose evaluation vanishes at exactly those points. Its [Hamming weight](../../../../../hamming-weight.md) is $n-k+1$. Hence

$$
\boxed{d=n-k+1.}
$$

For completeness, deleting $d-1$ coordinates from a [linear code](../../../../../linear-code.md) of [minimum Hamming distance](../../../../../minimum-distance-of-a-code.md) $d$ is injective on [codewords](../../../../../codeword.md), since two words with the same retained coordinates would differ in fewer than $d$ positions. Therefore $q^k\leq q^{n-d+1}$, giving the [Singleton bound](../../../../../singleton-bound.md) $d\leq n-k+1$. The [Reed-Solomon code](../../../../../reed-solomon-error-correction.md) attains this bound and is a [maximum distance separable code](../../../../../maximum-distance-separable-code.md). Multiplying individual coordinates by nonzero [field](../../../../../field.md) elements changes neither the [dimension](../../../../../dimension-vector-space.md) nor the [Hamming weight](../../../../../hamming-weight.md), so the same proof applies to a [generalized Reed-Solomon code](../../../../../generalized-reed-solomon-code.md).

To specify the [generator polynomials of a cyclic code](../../../../../generator-polynomial-of-a-cyclic-code.md) unambiguously, use the [primitive cyclic Reed-Solomon code](../../../../../primitive-cyclic-reed-solomon-code.md) convention. Put $n=q-1$, choose a [primitive element of a finite field](../../../../../primitive-element-of-a-finite-field.md) $\omega$, and set

$$
C_{k,b}=\langle g_b(X)\rangle\subseteq\mathbb F_q[X]/(X^n-1),\qquad
 g_b(X)=\prod_{t=b}^{b+n-k-1}(X-\omega^t).
$$

Exponents are taken modulo $n$. This [generator polynomial](../../../../../generator-polynomial-of-a-cyclic-code.md) is a [monic polynomial](../../../../../monic-polynomial.md) of degree $n-k$ dividing $X^n-1$, so the [dimension](../../../../../dimension-vector-space.md) is $k$. It agrees with the evaluation form

$$
C_{k,b}=\{(a_j^{1-b}f(a_j))_{j=0}^{n-1}:\deg f<k\},\qquad a_j=\omega^j.
$$

Indeed, at a defining exponent $t=b,\ldots,b+n-k-1$, a monomial $f(X)=X^s$ contributes the [finite geometric series](../../../../../finite-geometric-series.md) $\sum_j a_j^{t+1-b+s}$. Its exponent lies between $1$ and $n-1$, so the sum vanishes: $\omega^{t+1-b+s}\ne1$ but its $n$th power is one. Every displayed evaluation [vector](../../../../../vector.md) therefore lies in the [cyclic code](../../../../../cyclic-code.md), and both spaces have [dimension](../../../../../dimension-vector-space.md) $k$, proving equality. The narrow-sense choice $b=1$ is the ordinary unweighted evaluation [linear code](../../../../../linear-code.md) on all nonzero [field](../../../../../field.md) elements.

The [duality of primitive cyclic Reed-Solomon codes](../../../../../duality-of-primitive-cyclic-reed-solomon-codes.md) now follows directly. A [vector](../../../../../vector.md) in $C_{k,b}$ has coordinates $a_j^{1-b}f(a_j)$, while a [vector](../../../../../vector.md) in $C_{n-k,1-b}$ has coordinates $a_j^b h(a_j)$, with $\deg h<n-k$. Their [dot product](../../../../../dot-product.md) is $\sum_j a_j f(a_j)h(a_j)$. Every appearing exponent is between $1$ and $n-1$, so every such [finite geometric series](../../../../../finite-geometric-series.md) is zero. The two spaces are orthogonal and their [dimensions](../../../../../dimension-vector-space.md) sum to $n$, giving

$$
\boxed{C_{k,b}^{\perp}=C_{n-k,1-b}.}
$$

Thus the full cyclic family is closed under [dual codes](../../../../../dual-code.md). The offset matters: the [dual code](../../../../../dual-code.md) of the narrow-sense [linear code](../../../../../linear-code.md) generally has offset zero, rather than one.

For arbitrary evaluation points, the precise statement is closure of [generalized Reed-Solomon codes](../../../../../generalized-reed-solomon-code.md) under duality. If $C=\operatorname{GRS}_k(a,v)$, put $P(X)=\prod_i(X-a_i)$ and $u_i=(v_iP'(a_i))^{-1}$. [Lagrange interpolation](../../../../../lagrange-polynomial.md) shows $\sum_i p(a_i)/P'(a_i)=0$ whenever $\deg p\leq n-2$: this sum is the coefficient of $X^{n-1}$ in the interpolation formula for $p$. Taking $p=fh$ with $\deg f<k$ and $\deg h<n-k$ proves orthogonality of $C$ and $\operatorname{GRS}_{n-k}(a,u)$. Comparing [dimensions](../../../../../dimension-vector-space.md) gives equality with $C^\perp$. An unweighted evaluation [linear code](../../../../../linear-code.md) at arbitrary points need not have an unweighted evaluation dual at the same points; the multiplier form and the cyclic offset formula resolve that convention issue.

For the length-$15$, dimension-$11$ [linear code](../../../../../linear-code.md), choose $b=1$ and $\omega\in\mathbb F_{16}$ as in the [field](../../../../../field.md) table. Then $d=15-11+1=5$ and

$$
g_1(X)=\prod_{t=1}^4(X-\omega^t).
$$

The [field characteristic](../../../../../characteristic-of-a-field.md) is two, and the table gives $\omega^4=\omega+1$. In the [basis](../../../../../basis.md) $1,\omega,\omega^2,\omega^3$, the four roots are represented by $0010,0100,1000,0011$. Their elementary symmetric functions are

$$
\begin{aligned}
s_1&=\omega+\omega^2+\omega^3+\omega^4=\omega^{13},\\
s_2&=\omega^3+\omega^4+\omega^5+\omega^5+\omega^6+\omega^7=\omega^6,\\
s_3&=\omega^6+\omega^7+\omega^8+\omega^9=\omega^3,\\
s_4&=\omega^{1+2+3+4}=\omega^{10}.
\end{aligned}
$$

The repeated terms in $s_2$ cancel because the [field characteristic](../../../../../characteristic-of-a-field.md) is two. There are no alternating minus signs in this characteristic, so

$$
\boxed{g_1(X)=\omega^{10}+\omega^3X+\omega^6X^2+\omega^{13}X^3+\omega^0X^4,\qquad d=5.}
$$

For example, the coefficient [vectors](../../../../../vector.md) in ascending order are $0111,1000,1100,1101,0001$, giving the required single powers of $\omega$.

For the length-$10$, dimension-$6$ [linear code](../../../../../linear-code.md) over $\mathbb F_{11}$, take the table's [primitive element of a finite field](../../../../../primitive-element-of-a-finite-field.md) $\omega=2$ and again $b=1$. The four roots are $2,4,8,5$. Expanding in $\mathbb F_{11}[X]$ gives

$$
\begin{aligned}
g_2(X)&=(X-2)(X-4)(X-8)(X-5)\\
&=(X^2+5X+8)(X^2+9X+7)\\
&=X^4+3X^3+5X^2+8X+1.
\end{aligned}
$$

Thus

$$
\boxed{g_2(X)=1+8X+5X^2+3X^3+X^4,\qquad d=10-6+1=5.}
$$

The coefficients are reduced modulo $11$, including the constant term $2\cdot4\cdot8\cdot5=1\pmod{11}$.

A suitable two-error-correcting [Reed-Solomon code](../../../../../reed-solomon-error-correction.md) over $\mathbb F_{16}$ is precisely the first [linear code](../../../../../linear-code.md):

$$
\boxed{[n,k,d]_{16}=[15,11,5]_{16},\qquad g(X)=g_1(X).}
$$

Two distinct [codewords](../../../../../codeword.md) cannot both be within [Hamming distance](../../../../../hamming-distance.md) two of a received word, because the [triangle inequality](../../../../../triangle-inequality.md) would put them at distance at most four. Thus this [linear code](../../../../../linear-code.md) corrects any two symbol errors. Its [generator polynomial](../../../../../generator-polynomial-of-a-cyclic-code.md) has four consecutive [defining zeros of a cyclic code](../../../../../zero-of-a-cyclic-code.md), and its [dimension](../../../../../dimension-vector-space.md) and exact [minimum Hamming distance](../../../../../minimum-distance-of-a-code.md) have already been proved.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
