# Asymmetric Dirichlet hyperbola split

↑ **Parent:** [Dirichlet hyperbola method](dirichlet-hyperbola-method.md)

A balanced [Dirichlet hyperbola method](dirichlet-hyperbola-method.md) split takes real thresholds $A=B=\sqrt N$. An asymmetric split takes $1\le A\le N$ and $B=N/A$. Every [lattice point](lattice-point.md) with $ab\le N$ then has $a\le A$ or $b\le B$, and every point in their overlap rectangle is allowed because $AB=N$. For [arithmetic functions](arithmetic-function.md) $f,g$, define their [partial sums](partial-sum.md) by $F(t)=\sum_{a\le t}f(a)$ and $G(t)=\sum_{b\le t}g(b)$, always over [positive integers](positive-integer.md). The same [inclusion-exclusion principle](inclusion-exclusion-principle.md), now with weight $f(a)g(b)$, yields

$$
\sum_{n\le N}(f*g)(n)
=\sum_{a\le A}f(a)G(N/a)
+\sum_{b\le B}g(b)F(N/b)-F(A)G(B),
\qquad AB=N.
$$

No [multiplicativity](multiplicativity-of-an-arithmetic-function.md) assumption is needed: this is a finite rearrangement of [Dirichlet convolution](dirichlet-convolution.md). The [constant-one arithmetic function](constant-one-arithmetic-function.md) in both positions recovers the [divisor summatory function](divisor-summatory-function.md). For $N=12$, $A=2$, $B=6$ gives

$$
D(12)=(12+6)+(12+6+4+3+2+2)-2\cdot6=18+29-12=35.
$$

It uses two columns and six rows, with a twelve-point overlap.

For general positive real thresholds, **$AB\ge N$ is sufficient for coverage**, since $a>A$ and $b>B$ would imply $ab>AB\ge N$. If $AB>N$, however, the overlap can include points above the [hyperbola](hyperbola.md). The correct subtraction is then $\sum_{a\le A,\ b\le B,\ ab\le N}f(a)g(b)$; the product $F(A)G(B)$ is justified only when the whole integer rectangle lies below it. For example, $N=12$, $A=B=4$ covers every allowed pair, but its rectangle contains the forbidden pair $(4,4)$, so subtracting all sixteen points would give $34$ instead of $35$.

Conversely, the balanced integer thresholds $r,r$ have $r^2\le N$ and still cover every allowed pair because $(r+1)^2>N$. More generally, positive integer thresholds $U,V$ give coverage exactly when $(U+1)(V+1)>N$, and their overlap is a full rectangle exactly when $UV\le N$. These discrete conditions explain why the square-root identity works even when $r^2<N$.

## ↑ Ancestors (7)

1. [Dirichlet hyperbola method](dirichlet-hyperbola-method.md)
2. [Dirichlet convolution](dirichlet-convolution.md)
3. [Arithmetic function](arithmetic-function.md)
4. [Number theory](number-theory-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
