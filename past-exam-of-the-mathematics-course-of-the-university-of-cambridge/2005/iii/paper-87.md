# Paper 87

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper87.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper87.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 87](paper-87.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Work over the [finite field](../../../algebra.md#finite-field) $\mathbb F_2$, and write $A_i$ for row $i$ of the PDF's $12\times12$ matrix. The first row has [Hamming weight](../../../coding-theory.md#hamming-weight) eleven; all other rows have [Hamming weight](../../../coding-theory.md#hamming-weight) seven. To check their intersections economically, index the last eleven columns modulo eleven. The last eleven rows, after deleting the first column, are the successive cyclic shifts of the set $D=\{0,1,3,4,5,9\}$. Direct calculation gives

$$
\begin{array}{c|ccccc}t&1&2&3&4&5\\\hline D\cap(D+t)&\{1,4,5\}&\{0,3,5\}&\{1,3,4\}&\{4,5,9\}&\{3,5,9\}\end{array}.
$$

The intersection sizes for $-t$ equal those for $t$. Thus two different rows among $A_2,\ldots,A_{12}$ meet in four positions, including their shared first coordinate, whereas $A_1$ meets each of these rows in six positions. All these intersection sizes are [even numbers](../../../number-theory.md#even-number), while each row weight is an [odd number](../../../number-theory.md#odd-number). Consequently $AA^T=I$. The first row and column agree, and the entry of the last eleven-by-eleven block depends only on the sum of its row and column indices modulo eleven, because successive rows are left shifts. Thus $A$ is a [symmetric matrix](../../../linear-algebra.md#symmetric-matrix), so $A^2=I$.

The [generator matrix](../../../coding-theory.md#generator-matrix) $G=(I\mid A)$ has [rank](../../../linear-algebra.md#rank-one-quadratic-form) twelve, and

$$
GG^T=I+AA^T=0.
$$

Hence its [linear code](../../../coding-theory.md#linear-code) $C$ lies in its [dual code](../../../coding-theory.md#dual-code) $C^\perp$. Both have [dimension](../../../vector-space.md#dimension-vector-space) twelve, so $C=C^\perp$: it is a [self-dual code](../../../coding-theory.md#self-dual-code). Moreover $AG=(A\mid A^2)=(A\mid I)$, and $A$ is an [invertible matrix](../../../linear-algebra.md#invertible-matrix), so this is another [generator matrix](../../../coding-theory.md#generator-matrix) for the same code. In the column [parity-check matrix](../../../coding-theory.md#parity-check-matrix) convention of the question,

$$
\boxed{C=C^\perp,\qquad G'=(A\mid I),\qquad H=\begin{pmatrix}I\\A\end{pmatrix},\qquad GH=0.}
$$

The matrix $H$ has [rank](../../../linear-algebra.md#rank-one-quadratic-form) twelve, so its nullspace condition $cH=0$ characterizes $C$ exactly.

To prove the [minimum Hamming distance](../../../coding-theory.md#minimum-distance-of-a-code), first observe that the rows of $G$ have [Hamming weights](../../../coding-theory.md#hamming-weight) twelve and eight. For binary vectors,

$$
\operatorname{wt}(v+w)=\operatorname{wt}(v)+\operatorname{wt}(w)-2|\operatorname{supp}(v)\cap\operatorname{supp}(w)|.
$$

Every partial sum of generator rows is orthogonal to every further generator row, by $GG^T=0$. Its intersection with that row therefore contains an [even number](../../../number-theory.md#even-number) of positions. Induction using this identity proves that every [codeword](../../../coding-theory.md#codeword) has weight divisible by four: $C$ is a [doubly even code](../../../coding-theory.md#doubly-even-code).

The [systematic-matrix proof of extended Golay distance](../../../coding-theory.md#systematic-matrix-proof-of-extended-golay-distance) now excludes weight four. Write a [codeword](../../../coding-theory.md#codeword) as $(u,uA)$ and put $k=\operatorname{wt}(u)$. If its total weight were four, $1\leq k\leq4$. For $k=1$, the right half is a row of $A$ and has weight seven or eleven. For $k=2$, the right half is the sum of two distinct rows; the intersection counts above give weight $11+7-2\cdot6=6$ or $7+7-2\cdot4=6$. For $k=3$, the right half would be a unit vector, but then $u=(uA)A$ would be a row of $A$, of weight seven or eleven. For $k=4$, the right half would vanish, contradicting invertibility of $A$. Thus no nonzero word has weight four. Every nonzero weight is consequently at least eight, and any generator row other than the first attains eight. Since the [minimum Hamming distance of a linear code](../../../coding-theory.md#minimum-hamming-distance-of-a-linear-code) is its least nonzero weight,

$$
\boxed{d(C)=8,\qquad C\text{ has parameters }[24,12,8].}
$$

Define the length-$23$ [binary Golay code](../../../coding-theory.md#binary-golay-code) $C_{23}$ as the [punctured code](../../../coding-theory.md#punctured-code) obtained by deleting the first coordinate of this [extended binary Golay code](../../../coding-theory.md#extended-binary-golay-code). This [puncturing](../../../coding-theory.md#puncturing-coding-theory) is injective on $C$, because a nonzero word in its kernel would have weight one. Thus $\dim C_{23}=12$, and deleting one coordinate gives $d(C_{23})\geq7$. The sum of the first two generator rows has weight eight and first coordinate one, so its puncture has weight seven. Therefore $d(C_{23})=7$. In fact any coordinate can be punctured: every left coordinate except the first occurs in a weight-eight generator row, the first occurs in the sum just used, and every right coordinate occurs in at least one of the weight-eight generator rows.

The radius-three [Hamming balls](../../../coding-theory.md#hamming-ball) around the $2^{12}$ words of $C_{23}$ are disjoint, since two centers in intersecting balls would have [Hamming distance](../../../coding-theory.md#hamming-distance) at most six. Each ball contains

$$
\sum_{j=0}^3\binom{23}{j}=1+23+253+1771=2048=2^{11}
$$

words. Their combined size is $2^{12}2^{11}=2^{23}$, the size of the entire binary [Hamming space](../../../coding-theory.md#hamming-space). Hence

$$
\boxed{C_{23}\text{ is a perfect }[23,12,7]\text{ code, correcting three errors}.}
$$

For decoding in $C$, write the received word as $y=c+(p,q)$, where $(p,q)$ is the unknown error in its two halves. Its [syndrome](../../../coding-theory.md#syndrome) is

$$
s=yH=p+qA,\qquad t=sA=pA+q.
$$

Let $e_i$ denote the length-twelve unit vector. For [bounded-distance decoding](../../../coding-theory.md#bounded-distance-decoding), the [three-error syndrome decoding of extended Golay code](../../../coding-theory.md#three-error-syndrome-decoding-of-extended-golay-code) is the following finite search, returning the first successful candidate error:

- If $\operatorname{wt}(s)\leq3$, return $(s,0)$.
- Otherwise, if some $i$ satisfies $\operatorname{wt}(s+A_i)\leq2$, return $(s+A_i,e_i)$.
- Otherwise, compute $t=sA$; if $\operatorname{wt}(t)\leq3$, return $(0,t)$.
- Otherwise, if some $i$ satisfies $\operatorname{wt}(t+A_i)\leq2$, return $(e_i,t+A_i)$.
- If no test succeeds, declare that no error of weight at most three has this [syndrome](../../../coding-theory.md#syndrome).

Every returned candidate has total [Hamming weight](../../../coding-theory.md#hamming-weight) at most three and the required [syndrome](../../../coding-theory.md#syndrome). Conversely, an error of total weight at most three has a half of weight zero or one. The tests exhaust respectively $q=0$, $q=e_i$, $p=0$, and $p=e_i$, so they find every such error. Two distinct successful candidates would differ by a nonzero [codeword](../../../coding-theory.md#codeword) of weight at most six, contradicting $d(C)=8$. Thus the result is unique, and the decoded word is $y+(p,q)$. The condition $\operatorname{wt}(s)\geq3$ still allows the first test when the weight is exactly three; for larger syndrome weight begin with the second test. A large syndrome weight alone does not imply more than three errors.

**The decoder corrects every error of weight at most three; failure means that the received word is outside all radius-three decoding balls.** Unlike its puncture, $C$ is not a [perfect code](../../../coding-theory.md#perfect-code): its radius-three balls cover only $2^{12}(1+24+276+2024)=2^{12}\cdot2325<2^{24}$ words. Without the three-error assumption, a successful test identifies a nearby codeword but need not identify the transmitted word.

For an arbitrary received word, a complete [minimum-distance decoding](../../../coding-theory.md#minimum-distance-decoding) fallback is to enumerate $q\in\mathbb F_2^{12}$ and minimize $\operatorname{wt}(s+qA)+\operatorname{wt}(q)$. Every error with the observed [syndrome](../../../coding-theory.md#syndrome) has exactly the form $(s+qA,q)$, so a minimizer gives a nearest [codeword](../../../coding-theory.md#codeword) $y+(s+qA,q)$. Report all minimizers if there is a tie. This also decodes outside the guaranteed radius in the nearest-word sense, while making no unsupported claim that the transmitted word is determined. Thus a syndrome of weight at least three alone is insufficient for guaranteed recovery; either the three-error hypothesis or a choice among nearest words is needed.

## 2

↑ **Parent:** [Paper 87](paper-87.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Represent a word $(c_0,\ldots,c_{n-1})$ in the [Hamming space](../../../coding-theory.md#hamming-space) $H_{n,q}$ by the [polynomial](../../../polynomial.md) $c(x)=\sum_{j=0}^{n-1}c_jx^j$. A [cyclic code](../../../coding-theory.md#cyclic-code) is a [linear code](../../../coding-theory.md#linear-code) invariant under the cyclic coordinate shift $(c_0,\ldots,c_{n-1})\mapsto(c_{n-1},c_0,\ldots,c_{n-2})$. Under this identification the shift is multiplication by $x$ modulo $x^n-1$. A shift-invariant [vector subspace](../../../vector-space.md#vector-subspace) is closed under multiplication by every [polynomial](../../../polynomial.md), since such multiplication is a [linear combination](../../../vector-space.md#linear-combination) of shifts. It is therefore an [ideal](../../../commutative-algebra.md#ideal) of

$$
R=\mathbb F_q[x]/(x^n-1).
$$

Conversely every [ideal](../../../commutative-algebra.md#ideal) of $R$ is a [vector subspace](../../../vector-space.md#vector-subspace) closed under multiplication by $x$, hence a [cyclic code](../../../coding-theory.md#cyclic-code). Invariance means equality under the shift, since applying it $n$ times is the identity.

Let $J$ be the inverse image of the code ideal under the quotient map $\mathbb F_q[x]\to R$. It contains $(x^n-1)$ and is nonzero. Choose a nonzero element of $J$ of smallest degree and scale it to a [monic polynomial](../../../polynomial.md#monic-polynomial) $g$. For any $f\in J$, [polynomial division](../../../polynomial.md#polynomial-division) gives $f=ag+r$ with $\deg r<\deg g$. Since $r=f-ag\in J$, minimality forces $r=0$. Thus $J=(g)$ and in particular

$$
\boxed{g\mid x^n-1,\qquad C=(\overline g)\subseteq R.}
$$

This is the required [generator polynomial of a cyclic code](../../../coding-theory.md#generator-polynomial-of-a-cyclic-code); the divisibility direction in the printed formula is reversed. The quotient-ring modulus is $x^n-1$, with $1$ denoting the multiplicative identity of the [finite field](../../../algebra.md#finite-field). If $r=\deg g$, every codeword has a unique representative $ag$ with $\deg a<n-r$. Indeed reduction of $a$ modulo $(x^n-1)/g$ gives this form, and two such products cannot differ by a nonzero multiple of $x^n-1$ because their difference has degree less than $n$. Therefore

$$
\boxed{\dim C=n-r,\qquad g,xg,\ldots,x^{n-r-1}g\text{ form a basis}.}
$$

For the zero code the convention is $g=x^n-1$ and this [basis](../../../vector-space.md#basis) is empty; for the full word space $g=1$.

The [zeros of a cyclic code](../../../coding-theory.md#zero-of-a-cyclic-code) are the [polynomial roots](../../../polynomial.md#root-of-a-polynomial) of $g$ in a [splitting field](../../../galois-theory.md#splitting-field) $E$ of $x^n-1$. Suppose first that the [characteristic](../../../algebra.md#characteristic-of-a-field) $p$ of $\mathbb F_q$ does not divide $n$. The [formal derivative](../../../galois-theory.md#formal-derivative) of $x^n-1$ is $nx^{n-1}$, which has no common root with $x^n-1$; all roots of $g$ are therefore simple. If they are $\alpha_1,\ldots,\alpha_r$, then $g\mid c$ is equivalent to $c(\alpha_i)=0$ for all $i$. A [root-evaluation parity-check matrix of a cyclic code](../../../coding-theory.md#root-evaluation-parity-check-matrix-of-a-cyclic-code), written with checks as rows, is consequently

$$
H_E=\begin{pmatrix}1&\alpha_1&\cdots&\alpha_1^{n-1}\\\vdots&\vdots&&\vdots\\1&\alpha_r&\cdots&\alpha_r^{n-1}\end{pmatrix},\qquad H_Ec^T=0.
$$

Its entries may lie in $E$, rather than in the original [finite field](../../../algebra.md#finite-field). To obtain a [parity-check matrix](../../../coding-theory.md#parity-check-matrix) over $\mathbb F_q$, choose a [basis](../../../vector-space.md#basis) of $E$ over $\mathbb F_q$ and replace each equation by the equations for all of its field coordinates. The resulting matrix has the same kernel $C$, hence [rank](../../../linear-algebra.md#rank-one-quadratic-form) $r=n-\dim C$; retain any $r$ independent rows. More economically, choose one root from each [Frobenius conjugate](../../../algebra.md#frobenius-conjugate) orbit. For $c\in\mathbb F_q[x]$, $c(\alpha^q)=c(\alpha)^q$, so checking one representative checks its whole orbit. Expanding that representative's equation in a [basis](../../../vector-space.md#basis) of $\mathbb F_q(\alpha)$ gives precisely the number of checks equal to its orbit length.

No coprimality hypothesis is stated in the question, so the [repeated-root cyclic code](../../../coding-theory.md#repeated-root-cyclic-code) case must also be distinguished. Distinct roots alone cannot determine these codes: in $\mathbb F_2[x]/(x^2-1)$, the generators $x+1$ and $(x+1)^2$ have the same zero, but generate codes of [dimensions](../../../vector-space.md#dimension-vector-space) one and zero. In general write $g=\prod_i(x-\alpha_i)^{m_i}$ in $E[x]$. The correct checks are

$$
c^{[\ell]}(\alpha_i)=0\quad(0\leq\ell<m_i),\qquad c^{[\ell]}(x)=\sum_{j\geq\ell}\binom j\ell c_jx^{j-\ell},
$$

using [Hasse derivatives](../../../polynomial.md#hasse-derivative). Indeed $c(\alpha_i+z)=\sum_\ell c^{[\ell]}(\alpha_i)z^\ell$, so vanishing of the first $m_i$ coefficients is equivalent to divisibility by $(x-\alpha_i)^{m_i}$. A [repeated-root parity-check matrix](../../../coding-theory.md#repeated-root-parity-check-matrix) over $E$ thus has rows indexed by $(i,\ell)$ and entries

$$
\boxed{(H_E)_{(i,\ell),j}=\begin{cases}\binom j\ell\alpha_i^{j-\ell},&j\geq\ell,\\0,&j<\ell.\end{cases}}
$$

As before, expand to equations over $\mathbb F_q$ and retain $\deg g=\sum_i m_i$ independent rows. The ordinary root-evaluation matrix is exactly the special case $m_i=1$.

For the binary [Hamming code](../../../coding-theory.md#hamming-code), let $s\geq2$, $n=2^s-1$, and let $\omega$ generate the [multiplicative group of a finite field](../../../algebra.md#multiplicative-group-of-a-finite-field) $\mathbb F_{2^s}^{\times}$. This is possible because that group is a [cyclic group](../../../group.md#cyclic-group). Choose a [basis](../../../vector-space.md#basis) of $\mathbb F_{2^s}$ over $\mathbb F_2$. The coordinate columns of $1,\omega,\ldots,\omega^{n-1}$ then run through every nonzero vector of $\mathbb F_2^s$ exactly once. They are a [parity-check matrix](../../../coding-theory.md#parity-check-matrix) $H$ for a [Hamming code](../../../coding-theory.md#hamming-code), possibly after permuting the columns of a given Hamming matrix. Thus

$$
C=\left\{c\in\mathbb F_2^n:\sum_{j=0}^{n-1}c_j\omega^j=0\right\}=\{c:c(\omega)=0\}
$$

is equivalent to the [Hamming code](../../../coding-theory.md#hamming-code). Multiplication by $x$ modulo $x^n-1$ multiplies its evaluation at $\omega$ by $\omega$, so $C$ is a [cyclic code](../../../coding-theory.md#cyclic-code).

The [parity-check matrix](../../../coding-theory.md#parity-check-matrix) has [rank](../../../linear-algebra.md#rank-one-quadratic-form) $s$ because its columns contain a [basis](../../../vector-space.md#basis). It has no zero column or repeated column, so no nonzero word of weight one or two is in its kernel. Two distinct nonzero columns have a nonzero sum, which is a third distinct column; these three columns give a word of weight three. Hence $C$ has parameters $[2^s-1,2^s-s-1,3]$.

A [polynomial](../../../polynomial.md) over $\mathbb F_2$ vanishes at $\omega$ exactly when it is divisible by its [minimal polynomial of an algebraic element](../../../galois-theory.md#minimal-polynomial-of-an-algebraic-element) $m_\omega$. The [finite-field Frobenius automorphism](../../../algebra.md#finite-field-frobenius-automorphism) gives all conjugates of $\omega$ as $\omega^{2^j}$. Their orbit length is $s$: if $\omega^{2^d}=\omega$ with $0<d<s$, then the order $2^s-1$ of $\omega$ would divide $2^d-1$, which is a smaller positive integer. Therefore the [Hamming code as a cyclic code](../../../coding-theory.md#hamming-code-as-a-cyclic-code) has

$$
\boxed{g(x)=m_\omega(x)=\prod_{j=0}^{s-1}(x-\omega^{2^j}),\qquad\text{zeros }\omega,\omega^2,\omega^{2^2},\ldots,\omega^{2^{s-1}}.}
$$

The last exponent here is $2^{s-1}$. The printed exponent $2^s-1$ would give $\omega^{2^s-1}=1$, which is not a root of the degree-$s$ irreducible [minimal polynomial of an algebraic element](../../../galois-theory.md#minimal-polynomial-of-an-algebraic-element) for $s\geq2$.

## 3

↑ **Parent:** [Paper 87](paper-87.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For distinct evaluation points $a_0,\ldots,a_{n-1}\in\mathbb F_q$ and $1\leq k\leq n$, the [Reed-Solomon code](../../../coding-theory.md#reed-solomon-error-correction) is

$$
\operatorname{RS}_k(a)=\{(f(a_0),\ldots,f(a_{n-1})):\ f\in\mathbb F_q[x],\ \deg f<k\}.
$$

This is a [linear code](../../../coding-theory.md#linear-code) of [dimension](../../../vector-space.md#dimension-vector-space) $k$: evaluation is [linear](../../../vector-space.md#linearity), and a nonzero [polynomial](../../../polynomial.md) of degree less than $k\leq n$ cannot vanish at all $n$ distinct points. The assertion of cyclicity concerns the primitive, unextended construction: set $n=q-1$ and $a_j=\omega^j$, where $\omega$ generates the [multiplicative group of a finite field](../../../algebra.md#multiplicative-group-of-a-finite-field) $\mathbb F_q^\times$. Arbitrary evaluation sets or arbitrary coordinate orders need not make a [Reed-Solomon code](../../../coding-theory.md#reed-solomon-error-correction) a [cyclic code](../../../coding-theory.md#cyclic-code).

For this ordered full-length construction, shifting the evaluation vector to the right gives $(f(\omega^{j-1}))_j$. This is the evaluation vector of $f(\omega^{-1}x)$, whose degree is still less than $k$, so it is a [cyclic code](../../../coding-theory.md#cyclic-code). Its [generator polynomial](../../../coding-theory.md#generator-polynomial-of-a-cyclic-code) follows from the [finite geometric series](../../../real-analysis.md#finite-geometric-series)

$$
\sum_{j=0}^{n-1}\omega^{jt}=\begin{cases}n,&n\mid t,\\0,&n\nmid t.\end{cases}
$$

Here the scalar $n=q-1$ is nonzero in $\mathbb F_q$. Write $f(x)=\sum_{a=0}^{k-1}m_ax^a$ and $c(x)=\sum_{j=0}^{n-1}f(\omega^j)x^j$. For $1\leq\ell\leq n-k$,

$$
c(\omega^\ell)=\sum_{a=0}^{k-1}m_a\sum_{j=0}^{n-1}\omega^{j(a+\ell)}=0,
$$

since $1\leq a+\ell\leq n-1$. Thus every word is divisible by $g(x)=\prod_{\ell=1}^{n-k}(x-\omega^\ell)$. This monic divisor of $x^n-1$ generates a [cyclic code](../../../coding-theory.md#cyclic-code) of [dimension](../../../vector-space.md#dimension-vector-space) $n-(n-k)=k$, equal to the evaluation code by inclusion and dimension. Hence

$$
\boxed{\operatorname{RS}_k(1,\omega,\ldots,\omega^{n-1})=\langle g\rangle,\qquad g(x)=\prod_{\ell=1}^{n-k}(x-\omega^\ell),\quad n=q-1.}
$$

It is useful to allow a starting exponent $b$ for the consecutive [zeros of a cyclic code](../../../coding-theory.md#zero-of-a-cyclic-code). Define the [primitive cyclic Reed-Solomon code](../../../coding-theory.md#primitive-cyclic-reed-solomon-code)

$$
C_{k,b}=\left\langle\prod_{\ell=b}^{b+n-k-1}(x-\omega^\ell)\right\rangle.
$$

All exponents are understood modulo $n$. The same geometric-sum calculation shows that

$$
C_{k,b}=\{(a_j^{1-b}f(a_j))_{j=0}^{n-1}:\deg f<k\}.
$$

Indeed evaluating its word polynomial at $\omega^{b+\ell}$, $0\leq\ell<n-k$, gives sums with exponents $a+1+\ell$ between one and $n-1$. This is a [generalized Reed-Solomon code](../../../coding-theory.md#generalized-reed-solomon-code), with nonzero coordinate multipliers $a_j^{1-b}$; $C_{k,1}$ is the unweighted evaluation code. Directly, a right shift corresponds to replacing $f(x)$ by $\omega^{b-1}f(\omega^{-1}x)$, so these offset codes are also [cyclic codes](../../../coding-theory.md#cyclic-code).

A [maximum distance separable code](../../../coding-theory.md#maximum-distance-separable-code), or [MDS code](../../../coding-theory.md#maximum-distance-separable-code), is a [linear code](../../../coding-theory.md#linear-code) attaining the [Singleton bound](../../../coding-theory.md#singleton-bound), with $d=n-k+1$. To see the bound, deleting any $d-1$ coordinates is injective on a code of [minimum Hamming distance](../../../coding-theory.md#minimum-distance-of-a-code) $d$, since two words with the same puncture would differ in at most $d-1$ positions. Therefore $q^k\leq q^{n-d+1}$ and $d\leq n-k+1$. For a nonzero Reed-Solomon evaluation word, the [polynomial](../../../polynomial.md) has at most $k-1$ distinct [polynomial roots](../../../polynomial.md#root-of-a-polynomial), so at least $n-k+1$ coordinates are nonzero. Nonzero coordinate multipliers do not change these zero positions. This proves $d\geq n-k+1$ for both [Reed-Solomon codes](../../../coding-theory.md#reed-solomon-error-correction) and [generalized Reed-Solomon codes](../../../coding-theory.md#generalized-reed-solomon-code). Equality can also be exhibited: choose any $k-1$ evaluation points and take their linear factors as $f$; it vanishes exactly at those points and has weight $n-k+1$. Thus

$$
\boxed{\operatorname{RS}_k\text{ and }C_{k,b}\text{ have parameters }[n,k,n-k+1]\text{ and are MDS codes}.}
$$

The [duality of primitive cyclic Reed-Solomon codes](../../../coding-theory.md#duality-of-primitive-cyclic-reed-solomon-codes) is especially transparent in the evaluation form. Assume first $1\leq k<n$. A vector of $C_{k,b}$ has coordinates $a_j^{1-b}f(a_j)$, $\deg f<k$; a vector of $C_{n-k,1-b}$ has coordinates $a_j^b h(a_j)$, $\deg h<n-k$. Their standard [dot product](../../../linear-algebra.md#dot-product) is

$$
\sum_{j=0}^{n-1}a_j f(a_j)h(a_j)=0.
$$

Every monomial in $x f(x)h(x)$ has exponent at least one and at most $1+(k-1)+(n-k-1)=n-1$, and every such power sum vanishes. Thus $C_{n-k,1-b}\subseteq C_{k,b}^\perp$. Both sides have [dimension](../../../vector-space.md#dimension-vector-space) $n-k$, giving

$$
\boxed{C_{k,b}^\perp=C_{n-k,1-b},\qquad g^\perp(x)=\prod_{\ell=1-b}^{k-b}(x-\omega^\ell).}
$$

In particular $C_{k,1}^\perp=C_{n-k,0}$ has generator $\prod_{\ell=0}^{k-1}(x-\omega^\ell)$. This agrees with the general [dual of a cyclic code](../../../coding-theory.md#dual-of-a-cyclic-code) rule: invert the roots belonging to the complementary factor $(x^n-1)/g$. The dual is a Reed-Solomon code in the consecutive-zero convention. With the strictly unweighted evaluation definition, its coordinates instead have the form $(a_jh(a_j))_j$, so it is a [generalized Reed-Solomon code](../../../coding-theory.md#generalized-reed-solomon-code); it need not equal the unweighted code of dimension $n-k$ on the same points. This convention distinction is essential. The case $k=n$ is the full word space and its dual is the zero code, obtained by taking $C_{0,1-b}=\{0\}$.

For [code encoding](../../../coding-theory.md#code-encoding), use the [finite-field discrete Fourier transform](../../../numerical-analysis.md#finite-field-discrete-fourier-transform) and its inverse:

$$
\widehat c_\ell=\sum_{j=0}^{n-1}c_j\omega^{j\ell},\qquad c_j=n^{-1}\sum_{\ell=0}^{n-1}\widehat c_\ell\omega^{-j\ell}.
$$

For a message $(m_0,\ldots,m_{k-1})$, put $\widehat c_{b-1-a}=n m_a$ for $0\leq a<k$, and set all other transform coordinates to zero. The [inverse discrete Fourier transform](../../../numerical-analysis.md#inverse-discrete-fourier-transform) returns

$$
\boxed{c_j=a_j^{1-b}\sum_{a=0}^{k-1}m_a a_j^a,\qquad a_j=\omega^j.}
$$

The $n-k$ zero transform coordinates are precisely the root checks defining $C_{k,b}$. This gives non-systematic encoding by evaluation. For [systematic polynomial encoding of a cyclic code](../../../coding-theory.md#systematic-polynomial-encoding-of-a-cyclic-code) with a message [polynomial](../../../polynomial.md) $M$ of degree less than $k$, put $r=n-k$ and calculate the remainder $R(x)$ of $x^rM(x)$ upon division by $g(x)$. Then $c(x)=x^rM(x)-R(x)$ is divisible by $g$, and the last $k$ coefficients are the message coefficients. Both methods use the same [generator polynomial](../../../coding-theory.md#generator-polynomial-of-a-cyclic-code) and the same ordered powers of $\omega$.

For [bounded-distance decoding](../../../coding-theory.md#bounded-distance-decoding), let $y=c+e$, put $r=n-k$, and assume at most $T=\lfloor r/2\rfloor$ symbol errors. The following description uses the [Reed-Solomon key equation](../../../coding-theory.md#reed-solomon-key-equation) and fixes the transform and locator conventions explicitly.


- Compute the [syndromes](../../../coding-theory.md#syndrome) $S_\ell=y(\omega^{b+\ell})=\widehat y_{b+\ell}$ for $0\leq\ell<r$. The corresponding codeword transform values vanish. An error of value $E_i$ at coordinate $j_i$ contributes $E_iX_i^{b+\ell}$, where $X_i=\omega^{j_i}$, so $S_\ell=\sum_iE_iX_i^{b+\ell}$.
- Form $S(z)=\sum_{\ell=0}^{r-1}S_\ell z^\ell$. Use the [Berlekamp-Massey algorithm](../../../coding-theory.md#berlekamp-massey-algorithm), or the polynomial [extended Euclidean algorithm](../../../number-theory.md#extended-euclidean-algorithm) applied to $z^r$ and $S(z)$, to solve $\Lambda S\equiv\Omega\pmod{z^r}$ with $\Lambda(0)=1$, $\deg\Lambda=\nu\leq T$, and $\deg\Omega<\nu$. Choose the minimal-degree locator; zero syndrome gives $\Lambda=1$, $\Omega=0$. The [error locator polynomial](../../../coding-theory.md#error-locator-polynomial) is $\Lambda(z)=\prod_{i=1}^\nu(1-X_i z)$, and $\Omega$ is the [error evaluator polynomial](../../../coding-theory.md#error-evaluator-polynomial).
- Perform a [Chien search](../../../coding-theory.md#chien-search): test $\Lambda(\omega^{-j})$ for $0\leq j<n$. Its $\nu$ distinct zeros identify the erroneous coordinates. A mismatch between the degree and the number of distinct permitted roots is a decoding failure.
- Recover each error value by the [Forney algorithm](../../../coding-theory.md#forney-algorithm), with the present syndrome offset:


$$
\boxed{E_i=-X_i^{1-b}\frac{\Omega(X_i^{-1})}{\Lambda'(X_i^{-1})}.}
$$


- Set $e_{j_i}=E_i$, all other error coordinates to zero, and output $c=y-e$. Verify that all $r$ root checks vanish and that the correction has weight at most $T$. Recover the message from the unconstrained transform coordinates by $m_a=n^{-1}\widehat c_{b-1-a}$, or from the last $k$ coefficients if [systematic encoding](../../../coding-theory.md#systematic-encoding) was used.

The denominator in the [Forney algorithm](../../../coding-theory.md#forney-algorithm) is nonzero for distinct locations. The [minimum-distance error-detection and correction guarantee](../../../coding-theory.md#minimum-distance-error-detection-and-correction-guarantee) gives unique recovery because $d=n-k+1>2T$. If the required locator or a valid correction cannot be found, declare decoding failure. Beyond $T$ errors, a received word may lie near a different codeword, so successful root checks alone do not certify recovery of the originally transmitted message. **The guaranteed correction radius is $\lfloor(n-k)/2\rfloor$ symbol errors.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
