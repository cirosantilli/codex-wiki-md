<h1 id="o/o2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $S=\sum_i x_i$ and $\bar x=S/n$. Terms independent of $p$ can be dropped from the [log-likelihood](../../../../../log-likelihood.md), leaving

$$
\ell(p)=nr\log p+S\log(1-p)+C,
\quad\ell'(p)=\frac{nr}p-\frac S{1-p},
\quad\ell''(p)=-\frac{nr}{p^2}-\frac S{(1-p)^2}.
$$

For $S>0$, strict concavity gives the unique interior [maximum likelihood estimator](../../../../../maximum-likelihood-estimator.md)

$$
\boxed{\widehat p=\frac{nr}{nr+S}=\frac r{r+\bar x}}.
$$

If $S=0$, the likelihood increases up to $p=1$: this is the boundary estimate on the closed parameter range, or a supremum if the model insists on $p<1$.

Using the given mean, the sample [Fisher information](../../../../../fisher-information-matrix.md) is

$$
I_n(p)=-\mathbb E\ell''(p)
=\frac{nr}{p^2}+\frac{nr(1-p)/p}{(1-p)^2}
=\boxed{\frac{nr}{p^2(1-p)}}.
$$

The information per observation is $I_1(p)=r/[p^2(1-p)]$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [O2](../../o2.md)
3. [O](../../../o.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
