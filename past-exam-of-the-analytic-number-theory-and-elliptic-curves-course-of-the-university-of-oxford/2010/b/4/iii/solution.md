<h1 id="b/4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The constant and linear Taylor terms cancel in the Newton step, leaving

$$
|f(a_{i+1})|\le|h_i|^2=d^2q_i^2,\qquad
q_{i+1}\le q_i^2\le q_0^{2^{i+1}}.
$$

Thus residuals strictly decrease whenever the current residual is nonzero, and the steps tend to [zero](../../../../../zero-of-a-function.md) doubly exponentially. By the [ultrametric inequality](../../../../../ultrametric-inequality.md), the distance between any two sufficiently late iterates is bounded by the largest intervening step. The sequence is Cauchy and converges in the complete [valuation ring](../../../../../valuation-ring.md) to $a$. Continuity gives $f(a)=0$, and

$$
\boxed{|a-a_0|\le dq_0=\frac{|f(a_0)|}{|f'(a_0)|}.}
$$

The literal infinite chain of strict inequalities needs the root-hit exception: if $f(a_0)=0$, or a later iterate is already a root, it cannot keep strictly decreasing below [zero](../../../../../zero-of-a-function.md). The construction is eventually constant in that case; all existence and distance conclusions remain valid.

For the equality case, suppose $|f(a_0)|=d^2$ with $0<d<1$. The first Newton step has norm $|h_0|=d$. Write the [Taylor coefficient](../../../../../taylor-coefficient.md) of $h^2$ as $c_2(a_0)=f''(a_0)/2$. Its norm is strictly below one by hypothesis; all higher coefficients have norm at most one. Hence

$$
|f(a_0+h_0)|\le\max(|c_2(a_0)|d^2,d^3)<d^2.
$$

The [derivative](../../../../../derivative.md) changes by $2c_2(a_0)h_0+O(h_0^2)$, of norm strictly below $d$, so it still has norm $d$. The strict Hensel argument applies from this first iterate onward, and the root remains within distance $d=|f(a_0)|/d$ of $a_0$. If characteristic two is admitted, interpret the displayed half-second-[derivative](../../../../../derivative.md) as the second [Taylor coefficient](../../../../../taylor-coefficient.md) $\sum_j\binom j2c_jb^{j-2}$; this is the division-free form of the required hypothesis.

For the final local equation put $F(t)=t^3+3t$. Its values modulo nine are $0,4,5$, so the sum of two such values is confined to $0,1,4,5,8$. Conversely choose initial pairs for these five classes as

$$
(0,0),\quad(-1,-1),\quad(1,0),\quad(-1,0),\quad(1,1),
$$

respectively. Fix the second coordinate $y_0$ and apply the equality-case Hensel result to $g(X)=F(X)+F(y_0)-n$ at the first coordinate $x_0$. Its residual is divisible by nine, $g'(x_0)=3(x_0^2+1)$ has 3-adic norm $1/3$, and $g''(b)/2=3b$ has norm below one for every $b\in\mathbb Z_3$. The strict or equality case therefore supplies a root in $\mathbb Z_3$. Thus

$$
\boxed{n\equiv0,1,4,5,8\pmod9}
$$

is the necessary and sufficient condition.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../split.md)
6. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
