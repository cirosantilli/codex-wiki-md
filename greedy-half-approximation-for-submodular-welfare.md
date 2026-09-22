# Greedy half-approximation for submodular welfare

↑ **Parent:** [Winner determination problem](winner-determination-problem.md)

Allocate each remaining item to a bidder with greatest current marginal gain. For nonnegative monotone [submodular set functions](submodular-set-function.md), this uses $O(mn^2)$ value queries and achieves the displayed guarantee. To prove it by induction, let the first allocation give item $j$ to bidder $r$, and set $w=v_r(\{j\})$. Contract that item into bidder $r$'s value by replacing it with $v'_r(S)=v_r(S\cup\{j\})-w$ and leave the other bidders' values unchanged. The remaining greedy run is identical, and $A(v)=w+A(v')$. Move $j$ from its owner in an optimal allocation to $r$. [Submodularity](submodular-set-function.md) bounds the owner's loss by its initial singleton marginal, which is no larger than the selected greedy marginal and hence no larger than $w$. The receiver's value cannot decrease, so $\operatorname{Opt}(v')\geq\operatorname{Opt}(v)-2w$. Induction proves the guarantee, with the zero-item case immediate even for nonzero empty-bundle values.

## ↑ Ancestors (6)

1. [Winner determination problem](winner-determination-problem.md)
2. [Integer programming](integer-programming.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-35/4/b/solution.md)
