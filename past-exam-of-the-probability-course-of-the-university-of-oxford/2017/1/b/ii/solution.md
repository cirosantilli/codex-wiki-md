<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The two recursions use a [synchronous coupling](../../../../../synchronous-coupling.md): they receive exactly the same fresh inputs. Subtraction cancels the additive term:

$$
Z_n-X_n=U_n(Z_{n-1}-X_{n-1}).
$$

The variable $U_n$ is independent of the preceding difference and has [expected value](../../../../../expected-value-split.md) $1/2$. Thus [expectation of a product of independent random variables](../../../../../expectation-of-a-product-of-independent-random-variables.md) gives

$$
\mathbb E|Z_n-X_n|=\frac12\mathbb E|Z_{n-1}-X_{n-1}|
=2^{-n}\mathbb E|c-E_0|\leq2^{-n}(|c|+1).
$$

By [Markov's inequality](../../../../../markov-s-inequality.md), for every $\varepsilon>0$,

$$
\boxed{\mathbb P(|Z_n-X_n|>\varepsilon)\leq\frac{|c|+1}{\varepsilon\,2^n}\longrightarrow0.}
$$

This proves the requested [convergence in probability](../../../../../convergence-in-probability.md); in fact the difference has [L1 convergence](../../../../../convergence-in-l1.md). It is [synchronous contraction of a random affine recursion](../../../../../synchronous-contraction-of-a-random-affine-recursion.md), and the estimate holds for every real $c$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
