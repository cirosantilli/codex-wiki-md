<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**The printed minimization of the [evidence lower bound](../../../../../evidence-lower-bound.md) has no solution.** To distinguish that literal result from the usual [variational inference](../../../../../variational-inference.md) optimum, put $S=\sigma_1^{-2}+\sigma_2^{-2}>0$. The preceding [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md) satisfies

$$
\mathcal J'(\phi)=S\phi-\frac2\phi,\qquad \mathcal J''(\phi)=S+\frac2{\phi^2}>0.
$$

Its unique [global minimum](../../../../../global-minimum.md) occurs at $\phi^2=2/S$. Since $\mathcal L=\log p(\mathcal D)-\mathcal J$, this is the unique [global maximum](../../../../../global-maximum.md) of the [evidence lower bound](../../../../../evidence-lower-bound.md):

$$
\boxed{\phi_{\rm ELBO\,max}=\sqrt{\frac{2\sigma_1^2\sigma_2^2}{\sigma_1^2+\sigma_2^2}}}.
$$

The optimal common [variance](../../../../../variance-split.md) is the [harmonic mean](../../../../../harmonic-mean.md) of the two posterior [variances](../../../../../variance-split.md). However, $\mathcal J(\phi)\to+\infty$ as either $\phi\downarrow0$ or $\phi\to\infty$. Therefore

$$
\boxed{\inf_{\phi>0}\mathcal L(\phi)=-\infty,\qquad\text{no minimizing }\phi\text{ exists}}.
$$

The source PDF confirms the minimization wording; replacing it by maximization would give the finite value above, consistently with part (i).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the advanced topics in statistical machine learning course of the University of Oxford](../../../../split.md)
6. [Advanced topics in statistical machine learning course of the University of Oxford](../../../../../advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics and statistics course of the University of Oxford](../../../../../year-4-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
