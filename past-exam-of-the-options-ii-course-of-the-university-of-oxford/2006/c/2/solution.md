<h1 id="c/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [primitive root](../../../../primitive-root-modulo-n.md) modulo $p$ is an [integer](../../../../integer-split.md) whose residue generates the multiplicative group $\mathbb F_p^\times$, equivalently has order $p-1$.

The [Chinese remainder theorem](../../../../chinese-remainder-theorem.md) states that, for pairwise coprime positive [integers](../../../../integer-split.md) $m_1,\ldots,m_r$, the system $x\equiv a_i\pmod{m_i}$ has a unique solution modulo $M=\prod_i m_i$. For a constructive proof put $M_i=M/m_i$. Bézout's identity gives an [integer](../../../../integer-split.md) $u_i$ with $M_i u_i\equiv1\pmod{m_i}$. Then $x=\sum_i a_iM_i u_i$ has all the required residues. If two solutions exist, their difference is divisible by every $m_i$; pairwise [coprimality](../../../../coprime-integers.md) makes it divisible by their product, proving uniqueness modulo $M$.

Here $3,5,7$ divide $p-1$, and none is zero modulo $p$. Choose a [primitive root](../../../../primitive-root-modulo-n.md) $g$ and exponents $a,b,c$ with

$$
3\equiv g^a,\qquad5\equiv g^b,\qquad7\equiv g^c\pmod p.
$$

Use the theorem with moduli $3,5,7$ to choose $r$ such that $r\equiv a\pmod3$, $r\equiv b\pmod5$, $r\equiv c\pmod7$. Define nonzero residues

$$
n=g^r,\qquad x=g^{(r-a)/3},\qquad
y=g^{(r-b)/5},\qquad z=g^{(r-c)/7}.
$$

The exponents are [integers](../../../../integer-split.md); negative ones are interpreted using inverses in $\mathbb F_p^\times$. Taking [integer](../../../../integer-split.md) representatives now gives

$$
\boxed{p\nmid n,\qquad n\equiv3x^3\equiv5y^5\equiv7z^7\pmod p.}
$$

The theorem aligns the exponent [modular congruences](../../../../modular-congruence.md), which is why a [primitive root](../../../../primitive-root-modulo-n.md) converts the three power conditions into a linear [modular congruence](../../../../modular-congruence.md) problem.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [C](../../c.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
