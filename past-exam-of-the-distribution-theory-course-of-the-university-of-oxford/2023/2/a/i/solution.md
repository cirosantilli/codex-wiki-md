<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Convergence $\phi_j\to\phi$ in the [space of test functions](../../../../../space-of-test-functions.md) means that all [supports](../../../../../support.md) lie in one [compact set](../../../../../compact-space.md) $K\subset\mathbb R$ and $\|\phi_j^{(r)}-\phi^{(r)}\|_\infty\to0$ for every integer $r\geq0$. An eventual common [compact support](../../../../../compact-support.md) is equivalent, since finitely many initial [supports](../../../../../support.md) can be added to $K$.

Write the standard [mollifier](../../../../../mollifier.md) as $\rho_\varepsilon(x)=\varepsilon^{-1}\rho(x/\varepsilon)$, where $\rho\in\mathcal D(\mathbb R)$ is nonnegative, supported in $[-1,1]$, and has integral one. For $0<\varepsilon\leq1$, the [convolution](../../../../../convolution.md) $\rho_\varepsilon*\phi$ has [support](../../../../../support.md) in the fixed [compact set](../../../../../compact-space.md) $\operatorname{supp}\phi+[-1,1]$. The given [convolution derivative identity](../../../../../differentiation-commutes-with-convolution.md) yields

$$
(\rho_\varepsilon*\phi)^{(r)}(x)-\phi^{(r)}(x)
=\int_{-1}^{1}\rho(y)\bigl[\phi^{(r)}(x-\varepsilon y)-\phi^{(r)}(x)\bigr],dy.
$$

Each $\phi^{(r)}$ is uniformly continuous; more explicitly, the [mean value theorem](../../../../../mean-value-theorem.md) bounds the absolute value by $\varepsilon\|\phi^{(r+1)}\|_\infty\int|y|\rho(y)\,dy$, uniformly in $x$. Thus

$$
\boxed{\rho_\varepsilon*\phi\longrightarrow\phi\text{ in }\mathcal D(\mathbb R).}
$$

If $\phi_j\to0$ in the [space of test functions](../../../../../space-of-test-functions.md) and $K$ is a common [compact support](../../../../../compact-support.md), then $\|\phi_j\|_{L^1}\leq|K|\|\phi_j\|_\infty\to0$, where $|K|$ is its [Lebesgue measure](../../../../../lebesgue-measure.md).

The [mollifiers](../../../../../mollifier.md) themselves have no limit in the [L1 space](../../../../../l1-space.md). If $\rho_\varepsilon\to g$ in that [norm](../../../../../norm.md), then for each $\delta>0$ the integral of $|g|$ on $\{|x|>\delta\}$ is zero, because $\rho_\varepsilon$ vanishes there for $\varepsilon<\delta$. Hence $g=0$ [almost everywhere](../../../../../almost-everywhere.md). This contradicts $\|\rho_\varepsilon\|_{L^1}=1$. Therefore $\boxed{\rho_\varepsilon\text{ does not converge in }L^1(\mathbb R)}$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the distribution theory course of the University of Oxford](../../../../split.md)
6. [Distribution theory course of the University of Oxford](../../../../../distribution-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
