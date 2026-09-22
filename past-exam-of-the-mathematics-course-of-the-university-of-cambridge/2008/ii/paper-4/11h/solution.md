<h1 id="11h/solution">Solution</h1>

↑ **Parent:** [11H](../11h.md)

Put $\alpha=\sqrt N$ and use conventional convergent indexing starting at zero; the same argument covers all the printed positive indices. The [continued fraction](../../../../../continued-fraction.md) complete quotients satisfy $\alpha_{j+1}=1/(\alpha_j-a_j)$, $a_j=\lfloor\alpha_j\rfloor$. After the first step they exceed one, while their algebraic conjugates lie in $(-1,0)$. Indeed $\alpha_1'=1/(-\sqrt N-a_0)\in(-1,0)$, and if $\alpha_j'\in(-1,0)$ with $a_j\geq1$, then $1/(\alpha_j'-a_j)\in(-1,0)$.

Write $\alpha_{k+1}=(\sqrt N+m)/d$, where $m,d$ are integers and $d>0$. This form follows by rationalization at each step: $m_{j+1}=a_jd_j-m_j$ and $d_{j+1}=(N-m_{j+1}^2)/d_j$, starting from $m_0=0,d_0=1$. The two conjugate inequalities give

$$
d<\sqrt N+m,\qquad m<\sqrt N,
$$

so $d<2\sqrt N$. The standard convergent recursions also give

$$
\sqrt N=\frac{p_k\alpha_{k+1}+p_{k-1}}{q_k\alpha_{k+1}+q_{k-1}},\qquad
|p_kq_{k-1}-q_kp_{k-1}|=1.
$$

Substitute the displayed form of $\alpha_{k+1}$ and compare rational and irrational coefficients. This yields $p_k=mq_k+dq_{k-1}$ and $Nq_k=mp_k+dp_{k-1}$. Therefore the [small norm residues from square-root continued fractions](../../../../../small-norm-residues-from-square-root-continued-fractions.md) obey

$$
p_k^2-Nq_k^2=d(p_kq_{k-1}-q_kp_{k-1}),\qquad
\boxed{|p_k^2-Nq_k^2|=d<2\sqrt N.}
$$

The initial convergent satisfies the same relation with the usual $p_{-1}=1,q_{-1}=0$. This avoids the insufficient estimate obtained by merely replacing the convergent error with $1/q_k^2$.

For [integer factorization](../../../../../integer-factorization.md), choose a [factor base](../../../../../factor-base.md) of small primes for which $N$ is a quadratic residue, together with $-1$ to record negative residues; a prime dividing $N$ already supplies a factor. Test the small nonzero integers $r_k=p_k^2-Nq_k^2$ for being [B-numbers](../../../../../b-smooth-integer.md). Complete factorization over the base records each prime exponent modulo two. Once enough relations are collected, linear algebra over $\mathbb F_2$ can choose a nonempty subcollection whose exponent sum is even, including the sign. Then

$$
\prod r_k=Y^2,\qquad X=\prod p_k,\qquad X^2\equiv Y^2\pmod N.
$$

If $X\not\equiv\pm Y\pmod N$, one of $\gcd(X-Y,N)$ or $\gcd(X+Y,N)$ can yield a nontrivial factor. Relations with a noninvertible $p_k$ may already give a factor through its gcd. The small-residue bound makes smoothness more likely; it does not guarantee that any one dependency gives a nontrivial factor.

## ↑ Ancestors (10)

1. [11H](../11h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
