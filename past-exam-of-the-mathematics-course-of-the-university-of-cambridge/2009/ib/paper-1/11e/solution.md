<h1 id="11e/solution">Solution</h1>

↑ **Parent:** [11E](../11e.md)

Let $\phi(t)=\operatorname{dist}(t,\mathbb Z)$. It is continuous and takes values in $[0,1/2]$. The finite sums $f_N(x)=\sum_{n=1}^N2^{-n}\phi(2^nx)$ are continuous and their tails obey

$$
|f(x)-f_N(x)|\le\frac12\sum_{n>N}2^{-n}=2^{-N-1}
$$

for every real $x$. To prove continuity without invoking an unproved uniform-limit theorem, fix $x$ and $\varepsilon>0$. Choose $N$ with $2\cdot2^{-N-1}<\varepsilon/2$, then use continuity of $f_N$ to make $|f_N(y)-f_N(x)|<\varepsilon/2$ near $x$. The [triangle inequality](../../../../../triangle-inequality.md) then gives $|f(y)-f(x)|<\varepsilon$. Thus **$f$ is continuous**; it is the scaled [Takagi function](../../../../../blancmange-curve.md) $T(2x)/2$.

For the general secant claim, differentiability gives $g(x+h)=g(x)+g'(x)h+r(h)$, where $|r(h)|\le\varepsilon|h|$ for sufficiently small $h$, with $r(0)=0$. Since the two endpoints straddle $x$,

$$
\left|\frac{g(v_n)-g(u_n)}{v_n-u_n}-g'(x)\right|\le\varepsilon\frac{|v_n-x|+|u_n-x|}{v_n-u_n}=\varepsilon.
$$

Hence **the secant limit is $g'(x)$**, including cases where an endpoint equals $x$. This proves [secants straddling a differentiability point](../../../../../secants-straddling-a-differentiability-point.md).

Now take the nested dyadic intervals $u_N=2^{-N}\lfloor2^Nx\rfloor$, $v_N=u_N+2^{-N}$. They straddle $x$ and shrink to it. For every $n\ge N$, $2^nu_N$ and $2^nv_N$ are integers, so the corresponding summand vanishes at both endpoints. For $n<N$, all corners of that summand lie on the dyadic grid of mesh $2^{-N}$; on the chosen open interval it is linear with slope $\varepsilon_n\in\{-1,1\}$. Therefore its total secant slope is

$$
S_N=\frac{f(v_N)-f(u_N)}{v_N-u_N}=\sum_{n=1}^{N-1}\varepsilon_n.
$$

Refining to the nested interval preserves the slopes of all old terms and adds exactly one new term of slope $+1$ or $-1$. Thus $|S_{N+1}-S_N|=1$ for every $N$, so $S_N$ cannot converge. This contradicts the secant consequence of differentiability at any $x$. Therefore **$f$ is nowhere differentiable**. At dyadic $x$ the intervals chosen on its right satisfy the same argument. The printed reference to a denominator $2^{-n}$ is naturally read as mesh $2^{-n}$, or denominator $2^n$, as used here.

## ↑ Ancestors (10)

1. [11E](../11e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
