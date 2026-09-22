<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At fixed entropy, the [total differential](../../../../../total-differential.md) in coordinates $(T,p)$ is $0=S_T|_p\,dT+S_p|_T\,dp$. Dividing by $dT$ along that path gives $S_T|_p=-S_p|_T p_T|_S$. The same argument in coordinates $(T,V)$ gives $S_T|_V=-S_V|_T V_T|_S$. These are the two required intermediate identities.

To prove the final result without cancelling a possibly vanishing thermal-expansion derivative, write $a=S_T|_V$, $b=S_V|_T$, $c=p_T|_V$, $d=p_V|_T$. In a regular thermodynamic region with $a,d\ne0$, fixed pressure gives $V_T|_p=-c/d$, while fixed entropy gives $T_V|_S=-b/a$. The [chain rule](../../../../../chain-rule.md) then gives $S_T|_p=a-bc/d$ and $p_V|_S=d-bc/a$. Both cross-products equal $ad-bc$, proving

$$
\boxed{\left(\frac{\partial S}{\partial T}\right)_p\left(\frac{\partial p}{\partial V}\right)_T=\left(\frac{\partial p}{\partial V}\right)_S\left(\frac{\partial S}{\partial T}\right)_V.}
$$

The [heat-capacity and compressibility ratio identity](../../../../../heat-capacity-and-compressibility-ratio-identity.md) rewrites this as $C_p/C_V=\kappa_T/\kappa_S$: keeping entropy fixed rather than temperature fixed changes the mechanical stiffness by the same factor as the two thermal responses.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [7](../../7.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
