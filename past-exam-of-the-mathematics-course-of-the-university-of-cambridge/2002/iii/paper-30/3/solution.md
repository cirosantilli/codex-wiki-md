<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use $\mathbb F_{32}=\mathbb F_2[\omega]$ with $\omega^5=\omega^2+1$. The given [primitive polynomial over a finite field](../../../../../primitive-polynomial-over-a-finite-field.md) makes $\omega$ have order $31$. For a binary [cyclic code](../../../../../cyclic-code.md), squaring a zero preserves the zero condition: $v(\omega)^2=v(\omega^2)$ for $v\in\mathbb F_2[X]$. Thus the [binary cyclotomic cosets modulo an odd integer](../../../../../binary-cyclotomic-coset-modulo-an-odd-integer.md) governing the four specified zeros are

$$
\boxed{C_1=C_2=C_4=\{1,2,4,8,16\},\qquad C_3=\{3,6,12,24,17\}\pmod{31}.}
$$

The two displayed orbits are disjoint, each has size five, and together contain $1,2,3,4$. Therefore specifying $\omega$ and $\omega^3$ already forces all four consecutive [defining zeros of a cyclic code](../../../../../zero-of-a-cyclic-code.md).

The [minimal polynomial of an algebraic element](../../../../../minimal-polynomial-of-an-algebraic-element.md) of $\omega$ is $m_1(X)=X^5+X^2+1$. For $\omega^3$, the orbit size shows that its [algebraic minimal polynomial](../../../../../minimal-polynomial-of-an-algebraic-element.md) has degree five. The candidate $m_3(X)=X^5+X^4+X^3+X^2+1$ vanishes there, since

$$
m_3(\omega^3)=\omega^{15}+\omega^{12}+\omega^9+\omega^6+1=0.
$$

For example, the five-bit representations of these terms are $11111,01110,11010,01010,00001$, whose sum is zero in $\mathbb F_2^5$. As $m_3$ is a [monic polynomial](../../../../../monic-polynomial.md) of degree five and annihilates $\omega^3$, it is precisely its [algebraic minimal polynomial](../../../../../minimal-polynomial-of-an-algebraic-element.md); no assumption that the provided [polynomial](../../../../../polynomial-split.md) list is exhaustive is necessary.

The narrow-sense primitive [BCH code](../../../../../bch-code.md) is

$$
\mathcal X=\{v\in\mathbb F_2[X],\ \deg v<31:\ v(\omega)=v(\omega^3)=0\}.
$$

Both [algebraic minimal polynomials](../../../../../minimal-polynomial-of-an-algebraic-element.md) divide each such $v$, and they are [coprime polynomials](../../../../../coprime-polynomials.md). Their product is a divisor of $X^{31}-1$. Hence the [generator polynomial](../../../../../generator-polynomial-of-a-cyclic-code.md) is their product. Direct multiplication with [field characteristic](../../../../../characteristic-of-a-field.md) two gives

$$
\boxed{g(X)=m_1(X)m_3(X)=X^{10}+X^9+X^8+X^6+X^5+X^3+1,\qquad\dim\mathcal X=21.}
$$

The [designed distance](../../../../../designed-distance.md) is five, because $g$ vanishes at the four consecutive powers $\omega,\omega^2,\omega^3,\omega^4$.

Here is an explicit [BCH bound](../../../../../bch-bound.md) proof for these zeros. If a nonzero [codeword](../../../../../codeword.md) had [support of a vector](../../../../../support-of-a-vector.md) of size $\nu\leq4$, with distinct positions $i_1,\ldots,i_\nu$ and nonzero coefficients $b_1,\ldots,b_\nu$, put $\lambda_r=\omega^{i_r}$. Evaluating at the first $\nu$ defining powers gives

$$
\sum_{r=1}^\nu b_r\lambda_r^j=0\qquad(1\leq j\leq\nu).
$$

The coefficient [matrix](../../../../../matrix.md) has [determinant](../../../../../determinant.md) $\bigl(\prod_r\lambda_r\bigr)\prod_{r<s}(\lambda_s-\lambda_r)$, a nonzero [Vandermonde determinant](../../../../../vandermonde-determinant.md) because the $\lambda_r$ are distinct and nonzero. It therefore forces every $b_r=0$, a contradiction. Thus the [minimum Hamming distance](../../../../../minimum-distance-of-a-code.md) is at least five.

For the matching upper bound, multiplication gives the actual [codeword](../../../../../codeword.md)

$$
(1+X^2+X^3)g(X)=1+X^2+X^7+X^8+X^{13},
$$

which has [Hamming weight](../../../../../hamming-weight.md) five and degree below $31$. Hence

$$
\boxed{\mathcal X\text{ has parameters }[31,21,5]_2.}
$$

This proves the actual distance without needing the optional theorem. Its numerical hypothesis is also satisfied: with $s=5$ and the error parameter $l=2$, $2^{sl}=2^{10}=1024$, whereas $\sum_{i=0}^{3}\binom{31}{i}=1+31+465+4495=4992$.

Now calculate the [root-evaluation syndrome for a cyclic code](../../../../../root-evaluation-syndrome-for-a-cyclic-code.md) from the received [polynomial](../../../../../polynomial-split.md). Reduction modulo $m_1(X)$ gives $u(X)\equiv X^3$, so $S_1=u(\omega)=\omega^3$. Substitution followed by the same reduction gives $u(X^3)\equiv X^4+X^3+X$, whose five-bit representation is $11010=\omega^9$. Thus

$$
\boxed{S_1=\omega^3,\qquad S_3=u(\omega^3)=\omega^9=S_1^3.}
$$

The [single-error test from two binary BCH syndromes](../../../../../single-error-test-from-two-binary-bch-syndromes.md) identifies coordinate $3$, since a one-bit error $X^j$ has [syndromes](../../../../../syndrome.md) $\omega^j,\omega^{3j}$. Flip that coordinate to obtain

$$
\boxed{c_{\mathrm{correct}}(X)=u(X)+X^3=X^{12}+X^{11}+X^9+X^7+X^6+X^3+X^2+1.}
$$

Both defining evaluations vanish: $c_{\mathrm{correct}}(\omega)=\omega^3+\omega^3=0$ and $c_{\mathrm{correct}}(\omega^3)=\omega^9+\omega^9=0$. More directly,

$$
c_{\mathrm{correct}}(X)=(1+X^2)g(X),
$$

so it is certainly a [codeword](../../../../../codeword.md) of $\mathcal X$. It is at [Hamming distance](../../../../../hamming-distance.md) one from $u$. Since the [minimum Hamming distance](../../../../../minimum-distance-of-a-code.md) is five, no other [codeword](../../../../../codeword.md) can be within two errors of $u$: such a word would be at distance at most three from $c_{\mathrm{correct}}$, contradicting the proved distance. Thus this is the unique [bounded-distance decoding](../../../../../bounded-distance-decoding.md) under the [linear code](../../../../../linear-code.md)'s two-error guarantee.

**The decoded [polynomial](../../../../../polynomial-split.md) printed in the original PDF is incorrect.** It instead adds $X^{10}$ to $u$, giving a [polynomial](../../../../../polynomial-split.md) $c_{\mathrm{printed}}=u+X^{10}$. Its defining evaluations are

$$
c_{\mathrm{printed}}(\omega)=\omega^3+\omega^{10}=\omega^{25}\ne0,\qquad
c_{\mathrm{printed}}(\omega^3)=\omega^9+\omega^{30}=\omega^3\ne0.
$$

Therefore it is not a [codeword](../../../../../codeword.md), and the request to verify that it belongs to $\mathcal X$ is a false premise. The [field](../../../../../field.md) table and the printed [syndromes](../../../../../syndrome.md) agree with correction at $X^3$; the correction at $X^{10}$ does not. The boxed corrected [polynomial](../../../../../polynomial-split.md) resolves this source error and supplies the intended decoding and membership proof.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
