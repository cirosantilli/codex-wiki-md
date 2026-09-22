<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The probabilistic form of [Wick's theorem](../../../../../wick-s-theorem.md) is [Isserlis's theorem](../../../../../isserlis-s-theorem.md). If $(Y_1,\ldots,Y_k)$ is a centered [random vector](../../../../../random-vector.md) with a [multivariate Gaussian distribution](../../../../../multivariate-gaussian-distribution.md) and [covariance matrix](../../../../../covariance-matrix.md) $C$, its odd product [moments](../../../../../moment.md) vanish, and, for even $k$,

$$
\boxed{\mathbb E\prod_{a=1}^kY_a
=\sum_{\pi\in\mathcal P_2(k)}\prod_{\{a,b\}\in\pi}C_{ab}.}
$$

Here $\mathcal P_2(k)$ is the set of [perfect matchings](../../../../../perfect-matching.md) of the $k$ labelled positions. The formula allows repeated coordinates and singular [covariance matrices](../../../../../covariance-matrix.md). To see the pairing rule, differentiate the [moment-generating function](../../../../../moment-generating-function.md) $\exp(t^TCt/2)$ once in each coordinate and set $t=0$: only terms pairing all differentiated coordinates survive, each with the displayed product of [covariances](../../../../../covariance.md).

Take $Y_a=M_{i_ai_{a+1}}$, with $i_{k+1}=i_1$. These variables are linear combinations of the original [independent](../../../../../independent-random-variables.md) [normal random variables](../../../../../gaussian-random-variable.md), hence are jointly [Gaussian](../../../../../normal-distribution.md). They have zero [means](../../../../../expected-value-split.md), so

$$
\boxed{\mathbb E[M_{i_1i_2}\cdots M_{i_ki_1}]
=\sum_{\pi\in\mathcal P_2(k)}\prod_{\{a,b\}\in\pi}
\left(\delta_{i_ai_b}\delta_{i_{a+1}i_{b+1}}
+\delta_{i_ai_{b+1}}\delta_{i_{a+1}i_b}\right).}
$$

Substituting the entry [covariance](../../../../../covariance.md) from part (a)(i) identifies each parenthesis with $\mathbb E[M_{i_ai_{a+1}}M_{i_bi_{b+1}}]$, giving the requested identity.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the random matrix theory course of the University of Oxford](../../../../split.md)
6. [Random matrix theory course of the University of Oxford](../../../../../random-matrix-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
