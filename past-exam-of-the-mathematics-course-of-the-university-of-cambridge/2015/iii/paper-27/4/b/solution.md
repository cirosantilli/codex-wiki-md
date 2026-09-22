<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $E_q=\max_{(a,q)=1}|\pi(x;q,a)-\operatorname{Li}(x)/\phi(q)|$, with $\operatorname{Li}$ the offset [logarithmic integral function](../../../../../../logarithmic-integral-function.md). The permitted standard sieve estimate can be taken as the [Brun–Titchmarsh theorem](../../../../../../brun-titchmarsh-theorem.md):

$$
\pi(x;q,a)\leq\frac{2x}{\phi(q)\log(x/q)},\qquad q<x,quad(a,q)=1.
$$

For $q\leq x^{0.99}$, $\log(x/q)\geq0.01\log x$. Also $\operatorname{Li}(x)\ll x/\log x$. Thus both terms defining $E_q$ are $O(x/(\phi(q)\log x))$, uniformly over the permitted moduli. Apply the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) in the form

$$
\sum_{q\leq Q}3^{\omega(q)}E_q
\leq\left(\sum_{q\leq Q}E_q\right)^{1/2}\left(\sum_{q\leq Q}9^{\omega(q)}E_q\right)^{1/2}
\ll\left(\sum_{q\leq Q}E_q\right)^{1/2}\left(\frac{x}{\log x}\sum_{q\leq Q}\frac{9^{\omega(q)}}{\phi(q)}\right)^{1/2}.
$$

This is the [weighted arithmetic-progression error bound](../../../../../../weighted-arithmetic-progression-error-bound.md). The [prime omega function](../../../../../../prime-omega-function.md) and [Euler totient function](../../../../../../euler-totient-function.md) weights can therefore be handled using an unweighted mean error and a separate positive [sum](../../../../../../sum.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
