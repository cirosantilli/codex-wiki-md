# Greedy two-bin scheduling bound

↑ **Parent:** [Two-bin load balancing](two-bin-load-balancing.md)

Put each successive item into a currently lighter bin. Before receiving weight $w_j$, that bin contains at most half the total weight already assigned, hence at most $(s-w_j)/2$, where $s$ is the overall total. Apply this to the last item in a finally heaviest bin to get $\operatorname{ALG}\leq s/2+w_{\max}/2$. Since $\operatorname{OPT}\geq\max(s/2,w_{\max})$, the approximation ratio is at most $3/2$. Ordered weights $1,1,2$ give loads $3,1$ rather than the optimal $2,2$, proving the bound is sharp. Its relative-error guarantee is $\varepsilon=1/2$.

## ↑ Ancestors (6)

1. [Two-bin load balancing](two-bin-load-balancing.md)
2. [Integer programming](integer-programming.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-40/6/b/solution.md)
