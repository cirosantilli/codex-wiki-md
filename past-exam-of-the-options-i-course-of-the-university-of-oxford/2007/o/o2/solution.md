<h1 id="o/o2/solution">Solution</h1>

↑ **Parent:** [O2](../o2.md)

The power of a test at a parameter value is its probability of rejecting the null there. Its size is the supremum of this probability over the null parameter set. The [Neyman-Pearson lemma](../../../../neyman-pearson-lemma.md) states that for simple null and alternative densities $f_0,f_1$, a test rejecting where $f_1>cf_0$, accepting where $f_1<cf_0$, and randomizing as needed on equality to attain size $\alpha$, has greatest power among tests of size at most $\alpha$.

The specified function is nonnegative. Its integral is

$$
\frac{\theta^2}{\theta+1}\left\{\int_0^\infty xe^{-\theta x}\,dx+\int_0^\infty e^{-\theta x}\,dx\right\}
=\frac{\theta^2}{\theta+1}\left(\theta^{-2}+\theta^{-1}\right)=1.
$$

For independent observations write $S=\sum_iX_i$. The [likelihood ratio](../../../../likelihood-ratio.md) of the smaller alternative parameter to the null is

$$
\frac{L(\theta_1)}{L(\theta_0)}=
\left\{\frac{\theta_1^2(\theta_0+1)}{\theta_0^2(\theta_1+1)}\right\}^n
\exp\{(\theta_0-\theta_1)S\}.
$$

It is strictly increasing in $S$. Thus the most powerful level-$\alpha$ test rejects for

$$
\boxed{S>c_\alpha,\qquad\mathbb P_{\theta_0}(S>c_\alpha)=\alpha}.
$$

The continuous distribution permits this size without randomization for $0<\alpha<1$. Its threshold depends only on the null and the desired size, not on which $\theta_1<\theta_0$ was chosen. The same test is therefore **uniformly most powerful against the entire one-sided alternative $\theta<\theta_0$**.

## ↑ Ancestors (12)

1. [O2](../o2.md)
2. [O](../../o.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
