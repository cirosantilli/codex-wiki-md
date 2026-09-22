<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For $b\geq2$, write a number in hereditary base $b$: express its base-$b$ expansion as $\sum_i b^{e_i}c_i$, with $0<c_i<b$, and recursively expand every exponent $e_i$ in the same base. Let $B_{b,c}(m)$, for $c>b$, be the number obtained by replacing every occurrence of the base $b$ in this hereditary expression by $c$. Coefficients and the symbols for addition and exponentiation are retained.

For a starting number $m$, define its [Goodstein sequence](../../../../../goodstein-sequence.md) by $m_0=m$ and

$$
m_{s+1}=\begin{cases}B_{s+2,s+3}(m_s)-1,&m_s>0,\\0,&m_s=0.\end{cases}
$$

The [Goodstein function](../../../../../goodstein-function.md) is the termination-time [function](../../../../../function-split.md)

$$
\boxed{\mathcal G(m)=\min\{s:m_s=0\}.}
$$

This choice counts transitions from the initial term; a convention counting the initial term as well shifts the answer by one. For example the [sequence](../../../../../sequence.md) starting at $3$ is $3,3,3,2,1,0$, so $\mathcal G(3)=5$. Starting at $4$ gives $4,26,41,60,83,\ldots$, illustrating why descent of the numerical terms is not the termination argument.

Define the [ordinal rank of a Goodstein term](../../../../../ordinal-rank-of-a-goodstein-term.md) $\rho_b(m)$ by replacing the base $b$ in the hereditary expansion by $\omega$, at every exponent depth. The result is in [Cantor normal form](../../../../../cantor-normal-form.md) and lies below $\epsilon_0$, called [epsilon zero](../../../../../epsilon-zero.md), the least nonzero solution of $\omega^\alpha=\alpha$. Finite hereditary expressions have finite nesting depth, so their ranks are bounded by a sufficiently high finite tower of powers of $\omega$.

For a fixed base, $\rho_b$ is strictly increasing. To see this, compare two ordinary base-$b$ expansions at their largest differing exponent. By induction through the hereditary exponent expressions, their exponents have the same ordering after replacing $b$ by $\omega$; [computable Cantor normal form notation](../../../../../computable-cantor-normal-form-notation.md) then uses the same first differing exponent or coefficient. Also

$$
\rho_c(B_{b,c}(m))=\rho_b(m).
$$

Indeed after the base change all coefficients remain below $c$, the recursively changed exponents remain correctly ordered, and replacing the new base by $\omega$ gives exactly the original [ordinal](../../../../../ordinal.md) expression. These facts can be proved together by [structural induction for primitive recursive functions](../../../../../structural-induction-for-primitive-recursive-functions.md) on the hereditary expression.

Consequently, whenever $m_s>0$,

$$
\rho_{s+3}(m_{s+1})=\rho_{s+3}(B_{s+2,s+3}(m_s)-1)<\rho_{s+3}(B_{s+2,s+3}(m_s))=\rho_{s+2}(m_s).
$$

An infinite nonzero [Goodstein sequence](../../../../../goodstein-sequence.md) would give an infinite descending [sequence](../../../../../sequence.md) of [ordinals](../../../../../ordinal.md) below $\epsilon_0$, impossible because [ordinals](../../../../../ordinal.md) are well-ordered. Thus **the [Goodstein function](../../../../../goodstein-function.md) is total**. Its steps are effective finite operations, so simulating the [sequence](../../../../../sequence.md) until zero also proves that it is a [total computable function](../../../../../total-computable-function.md).

The same [ordinal](../../../../../ordinal.md) notation system gives the requested [decidable well-order](../../../../../decidable-well-order.md). Let $D$ consist of canonical finite terms for zero and for expressions

$$
\omega^{\alpha_1}c_1+\cdots+\omega^{\alpha_r}c_r,\qquad \alpha_1>\cdots>\alpha_r,\quad c_i\in\mathbb N\setminus\{0\},
$$

where the exponents are themselves canonical terms. Membership in $D$ is decidable by recursively checking the syntax, positive coefficients and decreasing exponents. Comparison is decidable by recursive [computable Cantor normal form notation](../../../../../computable-cantor-normal-form-notation.md), first of exponents, then coefficients, and then the remaining summands. All recursive calls inspect proper subterms, so the algorithm terminates.

Interpreting these terms as [ordinals](../../../../../ordinal.md) gives every [ordinal](../../../../../ordinal.md) below $\epsilon_0$, uniquely. One way to connect this directly to [hereditary base representations](../../../../../hereditary-base-representation.md) is to choose, for a given finite [ordinal](../../../../../ordinal.md) term, a base larger than every coefficient anywhere in that term. Replacing $\omega$ by that base evaluates it to a [natural number](../../../../../natural-number.md) whose hereditary representation recovers the [ordinal](../../../../../ordinal.md) term. Thus all bases together supply the complete notation system; a single fixed base is not enough.

Choose an effective injective coding of finite terms by [natural numbers](../../../../../natural-number.md), and enumerate the valid codes in increasing numerical order. The resulting [bijection](../../../../../bijection.md) $d:\mathbb N\to D$ is computable: validity is decidable and there are infinitely many finite-ordinal terms. Its inverse is computable by counting valid codes below a given code. Define

$$
n\prec m\quad\Longleftrightarrow\quad d(n)<_{\mathrm{CNF}}d(m).
$$

This is a decidable relation on all of $\mathbb N$. The interpretation into [ordinals](../../../../../ordinal.md) is an [order isomorphism](../../../../../order-isomorphism.md) onto $\epsilon_0$, proving

$$
\boxed{(\mathbb N,\prec)\text{ is a decidable well-order of order type }\epsilon_0.}
$$

Decidability here concerns comparing two notations. Well-foundedness is supplied by their [ordinal](../../../../../ordinal.md) interpretation, the same mathematical descent principle used to prove [Goodstein's theorem](../../../../../goodstein-s-theorem.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
