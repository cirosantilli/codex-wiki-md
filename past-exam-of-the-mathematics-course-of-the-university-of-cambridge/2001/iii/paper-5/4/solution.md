<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Assume $0\le k\le n$. Let $V=L_{n-1}$ be the $n$-dimensional irreducible [sl2 Lie algebra](../../../../../sl2-lie-algebra.md) representation. Choose a weight basis $v_0,\ldots,v_{n-1}$ with weights $2j-(n-1)$; this lists the usual irreducible weight string in increasing order. Its [exterior power](../../../../../exterior-power.md) $\Lambda^kV$ has basis $v_{j_1}\wedge\cdots\wedge v_{j_k}$ for $0\le j_1<\cdots<j_k<n$, so its [formal character](../../../../../formal-character-of-a-weight-module.md) is

$$
\operatorname{ch}\Lambda^kV
=\sum_{j_1<\cdots<j_k}q^{2(j_1+\cdots+j_k)-k(n-1)}
=q^{-N}\sum_{j_1<\cdots<j_k}(q^2)^{j_1+\cdots+j_k-k(k-1)/2},\quad N=k(n-k).
$$

The last sum is the [Gaussian binomial coefficient](../../../../../gaussian-binomial-coefficient.md) $G_{n,k}(q^2)$. To verify the product identity, splitting the subsets according to whether they contain $n-1$ gives

$$
G_{n,k}(t)=G_{n-1,k}(t)+t^{n-k}G_{n-1,k-1}(t),\qquad G_{n,0}=G_{n,n}=1.
$$

The product $\prod_{j=1}^k(1-t^{n-k+j})/(1-t^j)$ satisfies the same recurrence, after putting both terms over their common denominator. Thus induction identifies it with the subset sum, proving it is a polynomial with nonnegative integer coefficients.

The [quantum integer](../../../../../quantum-integer.md) convention in the PDF has

$$
[m]_q=\frac{q^m-q^{-m}}{q-q^{-1}}=q^{1-m}\frac{1-q^{2m}}{1-q^2}.
$$

Multiplying these factors in the factorial quotient gives

$$
\boxed{\begin{bmatrix}n\\k\end{bmatrix}_q=q^{-N}G_{n,k}(q^2)=\operatorname{ch}\Lambda^kL_{n-1}.}
$$

This establishes the required representation-theoretic interpretation.

By the [Weyl complete reducibility theorem](../../../../../weyl-complete-reducibility-theorem.md), write $\Lambda^kV\cong\bigoplus_{m\ge0}r_mL_m$, where $r_m$ are nonnegative integers. The [classification of finite-dimensional sl2 representations](../../../../../classification-of-finite-dimensional-sl2-representations.md) gives

$$
\operatorname{ch}L_m=q^m+q^{m-2}+\cdots+q^{-m}.
$$

Every exterior-power weight has parity $N$ and lies between $-N$ and $N$. Therefore only $m\le N$ with $m\equiv N\pmod2$ occur. For $j\ge0$ with that parity, the coefficient $c_j$ of $q^j$ is

$$
c_j=\sum_{\substack{m\ge j\\m\equiv N\ (2)}}r_m,\qquad c_j=c_{-j},\qquad c_j-c_{j+2}=r_j\ge0.
$$

The coefficients consequently increase toward the middle of the occupied weight string and decrease afterward. If $G_{n,k}(t)=\sum_{s=0}^N a_st^s$, then $a_s=c_{-N+2s}$. Hence

$$
\boxed{a_0\le a_1\le\cdots\le a_{\lfloor N/2\rfloor},\qquad a_s=a_{N-s}.}
$$

This is the [unimodality of Gaussian binomial coefficients](../../../../../unimodality-of-gaussian-binomial-coefficients.md), proved through [parity unimodality of an sl2 character](../../../../../parity-unimodality-of-an-sl2-character.md). It includes $k=0,n$, when the character is one.

There is a normalization qualification in the printed wording. The symmetric quantum-binomial quotient is a [Laurent polynomial](../../../../../laurent-polynomial.md) in $q$, with exponents spaced by two; the unimodality just proved is for that occupied parity, or equivalently for the ordinary polynomial $G_{n,k}(t)$ after setting $t=q^2$ and removing the monomial shift. If one instead includes every integer exponent of $q$, the literal coefficient claim is false: $\begin{bmatrix}2\\1\end{bmatrix}_q=q+q^{-1}$ has coefficients $1,0,1$. **The representation-theoretic conclusion is unimodality on the parity string, and ordinary unimodality of the Gaussian polynomial.**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
