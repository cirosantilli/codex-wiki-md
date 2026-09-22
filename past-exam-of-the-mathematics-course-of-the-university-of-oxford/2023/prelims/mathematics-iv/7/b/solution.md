<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the relative reciprocal error $\varepsilon_k=1-px_k$. The iteration has the exact identity

$$
px_{k+1}=3px_k-3(px_k)^2+(px_k)^3=1-(1-px_k)^3,
$$

so

$$
\boxed{\varepsilon_{k+1}=\varepsilon_k^3,\qquad\varepsilon_k=\varepsilon_0^{3^k}.}
$$

Consequently $|1-px_0|<1$ guarantees $x_k\to1/p$. For real $p,x_0$, this condition is $0<px_0<2$. A starting guess can be found without division by choosing $x_0$ with the sign of $p$ and repeatedly halving its magnitude until $0<px_0<2$.

For the absolute signed error $e_k=x_k-1/p$, the same identity gives

$$
\boxed{e_{k+1}=p^2e_k^3.}
$$

Thus the method has [cubic convergence](../../../../../../cubic-convergence.md), of [order of convergence](../../../../../../order-of-convergence.md) three, with asymptotic error constant $p^2>0$ for a nonexact convergent start. Convergence requires a suitable guess: $px_0=0$ and $px_0=2$ correspond to $\varepsilon_0=1$ and $\varepsilon_0=-1$, respectively, so both are fixed failures. For $|1-px_0|>1$ the error magnitude grows without bound. The exact initial value $px_0=1$ is already the answer.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
