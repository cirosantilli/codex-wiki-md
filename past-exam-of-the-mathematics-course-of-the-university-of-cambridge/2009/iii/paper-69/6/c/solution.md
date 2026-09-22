<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take $a=5$ and $x=\pi/2$. Since $5^k\equiv1\pmod4$, every cosine term vanishes at $x$, and

$$
g(\pi/2+h)-g(\pi/2)=-\sum_{k=0}^\infty5^{-k}\sin(5^kh).
$$

Set $h=1/n$ and $m=\lfloor\log_5n\rfloor$. For $0\le k\le m$, the sine argument lies in $[0,1]$, where $\sin u\ge(\sin1)u$. The initial part therefore has a common sign and magnitude at least $(m+1)(\sin1)/n$. The remaining tail has absolute value at most

$$
\sum_{k=m+1}^\infty5^{-k}=\frac{5^{-m}}4\le\frac5{4n}.
$$

The [reverse triangle inequality](../../../../../../reverse-triangle-inequality.md) now gives

$$
|g(\pi/2+1/n)-g(\pi/2)|
\ge\frac{(m+1)\sin1-5/4}{n}
\ge c\frac{\ln n}{n}
$$

for sufficiently large $n$, because $m+1>\ln n/\ln5$. This establishes **the sharp logarithmic lower bound**

$$
\boxed{|g(\pi/2+1/n)-g(\pi/2)|\ge c\frac{\ln n}{n},\qquad
\omega(g,1/n)\ge c\frac{\ln n}{n}.}
$$

The constant can be reduced to include the finitely many small indices: for $n\ge5$ the displayed lower bound is positive; for $n=2,3$ the first sine exceeds the tail bound $1/4$, and for $n=4$ the first two sines contribute $\sin(1/4)+\sin(5/4)/5$, exceeding the remaining tail bound $1/20$. At $n=1$ the logarithmic right side is zero.

Here $E_n(g)\asymp1/n$ but $g$ is not [Lipschitz continuous](../../../../../../lipschitz-continuity.md), so a first [modulus of continuity](../../../../../../modulus-of-continuity.md) bound $O(1/n)$ is sufficient by the [first Jackson theorem for periodic approximation](../../../../../../first-jackson-theorem-for-periodic-approximation.md) but is not necessary. Nor is the weaker necessary bound $O(\ln n/n)$ sufficient: an explicit comparison is the [logarithmic cusp with slow trigonometric approximation](../../../../../../logarithmic-cusp-with-slow-trigonometric-approximation.md)

$$
h(x)=|x|\ln\frac{e\pi}{|x|}\quad(-\pi\le x\le\pi),\qquad h(0)=0,
$$

extended periodically. On $[0,\pi]$ it is increasing and concave, so its largest increment over distance $\delta$ is from zero, giving $\omega(h,\delta)=\delta\ln(e\pi/\delta)$ for $0<\delta\le\pi$.

For a concrete approximation lower bound, its cosine [Fourier coefficients](../../../../../../fourier-coefficient.md) satisfy

$$
a_j=\frac2\pi\int_0^\pi h(x)\cos(jx)\,dx
=-\frac{2}{\pi j^2}H_j,\qquad
H_j=\int_0^{j\pi}\frac{1-\cos u}{u}\,du=\ln j+O(1).
$$

Indeed, [integration by parts](../../../../../../integration-by-parts.md) once replaces $h$ by $h'(x)=\ln(\pi/x)$; integrating that against sine with primitive $(1-\cos jx)/j$ yields the stated positive integral. Its logarithmic growth follows because $\int_1^A\cos u/u\,du$ stays bounded by the [Dirichlet test](../../../../../../dirichlet-test.md). All $a_j$ are negative and absolutely summable.

Let $V_n=2\sigma_{2n}-\sigma_n$, a [de la Vallée Poussin sum](../../../../../../de-la-vallee-poussin-sum.md). Its multiplier is one for $j\le n$, $2-j/n$ for $n<j<2n$, and zero for $j\ge2n$; the [Fejér summation is a uniform-norm contraction](../../../../../../fejer-summation-is-a-uniform-norm-contraction.md) property gives $\|V_n\|\le3$. Thus the functional $L_n(f)=f(0)-V_nf(0)$ has norm at most four and vanishes on every degree-at-most-$n$ [trigonometric polynomial](../../../../../../trigonometric-polynomial.md). Because the remaining multiplier weights are nonnegative and all $a_j<0$,

$$
|L_n(h)|\ge\sum_{j\ge2n}|a_j|\gtrsim\frac{\ln n}{n},\qquad
E_n(h)\ge\frac{|L_n(h)|}4\gtrsim\frac{\ln n}{n}.
$$

The [first Jackson theorem for periodic approximation](../../../../../../first-jackson-theorem-for-periodic-approximation.md) gives the corresponding upper bound. **The same first-modulus order $\delta\ln(1/\delta)$ occurs with both $E_n\asymp1/n$ and $E_n\asymp\ln n/n$.** Therefore first-modulus rates alone do not characterize the endpoint approximation class, unlike the matched direct and inverse rates for $0<\alpha<1$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
