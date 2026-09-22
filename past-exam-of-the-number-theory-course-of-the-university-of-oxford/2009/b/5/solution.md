<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

[ideals](../../../../ideal.md) are coprime when $A+B=\mathcal O_K$, equivalently $1=a+b$ for some $a\in A$, $b\in B$. Always $AB\subseteq A\cap B$. If $x\in A\cap B$, then $x=xa+xb\in AB$, giving $\boxed{AB=A\cap B}$ in the coprime case. For nonzero integral [ideals](../../../../ideal.md), the [Chinese remainder theorem](../../../../chinese-remainder-theorem.md) gives $\mathcal O_K/(AB)\cong\mathcal O_K/A\times\mathcal O_K/B$, and taking finite cardinalities yields $\boxed{N(AB)=N(A)N(B)}$.

For a nonzero [prime ideal](../../../../prime-ideal.md), the chain of finite-index inclusions gives

$$
N(P^e)=[\mathcal O_K:P]\prod_{i=1}^{e-1}[P^i:P^{i+1}]=N(P)^e
$$

by the given hypothesis. Distinct nonzero [prime ideals](../../../../prime-ideal.md) are maximal and coprime, as are their positive powers. [Unique factorization of ideals in a number field](../../../../unique-factorization-of-ideals-in-a-number-field.md) therefore gives $N(A)=\prod_PN(P)^{v_P(A)}$. Exponents add under [ideal](../../../../ideal.md) multiplication, proving multiplicativity for arbitrary nonzero integral [ideals](../../../../ideal.md). This is the standard domain of the finite [ideal norm](../../../../ideal-norm.md) used here.

For the [Dedekind factorization theorem](../../../../dedekind-factorization-theorem.md), choose an integral primitive element $\theta$ of $K$ with monic [minimal polynomial of an algebraic element](../../../../minimal-polynomial-of-an-algebraic-element.md) $f\in\mathbb Z[X]$, and assume the rational prime $p$ does not divide the index $[\mathcal O_K:\mathbb Z[\theta]]$. Factor

$$
\bar f=\prod_{i=1}^g\bar f_i^{e_i}
$$

over $\mathbb F_p$, with distinct monic irreducible factors. For [integer](../../../../integer-split.md) [polynomial](../../../../polynomial-split.md) lifts $f_i$, the distinct [prime ideals](../../../../prime-ideal.md) above $p$ are $P_i=(p,f_i(\theta))$, and

$$
\boxed{(p)=\prod_iP_i^{e_i},\quad\mathcal O_K/P_i\cong\mathbb F_p[X]/(\bar f_i),\quad N(P_i)=p^{\deg\bar f_i}.}
$$

Thus the [residue degree](../../../../residue-degree.md) is $\deg\bar f_i$, the [ramification index](../../../../ramification-index.md) is $e_i$, and $\sum_i e_i\deg\bar f_i=[K:\mathbb Q]$. The index restriction is essential to this direct [factorization](../../../../factorization.md) formula.

For $K=\mathbb Q(\sqrt{-2})$, the [ring of integers](../../../../ring-of-integers.md) is $\mathbb Z[\sqrt{-2}]$, so the index is one and the theorem applies to every prime. Modulo two, $X^2+2=X^2$, giving one [prime ideal](../../../../prime-ideal.md) of [ideal norm](../../../../ideal-norm.md) two. For an odd rational prime, a [prime ideal](../../../../prime-ideal.md) has [ideal norm](../../../../ideal-norm.md) $p$ if the [polynomial](../../../../polynomial-split.md) splits, and [ideal norm](../../../../ideal-norm.md) $p^2$ if it is irreducible. In the former case the supplied condition forces $p\equiv1$ or $3\pmod8$; in the latter case every odd square is one modulo eight. Consequently

$$
\boxed{N(P)=2\quad\text{or}\quad N(P)\equiv1,3\pmod8.}
$$

The odd part of any [ideal norm](../../../../ideal-norm.md) is thus one or three modulo eight, because $3^2\equiv1$. Multiplication by a power of two leaves possible residues $1,3$ for exponent zero, $2,6$ for exponent one, $4$ for exponent two, and $0$ for exponent at least three. Hence $\boxed{N(I)\not\equiv5,7\pmod8}$ for every nonzero [integral ideal](../../../../integral-ideal.md).

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the number theory course of the University of Oxford](../../../split.md)
5. [Number theory course of the University of Oxford](../../../../number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
