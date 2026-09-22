<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a [binary linear code](../../../../../binary-linear-code.md) $C\subseteq\mathbb F_2^n$, define the [linear functional](../../../../../linear-functional.md) $\sigma(x)=\sum_{j=1}^n x_j\in\mathbb F_2$. This is the parity of the [Hamming weight](../../../../../hamming-weight.md), so the [even-weight subcode of a binary linear code](../../../../../even-weight-subcode-of-a-binary-linear-code.md) is

$$
C^{\mathrm{ev}}=\ker(\sigma|_C).
$$

If $\sigma|_C=0$, then $C^{\mathrm{ev}}=C$. Otherwise its image is all of $\mathbb F_2$, and [rank-nullity theorem](../../../../../rank-nullity-theorem.md) gives $\dim C^{\mathrm{ev}}=k-1$. The [kernel of a linear map](../../../../../kernel-of-a-linear-map.md) is a [linear subspace](../../../../../vector-subspace.md), proving the required dichotomy including closure under addition.

Let $G$ be a full-rank $k\times n$ [generator matrix](../../../../../generator-matrix.md). Messages $a\in\mathbb F_2^k$ correspond bijectively to [codewords](../../../../../codeword.md) $aG$. If the $j$th column $g_j$ is nonzero, the coordinate $a\mapsto a\cdot g_j$ is a nonzero [linear functional](../../../../../linear-functional.md). Choose $a_0$ with $a_0\cdot g_j=1$. Translation $a\mapsto a+a_0$ pairs the messages with coordinate zero and those with coordinate one, so exactly $2^{k-1}$ [codewords](../../../../../codeword.md) contribute one at position $j$. Summing over the $n$ columns proves the [total weight of a full-support binary linear code](../../../../../total-weight-of-a-full-support-binary-linear-code.md) formula

$$
\boxed{\sum_{x\in C}w(x)=\sum_{j=1}^n\#\{a:a\cdot g_j=1\}=n2^{k-1}.}
$$

A zero column would contribute zero instead, explaining the hypothesis.

For the [Hamming code](../../../../../hamming-code.md), use a [parity-check matrix](../../../../../parity-check-matrix.md) $H$ whose columns are all nonzero [vectors](../../../../../vector.md) of $V=\mathbb F_2^\ell$, once each. Then $C_{H,\ell}=\ker H$ and $n=2^\ell-1$. The sum of all columns is zero: each coordinate occurs as one exactly $2^{\ell-1}$ times, which is even for $\ell\geq3$. Consequently

$$
\boxed{(1,\ldots,1)\in C_{H,\ell}\quad\text{for every }\ell\geq3.}
$$

Under this column labelling, the [support of a vector](../../../../../support-of-a-vector.md) of a [codeword](../../../../../codeword.md) is identified with a set of distinct nonzero columns whose sum is zero. No one-column or two-column [support of a vector](../../../../../support-of-a-vector.md) has this property, confirming $A_1=A_2=0$.

We can count the [low-weight coefficients of a binary Hamming code](../../../../../low-weight-coefficients-of-a-binary-hamming-code.md) directly. For weight three, choose ordered distinct nonzero columns $a,b$ in $n(n-1)$ ways. The third must be $a+b$, which is nonzero and different from both. Every unordered [support of a vector](../../../../../support-of-a-vector.md) has $3!$ orderings, so $A_3=n(n-1)/3!$.

For weight four, the first two columns $a,b$ are again distinct and nonzero. The third $c$ must avoid $a,b,a+b$, giving $n-3$ possibilities. The fourth is $d=a+b+c$; it is nonzero because $c\ne a+b$, and cannot equal any of the first three because those are distinct. Conversely every ordered zero-sum four-tuple arises in this way. Dividing by $4!$ gives $A_4=n(n-1)(n-3)/4!$.

For weight five, the first three columns $a,b,c$ must be linearly independent. If $a+b+c=0$, the sum condition would force the fourth and fifth to coincide. Thus there are $n(n-1)(n-3)$ choices for the first three. Put $t=a+b+c$. The fourth column $d$ must avoid all seven nonzero [vectors](../../../../../vector.md) of their [linear span](../../../../../linear-span.md): $a,b,c$ would repeat a column; $t$ would force the fifth column to be zero; and $a+b,a+c,b+c$ would force the fifth column to be $c,b,a$, respectively. Conversely, if $d$ avoids these seven [vectors](../../../../../vector.md), $e=t+d$ is nonzero and distinct from $a,b,c,d$. This gives $n-7$ choices for $d$ and determines $e$. Dividing by $5!$ yields

$$
\boxed{A_3=\frac{n(n-1)}{3!},\qquad A_4=\frac{n(n-1)(n-3)}{4!},\qquad A_5=\frac{n(n-1)(n-3)(n-7)}{5!}.}
$$

At $\ell=3$, the last count is zero, as the argument also shows.

The [dual code](../../../../../dual-code.md) $C_{H,\ell}^{\perp}$ is the [row space](../../../../../row-space.md) of $H$, so its [codewords](../../../../../codeword.md) are $aH$ for $a\in\mathbb F_2^\ell$. For nonzero $a$, the [linear functional](../../../../../linear-functional.md) $v\mapsto a\cdot v$ takes value one on exactly half the $2^\ell$ [vectors](../../../../../vector.md) of $V$, by the same translation-pairing argument used above. Removing the zero [vector](../../../../../vector.md) removes only a zero value, so the [Hamming weight](../../../../../hamming-weight.md) is still $m=2^{\ell-1}$. Since $H$ has [matrix rank](../../../../../matrix-rank.md) $\ell$, distinct $a$ give distinct [codewords](../../../../../codeword.md). This proves the [constant weight of a binary simplex code](../../../../../constant-weight-of-a-binary-simplex-code.md) and its full distribution:

$$
\boxed{A_0^{\perp}=1,\qquad A_m^{\perp}=2^\ell-1=n,\qquad A_s^{\perp}=0\ (s\ne0,m).}
$$

In particular, the ordinary [weight enumerator](../../../../../weight-enumerator.md) of the [binary simplex code](../../../../../binary-simplex-code.md) is $1+nz^m$.

Apply the [MacWilliams identity](../../../../../macwilliams-identity.md) to this [dual code](../../../../../dual-code.md), whose size is $2^\ell=n+1$. For $W_C(z)=\sum_sA_sz^s$, the result is

$$
W_{C_{H,\ell}}(z)=\frac{(1+z)^n+n(1-z)^m(1+z)^{n-m}}{n+1}.
$$

The coefficient of $z^s$ in the second product is a value of the binary [Kravchuk polynomials](../../../../../kravchuk-polynomials.md)

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

The unique length-$n$ binary word of weight $n$ is the all-ones word, exactly as proved by the [parity-check matrix](../../../../../parity-check-matrix.md) calculation.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
