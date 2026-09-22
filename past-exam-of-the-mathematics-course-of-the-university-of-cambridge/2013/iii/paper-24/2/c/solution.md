<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For fixed $u$, write $h(t)=\varphi_{X_t}(u)$. [Independent increments](../../../../../../independent-increments.md) and [stationary increments](../../../../../../stationary-increments.md) give

$$
h(s+t)=\mathbb E\bigl[e^{iuX_s}e^{iu(X_{s+t}-X_s)}\bigr]
=h(s)h(t),\qquad h(0)=1.
$$

The preceding part gives continuity. Also $h$ never vanishes: if $h(t_0)=0$ with $t_0>0$, then $h(t_0/m)^m=0$ for every positive integer $m$, contradicting $h(t_0/m)\to1$.

Here is a direct proof of the [exponential form of Lévy characteristic functions](../../../../../../exponential-form-of-levy-characteristic-functions.md). Choose $a>0$ small enough that $|h(t)-1|<1/2$ on $[0,a]$. The principal [complex logarithm](../../../../../../complex-logarithm.md) gives a continuous $L(t)=\log h(t)$ there, with $L(0)=0$. For $s,t\geq0$ with $s+t\leq a$, the multiplicative identity implies

$$
L(s+t)-L(s)-L(t)\in2\pi i\mathbb Z.
$$

This difference is continuous on the connected triangle of allowed $(s,t)$ and equals zero at $(0,0)$, so it is identically zero. Thus $L$ satisfies the additive [Cauchy functional equation](../../../../../../cauchy-s-functional-equation.md) locally. Subdivision gives $L(a/m)=L(a)/m$ and $L(ka/m)=kL(a)/m$; continuity then gives $L(t)=tL(a)/a$ for every $t\in[0,a]$.

Define $\eta(u)=L(a)/a$. For any $t\geq0$, choose an integer $m$ with $t/m\leq a$; then

$$
\boxed{\varphi_{X_t}(u)=h(t)=h(t/m)^m=e^{t\eta(u)}.}
$$

The coefficient is unique: if two coefficients give the same exponential for every $t\geq0$, their derivatives at zero agree. In particular $\eta(0)=0$, and $\operatorname{Re}\eta(u)\leq0$ follows from $|h(t)|\leq1$. The [characteristic exponent of a Lévy process](../../../../../../characteristic-exponent-of-a-levy-process.md) has therefore been obtained from first principles, without invoking the [Lévy–Khintchine formula](../../../../../../levy-khintchine-formula.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
