# Independent-set bound for biregular graphs

↑ **Parent:** [Biregular graph](biregular-graph.md)

For a [biregular graph](biregular-graph.md) with $m$ left vertices of degree $r$ and $n$ right vertices of degree $s$, let $X$ be the indicator vector of a uniformly selected [independent set](independent-set-graph-theory.md). Use base-two [information entropy](information-entropy.md). [Shearer inequality](shearer-s-inequality.md) gives $H(X_U)\leq r^{-1}\sum_{w\in W}H(X_{N(w)})$. Conditional on $X_U$, each right vertex with an empty selected neighbourhood is an independent fair binary choice, and the other right vertices are forbidden. Writing $q_w=\mathbb P(X_{N(w)}=0)$ gives $H(X)\leq r^{-1}\sum_w[H(X_{N(w)})+rq_w]$. For the $2^s$ neighbourhood patterns, assign weight $2^r$ to the zero pattern and weight one to all others. [Jensen's inequality](jensen-s-inequality.md) implies $H(Y)+rq_w\leq\log_2(2^r+2^s-1)$. Since $n/r=m/s$, the bound follows from $H(X)=\log_2i(G)$. If $s$ divides $m$, the disjoint union of $m/s$ copies of the [complete bipartite graph](complete-bipartite-graph.md) $K_{s,r}$ attains equality: each component has $2^s+2^r-1$ [independent sets](independent-set-graph-theory.md).

## ↑ Ancestors (7)

1. [Biregular graph](biregular-graph.md)
2. [Bipartite graph](bipartite-graph.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-12/4/i/solution.md)
