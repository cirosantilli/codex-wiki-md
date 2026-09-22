# Integral basis of a pure quartic field with radicand three modulo four

↑ **Parent:** [Integral basis](integral-basis.md)

For a nonzero squarefree integer $d\equiv3\pmod4$, set $\theta=\sqrt[4]d$. The [power basis](power-basis.md) $1,\theta,\theta^2,\theta^3$ is an [integral basis](integral-basis.md), with [discriminant](discriminant.md) $-256d^3$. The polynomial is Eisenstein at every prime dividing $d$; for $d=-1$, shift $X^4+1$ by one to obtain an Eisenstein polynomial at two. The [discriminant-index formula for an integral lattice](discriminant-index-formula-for-an-integral-lattice.md) restricts any power-basis index prime to $2d$. An Eisenstein prime cannot divide the index: the norm of $r\theta^i/p$ has valuation $i-4<0$ for $p\nmid r$ and $i<4$, while $\theta^4/p$ is integral; multiplying a putative denominator-$p$ integral element successively by powers of $\theta$ forces each numerator coefficient divisible by $p$.

It remains to exclude two. A putative integral element $(a+b\theta+c\theta^2+e\theta^3)/2$ has relative norm to $\mathbb Q(\sqrt d)$ with coefficients

$$
\frac{a^2+dc^2-2dbe}{4},\qquad\frac{2ac-b^2-de^2}{4}.
$$

The quadratic field has [ring of integers](ring-of-integers.md) $\mathbb Z[\sqrt d]$, so both coefficients are integers. The first congruence forces $a,c$ to have the same parity. If they are odd, the second requires $b^2+3e^2\equiv2\pmod4$, impossible. If they are even, the second forces $b,e$ to have the same parity and the first forces $be$ even, so both are even. Thus no nontrivial denominator-two element exists, proving index one.

## ↑ Ancestors (6)

1. [Integral basis](integral-basis.md)
2. [Algebraic number theory](algebraic-number-theory-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
