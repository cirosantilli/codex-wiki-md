<h1 id="20g/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The polynomial of $\alpha$ satisfies the [Eisenstein criterion](../../../../../../../eisenstein-criterion.md) at $p$. Let $\mathfrak p$ be any [prime ideal](../../../../../../../prime-ideal.md) of $\mathcal O_K$ above $p$, normalize its ideal valuation by $v_{\mathfrak p}(\mathfrak p)=1$, and write $e=v_{\mathfrak p}(p)$ for its [ramification index of a prime ideal](../../../../../../../ramification-index-of-a-prime-ideal.md). Put $t=v_{\mathfrak p}(\alpha)$. In

$$
\alpha^n+a_{n-1}\alpha^{n-1}+\cdots+a_0=0,
$$

the constant term has valuation $e$, while every other $a_j\alpha^j$ has valuation at least $e+jt$. The [non-Archimedean valuation](../../../../../../../non-archimedean-valuation.md) property then forces

$$
nt=e.
$$

Indeed, either strict inequality would leave a unique term of least valuation in the equation. Since $t$ is a positive integer and $e\le n$, it follows that $t=1$ and $e=n$.

The fundamental inequality $\sum_{\mathfrak p\mid p}e_{\mathfrak p}f_{\mathfrak p}\le n$ now shows that $\mathfrak p$ is the unique prime above $p$ and has residue degree one. At this prime,

$$
v_{\mathfrak p}(p)=n,\qquad v_{\mathfrak p}(\alpha)=1,
$$

while $(p,\alpha)$ has no factor away from $p$. Unique [prime ideal factorization](../../../../../../../prime-ideal-factorization.md) therefore gives

$$
\boxed{P=(p,\alpha)=\mathfrak p,\qquad P^n=(p)}.
$$

Finally $v_P(\alpha)=1$, so

$$
\boxed{\alpha\notin P^2}.
$$

This is [total ramification from an Eisenstein polynomial](../../../../../../../total-ramification-from-an-eisenstein-polynomial.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [20G](../../../20g.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
