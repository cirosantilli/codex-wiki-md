<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set $L=\sqrt D$, and restrict attention to the set $\mathcal S$ of [squarefree integers](../../../../../../squarefree-integer.md) $d\leq L$ all of whose [prime factors](../../../../../../prime-factor.md) lie in $\mathcal P$. Coefficients indexed by non-[squarefree integers](../../../../../../squarefree-integer.md) do not affect $\Sigma$, so they may be set to zero. Put

$$
h(t)=\prod_{p\mid t}(g(p)^{-1}-1),\qquad
k(t)=h(t)^{-1}=\prod_{p\mid t}\frac{g(p)}{1-g(p)},\qquad J=\sum_{t\in\mathcal S}k(t).
$$

In particular, the normalizing [sum](../../../../../../sum.md) runs to **$\sqrt D$**, as in the PDF; the converted TeX's $\sqrt d$ is a transcription error. Define $y_t=\sum_{\substack{m\in\mathcal S\\t\mid m}}g(m)\rho_m$. The finite multiples version of [Möbius inversion](../../../../../../mobius-inversion-formula.md) is

$$
g(d)\rho_d=\sum_{\substack{t\in\mathcal S\\d\mid t}}\mu(t/d)y_t.
$$

It follows by substituting the definition and using $\sum_{r\mid m/d}\mu(r)=1_{m=d}$. Taking $d=1$ gives $1=\sum_t\mu(t)y_t$. Thus the [Selberg sieve diagonalization](../../../../../../selberg-sieve-diagonalization.md) and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) give

$$
1\leq\left(\sum_{t\in\mathcal S}h(t)y_t^2\right)\left(\sum_{t\in\mathcal S}\frac{\mu(t)^2}{h(t)}\right)=\Sigma J.
$$

Equality holds at $y_t=\mu(t)/(Jh(t))$, which satisfies the constraint. Inverting, and writing $t=dv$, yields

$$
\boxed{\rho_d=\frac{\mu(d)}{J}\prod_{p\mid d}\frac1{1-g(p)}
\sum_{\substack{v\leq L/d\\v\text{ squarefree}\\(v,d)=1\\p\mid v\Rightarrow p\in\mathcal P}}\prod_{p\mid v}\frac{g(p)}{1-g(p)}.}
$$

For $d\notin\mathcal S$ set $\rho_d=0$. The formula has $\rho_1=1$ and gives **minimum $\Sigma=1/J$**.

To show these [optimal Selberg weights have modulus at most one](../../../../../../optimal-selberg-weights-have-modulus-at-most-one.md), fix $d\in\mathcal S$. Each integer $ev$, with $e\mid d$, $(v,d)=1$ and $v\leq L/d$, is a distinct term of $\mathcal S$. The total weight of these terms is

$$
\sum_{e\mid d}k(e)\sum_v k(v)=\prod_{p\mid d}(1-g(p))^{-1}\sum_v k(v).
$$

It is at most $J$, so the displayed formula gives $|\rho_d|\leq1$. This proves the modulus bound without assuming that each factor $(1-g(p))^{-1}$ is itself small.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
