<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

We give an explicit [Gimel recursion for cardinal exponentiation](../../../../../../gimel-recursion-for-cardinal-exponentiation.md). First recover the continuum [function](../../../../../../function-split.md) by induction on infinite [cardinals](../../../../../../cardinal-number.md). At a regular $\kappa$,

$$
2^\kappa=\kappa^\kappa=\gimel(\kappa),
$$

because $2^\kappa\le\kappa^\kappa\le(2^\kappa)^\kappa=2^\kappa$. At a singular $\kappa$, put $\theta=\operatorname{cf}(\kappa)$ and $s=\sup_{\rho<\kappa}2^\rho$, whose value is already known. A cofinal sequence $(\kappa_i)_{i<\theta}$ gives

$$
\boxed{2^\kappa=s^\theta.}
$$

Indeed $\prod_i2^{\kappa_i}=2^{\sum_i\kappa_i}=2^\kappa\le s^\theta$, while $s\le2^\kappa$ gives the reverse inequality after raising to $\theta$.

If the supremum $s$ is attained, the continuum [function](../../../../../../function-split.md) is eventually constant below $\kappa$, and we may choose $\rho<\kappa$ with $\rho\ge\theta$ and $2^\rho=s$. Then $s^\theta=(2^\rho)^\theta=s$. If it is not attained, the increasing cofinal power values show $\operatorname{cf}(s)=\theta$. To verify the reverse [cofinality](../../../../../../cofinality.md) bound, fewer than $\theta$ such lower power values have indices bounded below $\kappa$, and cannot be cofinal in $s$; the upper bound comes from $(\kappa_i)$. Consequently

$$
\boxed{2^\kappa=\begin{cases}s,&s\text{ attained below }\kappa,\\
\gimel(s),&s\text{ not attained below }\kappa.
\end{cases}}
$$

Every singular-stage value is therefore determined by the previously computed powers and the given [Gimel function](../../../../../../gimel-function.md).

Now fix an infinite exponent $\lambda$ and recurse on the infinite base $\kappa$. If $2\le\kappa\le\lambda$, then $\kappa^\lambda=2^\lambda$, already known. For a successor base $\kappa=\rho^+>\lambda$, every [function](../../../../../../function-split.md) $\lambda\to\kappa$ has bounded range, and each bounded range has size at most $\rho$. Hence

$$
\boxed{\kappa^\lambda=\max\{\kappa,\rho^\lambda\}.}
$$

This is the [Hausdorff formula for cardinal exponentiation](../../../../../../hausdorff-formula-for-cardinal-exponentiation.md). For a limit base $\kappa>\lambda$, put $a=\sup_{\rho<\kappa}\rho^\lambda$ and $\theta=\operatorname{cf}(\kappa)$. If $\theta>\lambda$, all ranges are bounded and counting over those bounds gives $\kappa^\lambda=a$ (here $a\ge\kappa$).

If $\theta\le\lambda$, then $\kappa^\lambda=a^\theta$. To see the nontrivial upper bound, use a cofinal sequence of bounds $\kappa_i$. A [function](../../../../../../function-split.md) $\lambda\to\kappa$ is coded by the assignment of each argument to one of these $\theta$ bounds, together with $\theta$ padded [functions](../../../../../../function-split.md) into the corresponding bounds. The assignment has at most $\theta^\lambda=2^\lambda\le a$ possibilities, and the [functions](../../../../../../function-split.md) have at most $a^\theta$ possibilities. Conversely $a\le\kappa^\lambda$ and $(\kappa^\lambda)^\theta=\kappa^\lambda$, giving the lower bound. If $a$ is attained as $\rho^\lambda$, then $a^\theta=a$ by currying; otherwise $\operatorname{cf}(a)=\theta$ by the same cofinal-index argument as above. Thus

$$
\boxed{\kappa^\lambda=\begin{cases}
a,&\operatorname{cf}(\kappa)>\lambda,\\
a,&\operatorname{cf}(\kappa)\le\lambda\text{ and }a\text{ attained},\\
\gimel(a),&\operatorname{cf}(\kappa)\le\lambda\text{ and }a\text{ not attained}.
\end{cases}}
$$

Only smaller-base powers occur in $a$, so this is a genuine recursion, not an implicit appeal to the unknown power.

Finally, finite positive exponents give $\kappa^n=\kappa$ for infinite $\kappa$; finite bases at infinite exponents satisfy $m^\lambda=2^\lambda$ for $m\ge2$. The cases with base $0$ or $1$, exponent $0$, or both arguments finite are elementary, with $0^0=1$ under the empty-function convention. **The [Gimel function](../../../../../../gimel-function.md) therefore determines both requested class [functions](../../../../../../function-split.md) completely.**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
