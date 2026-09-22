<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

We prove [Kantorovich duality theorem](../../../../../kantorovich-duality-theorem.md) here by a positive-functional extension argument; it produces the minimizing [transport plan](../../../../../transport-plan.md) at the same time as equality of the values. Let $Y=X\times X$ and $c(x,y)=d(x,y)$. This is a bounded [continuous function](../../../../../continuous-function.md) because $X$ is a compact [metric space](../../../../../metric-space.md). Write $C(Y)$ for the real [space of continuous functions on a compact space](../../../../../space-of-continuous-functions-on-a-compact-space.md), and let

$$
S=\{s\in C(Y):s(x,y)=f(x)+g(y),\ f,g\in C(X)\}.
$$

On this [vector subspace](../../../../../vector-subspace.md) define $\ell(s)=\int f\,d\mathbf P+\int g\,d\mathbf Q$. It is well-defined: two representations differ by a constant in the first variable and the opposite constant in the second, and both measures have mass one. It is positive, since $s\geq0$ implies $\min f+\min g\geq0$ and hence $\ell(s)\geq0$. Also $\ell(1)=1$.

Define the majorant envelope, which is a [sublinear functional](../../../../../sublinear-function.md):

$$
p(h)=\inf\{\ell(s):s\in S,\ s\geq h\}\qquad(h\in C(Y)).
$$

Constants majorize every $h$, and positivity gives $\min h\leq p(h)\leq\max h$, so this quantity is finite. Taking approximate minimizing majorants proves subadditivity; rescaling majorants proves positive homogeneity. Moreover $p(s)=\ell(s)$ for $s\in S$, and subtracting $s$ from a majorant proves

$$
p(h+s)=p(h)+\ell(s).
$$

The dual value in the question is exactly

$$
m_d=\sup\{\ell(s):s\in S,\ s\leq c\}=-p(-c).
$$

Subadditivity at $c+(-c)=0$ gives $m_d\leq p(c)$.

On $S+\mathbb Rc$, assign the value $\ell(s)+t m_d$ to $s+tc$. If $c\notin S$ the representation is unique. If $c\in S$, then $m_d=\ell(c)$, so the assignment is still well-defined. It is dominated by $p$: for $t\geq0$, use $t m_d\leq t p(c)=p(tc)$; for $t<0$, positive homogeneity gives $p(tc)=(-t)p(-c)=t m_d$. Together with the translation identity, these verify domination in both cases.

The real [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) extends this functional to $T:C(Y)\to\mathbb R$ with $T\leq p$. If $h\geq0$, then $p(-h)\leq\ell(0)=0$, so $T(h)\geq0$. Thus $T$ is a [positive linear functional](../../../../../positive-linear-functional.md), with $T(1)=1$ and $T(c)=m_d$. Positivity also gives $|T(h)|\leq\|h\|_\infty$, so $T$ is continuous. The [Riesz-Markov-Kakutani representation theorem](../../../../../riesz-markov-kakutani-representation-theorem.md) supplies a Borel [probability measure](../../../../../probability-measure.md) $\pi_0$ on the compact space $Y$, satisfying $T(h)=\int_Yh\,d\pi_0$.

For every $f\in C(X)$, its pullback $f(x)$ belongs to $S$, so $\int f(x)\,d\pi_0=\int f\,d\mathbf P$. Likewise $\int g(y)\,d\pi_0=\int g\,d\mathbf Q$. Uniqueness in the [Riesz-Markov-Kakutani representation theorem](../../../../../riesz-markov-kakutani-representation-theorem.md) shows that these are exactly the two [marginal distributions](../../../../../marginal-distribution.md). Finally, every feasible pair $f+g\leq c$ gives a lower bound for the cost of every [transport plan](../../../../../transport-plan.md), by integration. Our constructed plan achieves that bound:

$$
\boxed{\int_{X\times X}d(x,y)\,d\pi_0(x,y)
=m_d=\min_{\pi\text{ with marginals }\mathbf P,\mathbf Q}\int d\,d\pi.}
$$

This [Kantorovich duality by positive extension](../../../../../kantorovich-duality-by-positive-extension.md) establishes the requested existence and equality without assuming an optimal plan in advance.

The metric structure additionally gives the [Kantorovich–Rubinstein theorem](../../../../../kantorovich-rubinstein-theorem.md) formulation. For a feasible pair define $h(x)=\inf_y\{d(x,y)-g(y)\}$. The triangle inequality for $d$ makes $h$ one-[Lipschitz continuous](../../../../../lipschitz-continuity.md), $h\geq f$, and $h(y)\leq-g(y)$. Hence the dual objective is at most $\int h\,d\mathbf P-\int h\,d\mathbf Q$. Conversely $(h,-h)$ is feasible for every one-Lipschitz $h$. Therefore

$$
m_d=\sup_{\operatorname{Lip}(h)\leq1}\left(\int h\,d\mathbf P-\int h\,d\mathbf Q\right).
$$

Normalizing $h(x_0)=0$ for a fixed $x_0$ gives a uniformly bounded equicontinuous family; it is closed and compact in the uniform topology by the [Arzelà-Ascoli theorem](../../../../../arzela-ascoli-theorem.md). The objective is uniformly continuous on this family, so the supremum is attained as well. In particular, $m_d$ is the first [Wasserstein distance](../../../../../wasserstein-distance.md) between the two measures.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
