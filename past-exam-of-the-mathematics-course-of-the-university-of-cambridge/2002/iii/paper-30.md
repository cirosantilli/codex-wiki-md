# Paper 30

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper30.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper30.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Let $a_1,\ldots,a_n$ be distinct elements of a [finite field](../../../algebra.md#finite-field) $\mathbb F_q$, with $1\leq k\leq n$. The [Reed-Solomon code](../../../coding-theory.md#reed-solomon-error-correction) consists of the evaluation [vectors](../../../vector-space.md#vector)

$$
\operatorname{RS}_k(a)=\{(f(a_1),\ldots,f(a_n)):f\in\mathbb F_q[X],\ \deg f<k\}.
$$

Evaluation is an [injective](../../../algebra.md#injective-function) [linear map](../../../vector-space.md#linear-map): a nonzero [polynomial](../../../polynomial.md) of degree at most $k-1$ cannot vanish at all $n$ distinct points. Thus the [dimension](../../../vector-space.md#dimension-vector-space) is $k$. The same bound on [polynomial roots](../../../polynomial.md#root-of-a-polynomial) shows that every nonzero [codeword](../../../coding-theory.md#codeword) has [Hamming weight](../../../coding-theory.md#hamming-weight) at least $n-k+1$. Conversely, choosing any $k-1$ evaluation points and taking their product of linear factors gives a [polynomial](../../../polynomial.md) whose evaluation vanishes at exactly those points. Its [Hamming weight](../../../coding-theory.md#hamming-weight) is $n-k+1$. Hence

$$
\boxed{d=n-k+1.}
$$

For completeness, deleting $d-1$ coordinates from a [linear code](../../../coding-theory.md#linear-code) of [minimum Hamming distance](../../../coding-theory.md#minimum-distance-of-a-code) $d$ is injective on [codewords](../../../coding-theory.md#codeword), since two words with the same retained coordinates would differ in fewer than $d$ positions. Therefore $q^k\leq q^{n-d+1}$, giving the [Singleton bound](../../../coding-theory.md#singleton-bound) $d\leq n-k+1$. The [Reed-Solomon code](../../../coding-theory.md#reed-solomon-error-correction) attains this bound and is a [maximum distance separable code](../../../coding-theory.md#maximum-distance-separable-code). Multiplying individual coordinates by nonzero [field](../../../algebra.md#field) elements changes neither the [dimension](../../../vector-space.md#dimension-vector-space) nor the [Hamming weight](../../../coding-theory.md#hamming-weight), so the same proof applies to a [generalized Reed-Solomon code](../../../coding-theory.md#generalized-reed-solomon-code).

To specify the [generator polynomials of a cyclic code](../../../coding-theory.md#generator-polynomial-of-a-cyclic-code) unambiguously, use the [primitive cyclic Reed-Solomon code](../../../coding-theory.md#primitive-cyclic-reed-solomon-code) convention. Put $n=q-1$, choose a [primitive element of a finite field](../../../algebra.md#primitive-element-of-a-finite-field) $\omega$, and set

$$
C_{k,b}=\langle g_b(X)\rangle\subseteq\mathbb F_q[X]/(X^n-1),\qquad
 g_b(X)=\prod_{t=b}^{b+n-k-1}(X-\omega^t).
$$

Exponents are taken modulo $n$. This [generator polynomial](../../../coding-theory.md#generator-polynomial-of-a-cyclic-code) is a [monic polynomial](../../../polynomial.md#monic-polynomial) of degree $n-k$ dividing $X^n-1$, so the [dimension](../../../vector-space.md#dimension-vector-space) is $k$. It agrees with the evaluation form

$$
C_{k,b}=\{(a_j^{1-b}f(a_j))_{j=0}^{n-1}:\deg f<k\},\qquad a_j=\omega^j.
$$

Indeed, at a defining exponent $t=b,\ldots,b+n-k-1$, a monomial $f(X)=X^s$ contributes the [finite geometric series](../../../real-analysis.md#finite-geometric-series) $\sum_j a_j^{t+1-b+s}$. Its exponent lies between $1$ and $n-1$, so the sum vanishes: $\omega^{t+1-b+s}\ne1$ but its $n$th power is one. Every displayed evaluation [vector](../../../vector-space.md#vector) therefore lies in the [cyclic code](../../../coding-theory.md#cyclic-code), and both spaces have [dimension](../../../vector-space.md#dimension-vector-space) $k$, proving equality. The narrow-sense choice $b=1$ is the ordinary unweighted evaluation [linear code](../../../coding-theory.md#linear-code) on all nonzero [field](../../../algebra.md#field) elements.

The [duality of primitive cyclic Reed-Solomon codes](../../../coding-theory.md#duality-of-primitive-cyclic-reed-solomon-codes) now follows directly. A [vector](../../../vector-space.md#vector) in $C_{k,b}$ has coordinates $a_j^{1-b}f(a_j)$, while a [vector](../../../vector-space.md#vector) in $C_{n-k,1-b}$ has coordinates $a_j^b h(a_j)$, with $\deg h<n-k$. Their [dot product](../../../linear-algebra.md#dot-product) is $\sum_j a_j f(a_j)h(a_j)$. Every appearing exponent is between $1$ and $n-1$, so every such [finite geometric series](../../../real-analysis.md#finite-geometric-series) is zero. The two spaces are orthogonal and their [dimensions](../../../vector-space.md#dimension-vector-space) sum to $n$, giving

$$
\boxed{C_{k,b}^{\perp}=C_{n-k,1-b}.}
$$

Thus the full cyclic family is closed under [dual codes](../../../coding-theory.md#dual-code). The offset matters: the [dual code](../../../coding-theory.md#dual-code) of the narrow-sense [linear code](../../../coding-theory.md#linear-code) generally has offset zero, rather than one.

For arbitrary evaluation points, the precise statement is closure of [generalized Reed-Solomon codes](../../../coding-theory.md#generalized-reed-solomon-code) under duality. If $C=\operatorname{GRS}_k(a,v)$, put $P(X)=\prod_i(X-a_i)$ and $u_i=(v_iP'(a_i))^{-1}$. [Lagrange interpolation](../../../numerical-analysis.md#lagrange-polynomial) shows $\sum_i p(a_i)/P'(a_i)=0$ whenever $\deg p\leq n-2$: this sum is the coefficient of $X^{n-1}$ in the interpolation formula for $p$. Taking $p=fh$ with $\deg f<k$ and $\deg h<n-k$ proves orthogonality of $C$ and $\operatorname{GRS}_{n-k}(a,u)$. Comparing [dimensions](../../../vector-space.md#dimension-vector-space) gives equality with $C^\perp$. An unweighted evaluation [linear code](../../../coding-theory.md#linear-code) at arbitrary points need not have an unweighted evaluation dual at the same points; the multiplier form and the cyclic offset formula resolve that convention issue.

For the length-$15$, dimension-$11$ [linear code](../../../coding-theory.md#linear-code), choose $b=1$ and $\omega\in\mathbb F_{16}$ as in the [field](../../../algebra.md#field) table. Then $d=15-11+1=5$ and

$$
g_1(X)=\prod_{t=1}^4(X-\omega^t).
$$

The [field characteristic](../../../algebra.md#characteristic-of-a-field) is two, and the table gives $\omega^4=\omega+1$. In the [basis](../../../vector-space.md#basis) $1,\omega,\omega^2,\omega^3$, the four roots are represented by $0010,0100,1000,0011$. Their elementary symmetric functions are

$$
\begin{aligned}
s_1&=\omega+\omega^2+\omega^3+\omega^4=\omega^{13},\\
s_2&=\omega^3+\omega^4+\omega^5+\omega^5+\omega^6+\omega^7=\omega^6,\\
s_3&=\omega^6+\omega^7+\omega^8+\omega^9=\omega^3,\\
s_4&=\omega^{1+2+3+4}=\omega^{10}.
\end{aligned}
$$

The repeated terms in $s_2$ cancel because the [field characteristic](../../../algebra.md#characteristic-of-a-field) is two. There are no alternating minus signs in this characteristic, so

$$
\boxed{g_1(X)=\omega^{10}+\omega^3X+\omega^6X^2+\omega^{13}X^3+\omega^0X^4,\qquad d=5.}
$$

For example, the coefficient [vectors](../../../vector-space.md#vector) in ascending order are $0111,1000,1100,1101,0001$, giving the required single powers of $\omega$.

For the length-$10$, dimension-$6$ [linear code](../../../coding-theory.md#linear-code) over $\mathbb F_{11}$, take the table's [primitive element of a finite field](../../../algebra.md#primitive-element-of-a-finite-field) $\omega=2$ and again $b=1$. The four roots are $2,4,8,5$. Expanding in $\mathbb F_{11}[X]$ gives

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

A suitable two-error-correcting [Reed-Solomon code](../../../coding-theory.md#reed-solomon-error-correction) over $\mathbb F_{16}$ is precisely the first [linear code](../../../coding-theory.md#linear-code):

$$
\boxed{[n,k,d]_{16}=[15,11,5]_{16},\qquad g(X)=g_1(X).}
$$

Two distinct [codewords](../../../coding-theory.md#codeword) cannot both be within [Hamming distance](../../../coding-theory.md#hamming-distance) two of a received word, because the [triangle inequality](../../../topological-analysis.md#triangle-inequality) would put them at distance at most four. Thus this [linear code](../../../coding-theory.md#linear-code) corrects any two symbol errors. Its [generator polynomial](../../../coding-theory.md#generator-polynomial-of-a-cyclic-code) has four consecutive [defining zeros of a cyclic code](../../../coding-theory.md#zero-of-a-cyclic-code), and its [dimension](../../../vector-space.md#dimension-vector-space) and exact [minimum Hamming distance](../../../coding-theory.md#minimum-distance-of-a-code) have already been proved.

## 2

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For a [binary linear code](../../../coding-theory.md#binary-linear-code) $C\subseteq\mathbb F_2^n$, define the [linear functional](../../../linear-algebra.md#linear-functional) $\sigma(x)=\sum_{j=1}^n x_j\in\mathbb F_2$. This is the parity of the [Hamming weight](../../../coding-theory.md#hamming-weight), so the [even-weight subcode of a binary linear code](../../../coding-theory.md#even-weight-subcode-of-a-binary-linear-code) is

$$
C^{\mathrm{ev}}=\ker(\sigma|_C).
$$

If $\sigma|_C=0$, then $C^{\mathrm{ev}}=C$. Otherwise its image is all of $\mathbb F_2$, and [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem) gives $\dim C^{\mathrm{ev}}=k-1$. The [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map) is a [linear subspace](../../../vector-space.md#vector-subspace), proving the required dichotomy including closure under addition.

Let $G$ be a full-rank $k\times n$ [generator matrix](../../../coding-theory.md#generator-matrix). Messages $a\in\mathbb F_2^k$ correspond bijectively to [codewords](../../../coding-theory.md#codeword) $aG$. If the $j$th column $g_j$ is nonzero, the coordinate $a\mapsto a\cdot g_j$ is a nonzero [linear functional](../../../linear-algebra.md#linear-functional). Choose $a_0$ with $a_0\cdot g_j=1$. Translation $a\mapsto a+a_0$ pairs the messages with coordinate zero and those with coordinate one, so exactly $2^{k-1}$ [codewords](../../../coding-theory.md#codeword) contribute one at position $j$. Summing over the $n$ columns proves the [total weight of a full-support binary linear code](../../../coding-theory.md#total-weight-of-a-full-support-binary-linear-code) formula

$$
\boxed{\sum_{x\in C}w(x)=\sum_{j=1}^n\#\{a:a\cdot g_j=1\}=n2^{k-1}.}
$$

A zero column would contribute zero instead, explaining the hypothesis.

For the [Hamming code](../../../coding-theory.md#hamming-code), use a [parity-check matrix](../../../coding-theory.md#parity-check-matrix) $H$ whose columns are all nonzero [vectors](../../../vector-space.md#vector) of $V=\mathbb F_2^\ell$, once each. Then $C_{H,\ell}=\ker H$ and $n=2^\ell-1$. The sum of all columns is zero: each coordinate occurs as one exactly $2^{\ell-1}$ times, which is even for $\ell\geq3$. Consequently

$$
\boxed{(1,\ldots,1)\in C_{H,\ell}\quad\text{for every }\ell\geq3.}
$$

Under this column labelling, the [support of a vector](../../../numerical-analysis.md#support-of-a-vector) of a [codeword](../../../coding-theory.md#codeword) is identified with a set of distinct nonzero columns whose sum is zero. No one-column or two-column [support of a vector](../../../numerical-analysis.md#support-of-a-vector) has this property, confirming $A_1=A_2=0$.

We can count the [low-weight coefficients of a binary Hamming code](../../../coding-theory.md#low-weight-coefficients-of-a-binary-hamming-code) directly. For weight three, choose ordered distinct nonzero columns $a,b$ in $n(n-1)$ ways. The third must be $a+b$, which is nonzero and different from both. Every unordered [support of a vector](../../../numerical-analysis.md#support-of-a-vector) has $3!$ orderings, so $A_3=n(n-1)/3!$.

For weight four, the first two columns $a,b$ are again distinct and nonzero. The third $c$ must avoid $a,b,a+b$, giving $n-3$ possibilities. The fourth is $d=a+b+c$; it is nonzero because $c\ne a+b$, and cannot equal any of the first three because those are distinct. Conversely every ordered zero-sum four-tuple arises in this way. Dividing by $4!$ gives $A_4=n(n-1)(n-3)/4!$.

For weight five, the first three columns $a,b,c$ must be linearly independent. If $a+b+c=0$, the sum condition would force the fourth and fifth to coincide. Thus there are $n(n-1)(n-3)$ choices for the first three. Put $t=a+b+c$. The fourth column $d$ must avoid all seven nonzero [vectors](../../../vector-space.md#vector) of their [linear span](../../../vector-space.md#linear-span): $a,b,c$ would repeat a column; $t$ would force the fifth column to be zero; and $a+b,a+c,b+c$ would force the fifth column to be $c,b,a$, respectively. Conversely, if $d$ avoids these seven [vectors](../../../vector-space.md#vector), $e=t+d$ is nonzero and distinct from $a,b,c,d$. This gives $n-7$ choices for $d$ and determines $e$. Dividing by $5!$ yields

$$
\boxed{A_3=\frac{n(n-1)}{3!},\qquad A_4=\frac{n(n-1)(n-3)}{4!},\qquad A_5=\frac{n(n-1)(n-3)(n-7)}{5!}.}
$$

At $\ell=3$, the last count is zero, as the argument also shows.

The [dual code](../../../coding-theory.md#dual-code) $C_{H,\ell}^{\perp}$ is the [row space](../../../vector-space.md#row-space) of $H$, so its [codewords](../../../coding-theory.md#codeword) are $aH$ for $a\in\mathbb F_2^\ell$. For nonzero $a$, the [linear functional](../../../linear-algebra.md#linear-functional) $v\mapsto a\cdot v$ takes value one on exactly half the $2^\ell$ [vectors](../../../vector-space.md#vector) of $V$, by the same translation-pairing argument used above. Removing the zero [vector](../../../vector-space.md#vector) removes only a zero value, so the [Hamming weight](../../../coding-theory.md#hamming-weight) is still $m=2^{\ell-1}$. Since $H$ has [matrix rank](../../../vector-space.md#matrix-rank) $\ell$, distinct $a$ give distinct [codewords](../../../coding-theory.md#codeword). This proves the [constant weight of a binary simplex code](../../../coding-theory.md#constant-weight-of-a-binary-simplex-code) and its full distribution:

$$
\boxed{A_0^{\perp}=1,\qquad A_m^{\perp}=2^\ell-1=n,\qquad A_s^{\perp}=0\ (s\ne0,m).}
$$

In particular, the ordinary [weight enumerator](../../../coding-theory.md#weight-enumerator) of the [binary simplex code](../../../coding-theory.md#binary-simplex-code) is $1+nz^m$.

Apply the [MacWilliams identity](../../../coding-theory.md#macwilliams-identity) to this [dual code](../../../coding-theory.md#dual-code), whose size is $2^\ell=n+1$. For $W_C(z)=\sum_sA_sz^s$, the result is

$$
W_{C_{H,\ell}}(z)=\frac{(1+z)^n+n(1-z)^m(1+z)^{n-m}}{n+1}.
$$

The coefficient of $z^s$ in the second product is a value of the binary [Kravchuk polynomials](../../../numerical-analysis.md#kravchuk-polynomials)

$$
K_s(m;n,2)=\sum_{j=\max(0,s-(n-m))}^{\min(s,m)}(-1)^j\binom mj\binom{n-m}{s-j}.
$$

These bounds merely enforce $0\leq j\leq m$ and $0\leq s-j\leq n-m$. Since $n-m=2^{\ell-1}-1$, they agree with the bounds in the PDF. Therefore the requested formula is

$$
\boxed{A_s=\frac{1}{2^\ell}\left[\binom ns+nK_s(2^{\ell-1};n,2)\right].}
$$

For a further check on the low-weight counts, $n=2m-1$ gives

$$
(1-z)^m(1+z)^{m-1}=(1-z)(1-z^2)^{m-1}.
$$

Thus $K_3(m)=m-1$, $K_4(m)=\binom{m-1}{2}$, and $K_5(m)=-\binom{m-1}{2}$. Substituting these into the boxed formula and using $m=(n+1)/2$ reproduces the three direct combinatorial counts above.

Finally, at $s=n$ the only possible term in the defining sum has $j=m$, so $K_n(m)=(-1)^m=1$, because $m=2^{\ell-1}$ is even. Consequently

$$
\boxed{A_n=\frac{1+n}{n+1}=1.}
$$

The unique length-$n$ binary word of weight $n$ is the all-ones word, exactly as proved by the [parity-check matrix](../../../coding-theory.md#parity-check-matrix) calculation.

## 3

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use $\mathbb F_{32}=\mathbb F_2[\omega]$ with $\omega^5=\omega^2+1$. The given [primitive polynomial over a finite field](../../../algebra.md#primitive-polynomial-over-a-finite-field) makes $\omega$ have order $31$. For a binary [cyclic code](../../../coding-theory.md#cyclic-code), squaring a zero preserves the zero condition: $v(\omega)^2=v(\omega^2)$ for $v\in\mathbb F_2[X]$. Thus the [binary cyclotomic cosets modulo an odd integer](../../../coding-theory.md#binary-cyclotomic-coset-modulo-an-odd-integer) governing the four specified zeros are

$$
\boxed{C_1=C_2=C_4=\{1,2,4,8,16\},\qquad C_3=\{3,6,12,24,17\}\pmod{31}.}
$$

The two displayed orbits are disjoint, each has size five, and together contain $1,2,3,4$. Therefore specifying $\omega$ and $\omega^3$ already forces all four consecutive [defining zeros of a cyclic code](../../../coding-theory.md#zero-of-a-cyclic-code).

The [minimal polynomial of an algebraic element](../../../galois-theory.md#minimal-polynomial-of-an-algebraic-element) of $\omega$ is $m_1(X)=X^5+X^2+1$. For $\omega^3$, the orbit size shows that its [algebraic minimal polynomial](../../../galois-theory.md#minimal-polynomial-of-an-algebraic-element) has degree five. The candidate $m_3(X)=X^5+X^4+X^3+X^2+1$ vanishes there, since

$$
m_3(\omega^3)=\omega^{15}+\omega^{12}+\omega^9+\omega^6+1=0.
$$

For example, the five-bit representations of these terms are $11111,01110,11010,01010,00001$, whose sum is zero in $\mathbb F_2^5$. As $m_3$ is a [monic polynomial](../../../polynomial.md#monic-polynomial) of degree five and annihilates $\omega^3$, it is precisely its [algebraic minimal polynomial](../../../galois-theory.md#minimal-polynomial-of-an-algebraic-element); no assumption that the provided [polynomial](../../../polynomial.md) list is exhaustive is necessary.

The narrow-sense primitive [BCH code](../../../coding-theory.md#bch-code) is

$$
\mathcal X=\{v\in\mathbb F_2[X],\ \deg v<31:\ v(\omega)=v(\omega^3)=0\}.
$$

Both [algebraic minimal polynomials](../../../galois-theory.md#minimal-polynomial-of-an-algebraic-element) divide each such $v$, and they are [coprime polynomials](../../../polynomial.md#coprime-polynomials). Their product is a divisor of $X^{31}-1$. Hence the [generator polynomial](../../../coding-theory.md#generator-polynomial-of-a-cyclic-code) is their product. Direct multiplication with [field characteristic](../../../algebra.md#characteristic-of-a-field) two gives

$$
\boxed{g(X)=m_1(X)m_3(X)=X^{10}+X^9+X^8+X^6+X^5+X^3+1,\qquad\dim\mathcal X=21.}
$$

The [designed distance](../../../coding-theory.md#designed-distance) is five, because $g$ vanishes at the four consecutive powers $\omega,\omega^2,\omega^3,\omega^4$.

Here is an explicit [BCH bound](../../../coding-theory.md#bch-bound) proof for these zeros. If a nonzero [codeword](../../../coding-theory.md#codeword) had [support of a vector](../../../numerical-analysis.md#support-of-a-vector) of size $\nu\leq4$, with distinct positions $i_1,\ldots,i_\nu$ and nonzero coefficients $b_1,\ldots,b_\nu$, put $\lambda_r=\omega^{i_r}$. Evaluating at the first $\nu$ defining powers gives

$$
\sum_{r=1}^\nu b_r\lambda_r^j=0\qquad(1\leq j\leq\nu).
$$

The coefficient [matrix](../../../vector-space.md#matrix) has [determinant](../../../linear-algebra.md#determinant) $\bigl(\prod_r\lambda_r\bigr)\prod_{r<s}(\lambda_s-\lambda_r)$, a nonzero [Vandermonde determinant](../../../galois-theory.md#vandermonde-determinant) because the $\lambda_r$ are distinct and nonzero. It therefore forces every $b_r=0$, a contradiction. Thus the [minimum Hamming distance](../../../coding-theory.md#minimum-distance-of-a-code) is at least five.

For the matching upper bound, multiplication gives the actual [codeword](../../../coding-theory.md#codeword)

$$
(1+X^2+X^3)g(X)=1+X^2+X^7+X^8+X^{13},
$$

which has [Hamming weight](../../../coding-theory.md#hamming-weight) five and degree below $31$. Hence

$$
\boxed{\mathcal X\text{ has parameters }[31,21,5]_2.}
$$

This proves the actual distance without needing the optional theorem. Its numerical hypothesis is also satisfied: with $s=5$ and the error parameter $l=2$, $2^{sl}=2^{10}=1024$, whereas $\sum_{i=0}^{3}\binom{31}{i}=1+31+465+4495=4992$.

Now calculate the [root-evaluation syndrome for a cyclic code](../../../coding-theory.md#root-evaluation-syndrome-for-a-cyclic-code) from the received [polynomial](../../../polynomial.md). Reduction modulo $m_1(X)$ gives $u(X)\equiv X^3$, so $S_1=u(\omega)=\omega^3$. Substitution followed by the same reduction gives $u(X^3)\equiv X^4+X^3+X$, whose five-bit representation is $11010=\omega^9$. Thus

$$
\boxed{S_1=\omega^3,\qquad S_3=u(\omega^3)=\omega^9=S_1^3.}
$$

The [single-error test from two binary BCH syndromes](../../../coding-theory.md#single-error-test-from-two-binary-bch-syndromes) identifies coordinate $3$, since a one-bit error $X^j$ has [syndromes](../../../coding-theory.md#syndrome) $\omega^j,\omega^{3j}$. Flip that coordinate to obtain

$$
\boxed{c_{\mathrm{correct}}(X)=u(X)+X^3=X^{12}+X^{11}+X^9+X^7+X^6+X^3+X^2+1.}
$$

Both defining evaluations vanish: $c_{\mathrm{correct}}(\omega)=\omega^3+\omega^3=0$ and $c_{\mathrm{correct}}(\omega^3)=\omega^9+\omega^9=0$. More directly,

$$
c_{\mathrm{correct}}(X)=(1+X^2)g(X),
$$

so it is certainly a [codeword](../../../coding-theory.md#codeword) of $\mathcal X$. It is at [Hamming distance](../../../coding-theory.md#hamming-distance) one from $u$. Since the [minimum Hamming distance](../../../coding-theory.md#minimum-distance-of-a-code) is five, no other [codeword](../../../coding-theory.md#codeword) can be within two errors of $u$: such a word would be at distance at most three from $c_{\mathrm{correct}}$, contradicting the proved distance. Thus this is the unique [bounded-distance decoding](../../../coding-theory.md#bounded-distance-decoding) under the [linear code](../../../coding-theory.md#linear-code)'s two-error guarantee.

**The decoded [polynomial](../../../polynomial.md) printed in the original PDF is incorrect.** It instead adds $X^{10}$ to $u$, giving a [polynomial](../../../polynomial.md) $c_{\mathrm{printed}}=u+X^{10}$. Its defining evaluations are

$$
c_{\mathrm{printed}}(\omega)=\omega^3+\omega^{10}=\omega^{25}\ne0,\qquad
c_{\mathrm{printed}}(\omega^3)=\omega^9+\omega^{30}=\omega^3\ne0.
$$

Therefore it is not a [codeword](../../../coding-theory.md#codeword), and the request to verify that it belongs to $\mathcal X$ is a false premise. The [field](../../../algebra.md#field) table and the printed [syndromes](../../../coding-theory.md#syndrome) agree with correction at $X^3$; the correction at $X^{10}$ does not. The boxed corrected [polynomial](../../../polynomial.md) resolves this source error and supplies the intended decoding and membership proof.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
