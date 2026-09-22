<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The unconstrained cases can be treated as [don't-care conditions](../../../../../don-t-care-term.md) during [Boolean function](../../../../../boolean-function.md) minimization. One particularly small, deliberately asymmetric choice is

$$
\boxed{q^+=ab+cq.}
$$

Use the same two history [D flip-flops](../../../../../d-flip-flop.md) and one output [D flip-flop](../../../../../d-flip-flop.md), with this expression at the output D input. It requires two two-input [AND gates](../../../../../and-gate.md) and one [OR gate](../../../../../or-gate.md).

To verify every required case, first set $q=0$. If zero occurs at least twice among $a,b,c$, then $ab=0$, so $q^+=0$ as required. If all three samples are one, then $ab=1$, so $q^+=1$. The remaining triples have exactly two ones and hence exactly one sample agreeing with the old zero; either output is allowed.

Now set $q=1$. If at least two samples are one, either $c=1$ or $a=b=1$, giving $q^+=1$. If all three samples are zero, both terms vanish, giving $q^+=0$. The remaining triples have exactly one one and are the allowed [don't-care conditions](../../../../../don-t-care-term.md). Thus the expression meets both requirements, including every constant-input triple.

For minimality, consider these required one-entries in $(a,b,c,q)$ order: $1110$, $1101$, $1011$ and $0111$ have no common literal. Therefore a product covering all four would be the constant one, which violates required zero-entries. Also no single-literal product is safe: each of $a,b,c,q$ is one at some required zero-entry, and each complemented literal is one at $0000$. Hence at least two products with at least two [Boolean literals](../../../../../boolean-literal.md) each are needed. The displayed expression attains two products and four literals.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
