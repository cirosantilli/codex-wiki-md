<h1 id="28k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Since the MLE has constant risk $p$, its worst-case risk is $p$, so the minimax risk is at most $p$. On the other hand, the worst-case risk of every estimator is at least its average risk under any prior, and therefore at least the optimal Bayes risk for that prior. Using $\pi_c=N_p(0,c^2I_p)$ gives

$$
\inf_\delta\sup_\theta R(\theta,\delta)
\geq r(\pi_c)=\frac{pc^2}{1+c^2}.
$$

Letting $c\to\infty$ yields a lower bound $p$. The bounds agree, proving the [minimaxity of the usual multivariate normal mean estimator](../../../../../../minimaxity-of-the-usual-multivariate-normal-mean-estimator.md):

$$
\boxed{\inf_\delta\sup_\theta R(\theta,\delta)=p,
\qquad\widehat\theta_{\rm MLE}=X\text{ is minimax}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [28K](../../28k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
