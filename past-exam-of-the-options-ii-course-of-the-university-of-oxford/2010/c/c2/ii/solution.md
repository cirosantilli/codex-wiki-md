<h1 id="c/c2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $n\geq1$, the zero [residue](../../../../../residue.md) contributes zero. Write $S=\sum_{x\in\mathbb F_p^\times}x^n$. Multiplication by any nonzero $\alpha$ permutes these residues, so $S=\alpha^nS$ in $\mathbb F_p$. If $(p-1)\nmid n$, choose a [primitive root](../../../../../primitive-root-modulo-n.md) $g$; then $g^n\neq1$, and $(1-g^n)S=0$ forces $S=0$.

If $(p-1)\mid n$, every nonzero $x$ has $x^n=1$, so $S=p-1\equiv-1\pmod p$. Therefore

$$
\boxed{\sum_{x=1}^p x^n\equiv
\begin{cases}0,&(p-1)\nmid n,\\-1,&(p-1)\mid n\end{cases}\pmod p\quad(n\geq1).}
$$

The source also lists $n=0$, although its premise assumes $n\geq1$. For that separate case, the [integer](../../../../../integer-split.md) sum has $p$ terms each equal to one, so it is zero modulo $p$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C2](../../c2.md)
3. [C](../../../c.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
