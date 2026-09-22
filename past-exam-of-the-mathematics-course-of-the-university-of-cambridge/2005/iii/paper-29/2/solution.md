<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An [integer](../../../../../integer.md) version of [Siegel lemma](../../../../../siegel-s-lemma.md) is as follows. For $M<N$ homogeneous [linear equations](../../../../../linear-equation.md) $Az=0$, with [integer](../../../../../integer.md) [matrix](../../../../../matrix.md) entries bounded in absolute value by $A_0\geq1$, there is a nonzero [integer](../../../../../integer.md) solution satisfying

$$
\boxed{\|z\|_\infty\leq\left\lfloor(2NA_0)^{M/(N-M)}\right\rfloor.}
$$

Put the displayed [integer](../../../../../integer.md) bound equal to $Q$ and evaluate the equations at every [vector](../../../../../vector.md) in $\{0,\ldots,Q\}^N$. There are $(Q+1)^N$ inputs and at most $(2NA_0Q+1)^M$ outputs. But $2NA_0Q+1\leq2NA_0(Q+1)$ and $(Q+1)^{N-M}>(2NA_0)^M$, so the number of inputs is larger. Two distinct inputs have identical outputs; their difference proves the claim. This is the [pigeonhole proof of integer Siegel lemma](../../../../../pigeonhole-proof-of-integer-siegel-lemma.md). Rational coefficients are handled by clearing denominators. Over a [number field](../../../../../number-field.md) of degree $d$, expanding in a rational basis gives at most $dM$ rational equations, so the same construction applies when $N>dM$, with the height of the resulting [integer](../../../../../integer.md) [matrix](../../../../../matrix.md) controlling the bound.

Siegel's original arithmetic definition starts with an entire series $E(z)=\sum_{n\geq0}a_nz^n/n!$, with all $a_n$ in a fixed [number field](../../../../../number-field.md). For every $\epsilon>0$ there must be positive [integers](../../../../../integer.md) $d_n$ such that $d_na_0,\ldots,d_na_n$ are [algebraic integers](../../../../../algebraic-integer.md), and both $d_n$ and the absolute values of every conjugate of $a_n$ are $O_\epsilon(n^{\epsilon n})$. The growth condition ensures convergence everywhere. The stronger, now customary strict [E-function](../../../../../e-function.md) definition uses bounds $C^{n+1}$ for a fixed $C$ and also includes the requirement of a nonzero [linear differential equation](../../../../../linear-differential-equation.md) over $\overline{\mathbb Q}(z)$. In the original formulation, that differential condition is explicitly part of the system hypothesis in the theorem below. These definitions should be distinguished; the exponentials used here satisfy even the stronger conditions.

The [Siegel–Shidlovsky theorem](../../../../../siegel-shidlovsky-theorem.md) states that if a [vector](../../../../../vector.md) of [E-functions](../../../../../e-function.md) satisfies $f'=A(z)f$, with $A(z)$ a [matrix](../../../../../matrix.md) of [rational functions](../../../../../rational-function.md) over $\overline{\mathbb Q}$, then for every nonzero algebraic $\xi$ which is not a pole of $A$,

$$
\boxed{\operatorname{trdeg}_{\overline{\mathbb Q}}\overline{\mathbb Q}(f_1(\xi),\ldots,f_s(\xi))
=\operatorname{trdeg}_{\overline{\mathbb Q}(z)}\overline{\mathbb Q}(z)(f_1(z),\ldots,f_s(z)).}
$$

In particular, [algebraic independence](../../../../../algebraic-independence.md) of the functions implies [algebraic independence](../../../../../algebraic-independence.md) of the values. The exclusion of zero is necessary: their Taylor values there are algebraic.

Take rationally independent algebraic $\gamma_1,\ldots,\gamma_s$ and $f_j(z)=e^{\gamma_jz}$. Their coefficients are $\gamma_j^n$, their conjugates grow exponentially, and powers of a fixed common denominator clear all coefficients through degree $n$. They satisfy the nonsingular diagonal system $f_j'=\gamma_jf_j$.

To check functional independence, a [polynomial](../../../../../polynomial-split.md) relation among these exponentials, after clearing rational-function denominators, would be $\sum_mP_m(z)e^{\lambda_mz}=0$ with distinct $\lambda_m=\sum_jm_j\gamma_j$. Such an [exponential polynomial](../../../../../exponential-polynomial.md) cannot vanish identically. To isolate a nonzero term with exponent $\lambda_0$, apply $\prod_{\lambda\ne\lambda_0}(D-\lambda)^{\deg P_\lambda+1}$. All other terms vanish, while the remaining [polynomial](../../../../../polynomial-split.md) is acted on by operators $D+\lambda_0-\lambda$, each injective on [polynomials](../../../../../polynomial-split.md) because its nonzero constant preserves a nonzero leading coefficient. Thus the remaining term is nonzero, a contradiction.

The theorem at $\xi=1$ now makes $e^{\gamma_j}$ algebraically independent. For arbitrary distinct algebraic exponents $\alpha_i$, choose a rational basis of their span and divide its elements by a common denominator so that every $\alpha_i$ is an [integer](../../../../../integer.md) combination of the resulting $\gamma_j$. Then $e^{\alpha_i}$ are distinct Laurent monomials in $e^{\gamma_j}$. A linear relation among them becomes a nonzero [polynomial](../../../../../polynomial-split.md) relation after multiplying by a common monomial, contradicting independence. These particular [E-functions](../../../../../e-function.md) therefore yield the full [Lindemann–Weierstrass theorem](../../../../../lindemann-weierstrass-theorem.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
