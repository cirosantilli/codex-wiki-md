# EM likelihood monotonicity

↑ **Parent:** [Expectation-maximization algorithm](expectation-maximization-algorithm.md)

For $Q(\theta\mid\theta_0)=\mathbb E_{\theta_0}[\log p_\theta(Y,Z)\mid Y]$, the [Jensen inequality](jensen-s-inequality.md) gives

$$
\log p_\theta(Y)-\log p_{\theta_0}(Y)\geq Q(\theta\mid\theta_0)-Q(\theta_0\mid\theta_0).
$$

Thus any [expectation-maximization algorithm](expectation-maximization-algorithm.md) M-step that increases $Q$ cannot decrease the observed-data [likelihood function](likelihood-function.md). Monotonicity does not by itself assert convergence to a global maximum.

## ↑ Ancestors (8)

1. [Expectation-maximization algorithm](expectation-maximization-algorithm.md)
2. [Latent variable](latent-variable.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (10)

- [EM for Gaussian mixtures with a common variance](em-for-gaussian-mixtures-with-a-common-variance.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/4/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-41/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-41/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-216/4/c/solution.md)
