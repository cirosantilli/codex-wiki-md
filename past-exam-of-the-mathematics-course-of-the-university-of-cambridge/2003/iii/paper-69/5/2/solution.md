<h1 id="5/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Order the [interpolation nodes](../../../../../../interpolation-node.md) as $t_0<\cdots<t_n$, as required by their alternating nodal data. Write $w(x)=\prod_{j=0}^n(x-t_j)$ and $\ell_i(x)=w(x)/[(x-t_i)w'(t_i)]$ for the [Lagrange cardinal polynomials](../../../../../../lagrange-cardinal-polynomial.md). Differentiating [Lagrange interpolation](../../../../../../lagrange-polynomial.md) gives

$$
p^{(k)}(x)=\sum_{i=0}^np(t_i)\ell_i^{(k)}(x),\qquad M_k(x)=\sum_{i=0}^n|\ell_i^{(k)}(x)|.
$$

The upper bound is the [triangle inequality](../../../../../../triangle-inequality.md); equality follows by choosing each independent nodal value to be the sign of its weight. Thus this is the [nodal derivative norm from Lagrange cardinal polynomials](../../../../../../nodal-derivative-norm-from-lagrange-cardinal-polynomials.md).

To identify the maximizing signs, put $P_i=w/(x-t_i)$, a [monic polynomial](../../../../../../monic-polynomial.md) of degree $n$. Since $\operatorname{sign}w'(t_i)=(-1)^{n-i}$,

$$
(-1)^i\ell_i^{(k)}(x)=\frac{(-1)^nP_i^{(k)}(x)}{|w'(t_i)|}.
$$

For $0\le k<n$, let $\xi_{i,j}$ be the ordered roots of $P_i^{(k)}$, $1\le j\le n-k$. The roots of $P_i$ decrease componentwise as $i$ increases: deleting a later node replaces one retained node by an earlier one. The [monotonicity of polynomial critical points in their roots](../../../../../../monotonicity-of-polynomial-critical-points-in-their-roots.md), iterated $k$ times, therefore gives $\xi_{n,j}\le\cdots\le\xi_{0,j}$. Moreover, $P_n$ and $P_0$ weakly interlace, so the [Markov interlacing lemma](../../../../../../markov-interlacing-lemma.md) gives $\xi_{0,j}\le\xi_{n,j+1}$. Together,

$$
\xi_{n,j}\le\xi_{n-1,j}\le\cdots\le\xi_{0,j}\le\xi_{n,j+1}.
$$

These root bands have disjoint interiors. At a fixed $x$, all but at most one band lie wholly on one side of $x$. In the possible remaining band, $\xi_{i,j}$ moves monotonically as $i$ increases. Since the [leading coefficients](../../../../../../leading-coefficient-of-a-polynomial.md) of all $P_i^{(k)}$ are positive, the sequence $P_i^{(k)}(x)$ has at most one sign change after zero entries are ignored. The same holds for $(-1)^i\ell_i^{(k)}(x)$. If $k=n$, every $P_i^{(n)}=n!>0$, so the conclusion also holds.

The maximizing nodal signs can consequently be chosen as $\pm(-1)^i$ throughout, or as $\pm(-1)^i$ before one index $s$ and $\mp(-1)^i$ from that index onward. Zero weights can be assigned either sign to complete such a pattern. These are precisely the nodal values of $\pm p^*$ or $\pm q_s$, proving

$$
\boxed{M_k(x)=|p^{*\,(k)}(x)|\quad\text{or}\quad M_k(x)=|q_s^{(k)}(x)|\text{ for some }1\le s\le n}.
$$

The argument works for all real $x$, hence in particular for $[-1,1]$. For $k>n$ every derivative vanishes and the result is immediate.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [5](../../5.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
