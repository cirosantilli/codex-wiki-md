<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take $Y(p)=p\to q$ and put $\top=(\bot\to\bot)$, $H=Y(\top)$ and $F_0=Y(\Box H)=\Box H\to q$. The first supplied substitution identity reads

$$
\mathrm{GL}\vdash\Box H\leftrightarrow\Box Y(\Box H)=\Box F_0.
$$

Use the supplied replacement of equivalents in the context $D(p)=p\to q$. It gives

$$
\mathrm{GL}\vdash F_0\leftrightarrow(\Box F_0\to q).
$$

But $H=(\top\to q)$ is equivalent to $q$. Replacement under a box gives $\Box H\leftrightarrow\Box q$, so $F_0$ is equivalent to

$$
\boxed{F=(\Box q\to q).}
$$

Replacing equivalents once more transfers the fixed-point equation to $F$, proving $\mathrm{GL}\vdash F\leftrightarrow(\Box F\to q)$.

A direct check of this [GL fixed point for a provability implication](../../../../gl-fixed-point-for-a-provability-implication.md) is useful: the Löb axiom gives $\Box F\to\Box q$, and necessitating the [tautology](../../../../tautology.md) $q\to F$ gives $\Box q\to\Box F$ by $\mathrm K$. Thus $\Box F\leftrightarrow\Box q$, and replacing the antecedent in $\Box F\to q$ recovers $F$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the Gödel's incompleteness theorems course of the University of Oxford](../../../split.md)
5. [Gödel's incompleteness theorems course of the University of Oxford](../../../../godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
