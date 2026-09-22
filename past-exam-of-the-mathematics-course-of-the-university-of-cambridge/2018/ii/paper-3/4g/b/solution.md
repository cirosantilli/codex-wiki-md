<h1 id="4g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The standard [conversion of a context-free grammar to Chomsky normal form](../../../../../../conversion-of-a-context-free-grammar-to-chomsky-normal-form.md) proceeds as follows:

[ Add](https://ourbigbook.com/-/topic/add) a fresh start symbol $S_0$ with $S_0\to S$.  
[ Find](https://ourbigbook.com/-/topic/find) the nullable nonterminals, add the variants obtained by omitting nullable occurrences, and remove all [epsilon productions](../../../../../../epsilon-production.md). Omit $S_0\to\epsilon$ as well because the requested language excludes $\epsilon$.  
[ Remove](https://ourbigbook.com/-/topic/remove) every [unit production](../../../../../../unit-production.md) $A\to B$ by copying the non-unit productions reachable from $B$ to $A$.  
[ Remove](https://ourbigbook.com/-/topic/remove) nonterminals that are unreachable from $S_0$ or cannot derive a terminal word.  
[ In](https://ourbigbook.com/-/topic/in) every right-hand side of length at least two, replace a terminal $a$ by a fresh nonterminal $T_a$ with $T_a\to a$.  
[ Replace](https://ourbigbook.com/-/topic/replace) each right-hand side of length greater than two by a chain of binary productions using fresh nonterminals.

Each remaining production is of the required binary or terminal form, and these transformations preserve every nonempty generated word. Thus **$\mathcal L(G_{\rm Chom})=\mathcal L(G)\setminus\{\epsilon\}$.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4G](../../4g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
