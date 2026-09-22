<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Set $X=1+T$ and let $\varphi:R\to R$ be the [Frobenius substitution on cyclotomic power series](../../../../../frobenius-substitution-on-cyclotomic-power-series.md), $\varphi(g)(T)=g(X^p-1)$. It is injective: modulo $p$ the substitution is $g(T)\mapsto g(T^p)$, which is injective; if $\varphi(g)=0$, this first gives $g\in pR$, and iterating gives $g\in\bigcap_rp^rR=0$.

We first prove that every [formal power series](../../../../../formal-power-series.md) has a unique expansion

$$
\boxed{f(T)=\sum_{i=0}^{p-1}X^i\varphi(f_i)(T),\qquad f_i\in R.}
$$

Modulo $p$, the ring $\mathbb F_p[[T]]$ is free over $\mathbb F_p[[T^p]]$ with basis $1,T,\ldots,T^{p-1}$: group the coefficients by their exponents modulo $p$. Replacing this basis by $1,X,\ldots,X^{p-1}$ gives an invertible triangular change of basis with diagonal entries one. Lift the resulting coefficients to $R$, subtract their displayed expression from $f$, divide the remainder by $p$ and repeat. The p-adic limits of these corrections give the required $f_i$ because $R$ is p-adically complete. If an expression is zero, reduction modulo $p$ forces all $f_i$ to be divisible by $p$; repetition forces every $f_i$ to vanish. This proves both existence and uniqueness without dividing coefficients by $p$.

Define the [Coleman trace operator](../../../../../coleman-trace-operator.md) by $\psi(f)=f_0$. To verify its averaging formula, work temporarily over $\mathbb Z_p[\mu_p][[T]]$, interpreting the substitutions in the $(\xi-1,T)$-adic topology. The argument $\xi X-1$ is topologically nilpotent there, so substituting into an arbitrary [formal power series](../../../../../formal-power-series.md) is legitimate. Moreover

$$
\varphi(f_i)(\xi X-1)=f_i((\xi X)^p-1)=\varphi(f_i)(T).
$$

The sum of $\xi^i$ over the p-th [roots of unity](../../../../../root-of-unity.md) is $p$ at $i=0$ and zero at $1\le i<p$. Therefore

$$
\frac1p\sum_{\xi\in\mu_p}f(\xi X-1)=\varphi(f_0)=\varphi(\psi(f)).
$$

The right side belongs to $R$, so the apparent denominator causes no integrality problem. Injectivity of $\varphi$ proves that this is **the unique map $\psi$ with the required identity**. The construction also proves $\psi(\varphi(g)f)=g\psi(f)$ and $\psi(\varphi(g))=g$.

Write a bar for reduction modulo $p$. For $n\ge1$,

$$
\overline{T^{np}}=\overline\varphi(T^n),\qquad
\overline{T^{np-1}}=\overline\varphi(T^{n-1})T^{p-1}.
$$

The [binomial theorem](../../../../../binomial-theorem.md) in [characteristic](../../../../../characteristic-of-a-field.md) $p$ gives

$$
T^{p-1}=(X-1)^{p-1}=1+X+\cdots+X^{p-1}
\quad\text{in }\mathbb F_p[[T]],
$$

since $\binom{p-1}{i}\equiv(-1)^i\pmod p$ and $p$ is odd. Taking the zeroth basis coefficient yields

$$
\boxed{\psi(T^{np}+T^{np-1})\equiv T^n+T^{n-1}\pmod{pR}.}
$$

The endpoint case $n=1$ includes the constant term $T^0=1$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
