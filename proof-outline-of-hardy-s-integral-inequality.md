<h1 id="proof-outline-of-hardy-s-integral-inequality">Proof outline of Hardy's integral inequality</h1>

↑ **Parent:** [Hardy's integral inequality](hardy-s-integral-inequality.md)

For a nonnegative $f$, first set $g_n(x)=\min(f(x),n)\mathbf1_{(1/n,n)}(x)$ and $F_n(x)=\int_0^xg_n(t)\,dt$. These bounded [functions](function-split.md) vanish near zero and have [compact support](compact-support.md). Their averages have finite [Lp norms](lp-norm.md): they vanish near zero and decay as $1/x$ beyond $n$. [Integration by parts](integration-by-parts.md) gives

$$
I_n:=\int_0^\infty(F_n(x)/x)^p\,dx=\frac{p}{p-1}\int_0^\infty(F_n(x)/x)^{p-1}g_n(x)\,dx\leq\frac{p}{p-1}I_n^{(p-1)/p}\|g_n\|_p.
$$

The boundary term $x^{1-p}F_n(x)^p$ vanishes at zero because $F_n$ is zero there, and at infinity because $F_n$ is eventually constant and $p>1$. The inequality is [Hölder's inequality](holder-s-inequality.md) with [conjugate exponents](conjugate-exponents.md) $p$ and $p/(p-1)$. Divide when $I_n>0$; the zero case is immediate. Since $g_n\uparrow f$ and $Hg_n\uparrow Hf$, the [monotone convergence theorem](monotone-convergence-theorem.md) proves the full bound without presupposing that $Hf$ has finite [Lp norm](lp-norm.md). Apply it to $|f|$ for the signed or complex case.[Inequalities, second edition, §9.8(ii), truncation and integration by parts, printed pp. 242–243](inequalities-by-godfrey-harold-hardy-and-others.md)

## ↑ Ancestors (7)

1. [Hardy's integral inequality](hardy-s-integral-inequality.md)
2. [Hardy's inequality](hardy-s-inequality.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
