<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the [shortest path](../../../../../shortest-path.md) distances in the directed dependency [graph](../../../../../graph-split.md) to define

$$
\boxed{
h_2(R)=
\begin{cases}
0,&R=\varnothing,\\
\max\bigl\{|R|,\ 1+\max_{\neg p\in R}d_G(p)\bigr\},&R\ne\varnothing.
\end{cases}}
$$

The additional $1$ counts the final use of a positive unit [Horn clause](../../../../../horn-clause.md), which corresponds to a fact rather than an [edge](../../../../../edge-of-a-graph.md) of $G$.

To justify the new lower bound, consider any complete proof from $R$ and fix $\neg p\in R$. At some step this obligation must be removed using a [Horn clause](../../../../../horn-clause.md) with head $p$. If that [Horn clause](../../../../../horn-clause.md) is the fact $\{p\}$, we have already found a dependency [graph path](../../../../../path-in-a-graph.md) of length zero ending at a fact. Otherwise select one negative body [Boolean literal](../../../../../boolean-literal.md) $\neg q$. Immediately after the step it belongs to the query, whether newly inserted or merged with an existing obligation. It must subsequently be removed. Record the [edge](../../../../../edge-of-a-graph.md) $p\to q$ and repeat this argument at its later removal.

The selected removal times strictly increase. Since the proof is finite and ends with no obligations, this chain eventually uses a fact. A proof of $\ell$ actions therefore produces a dependency walk of at most $\ell-1$ [edges](../../../../../edge-of-a-graph.md) from $p$ to a fact. Removing any cycles from that walk gives $d_G(p)\le\ell-1$. Hence $1+d_G(p)\le\ell$ for every initial obligation. If $d_G(p)=\infty$, no such proof exists. Combining this bound with the [admissible heuristic](../../../../../admissible-heuristic.md) $|R|$ by taking their maximum preserves admissibility.

For a strict improvement, use

$$
T=\bigl\{\{p,\neg q\},\{q,\neg r\},\{r\}\bigr\},\qquad R=\{\neg p\}.
$$

Here $d_G(p)=2$, so $h_1(R)=1$ while $h_2(R)=3$. The three successive obligations are $\neg p,\neg q,\neg r$, followed by the empty query, so the improved bound is exact.

Do not sum all the values $1+d_G(p)$ without an additional argument: different obligations may share work. For example, with $T=\{\{p,\neg r\},\{q,\neg r\},\{r\}\}$, the query $\{\neg p,\neg q\}$ takes three actions, while that sum would be four.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Intelligent systems](../../../intelligent-systems-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
