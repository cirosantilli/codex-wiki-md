<h1 id="5/with-transaction-costs/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

On each open half-line the sample objective is a utility of a linear gain: $U(\theta(X-\varepsilon))$ on the positive half-line, and $U(\theta(X+\varepsilon))$ on the negative half-line. On a compact subinterval wholly inside either half-line, the secant domination argument from the frictionless part ii applies verbatim, using finiteness of $G$ at four surrounding points. The [dominated convergence theorem](../../../../../../../dominated-convergence-theorem.md) therefore gives **the derivatives**

$$
\boxed{G'(\theta)=\begin{cases}\mathbb E[(X-\varepsilon)U'(\theta(X-\varepsilon))],&\theta>0,\\\mathbb E[(X+\varepsilon)U'(\theta(X+\varepsilon))],&\theta<0.\end{cases}}
$$

They are continuous on their respective half-lines. Near zero, the same outer secants of the globally concave sample objective bound its one-sided slopes. Dominated convergence consequently gives

$$
G'_+(0)=U'(0)(\mathbb EX-\varepsilon),\qquad G'_-(0)=U'(0)(\mathbb EX+\varepsilon).
$$

Here $\mathbb E|X|<\infty$: the frictionless derivative at zero already proves it, since $U'(0)>0$. Thus zero generally has a transaction-cost kink; when $\varepsilon=0$ the two formulas agree.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [With transaction costs](../../with-transaction-costs.md)
3. [5](../../../5.md)
4. [Paper 43](../../../../paper-43-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
