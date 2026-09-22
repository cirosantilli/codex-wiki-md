<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Choose $\epsilon=1/6$ and a sufficiently large absolute constant $k$. Part (iii)'s size bound gives

$$
|Y|/|G|\ge\alpha^{O(1)}.
$$

Let

$$
\Gamma=\{\gamma\in\widehat G:|\widehat{\mu_Y}(\gamma)|\ge1/2\}
$$

and choose a maximal [dissociated set](../../../../../../dissociated-set.md) $\Lambda\subseteq\Gamma$. The entropy form of the [Chang theorem](../../../../../../chang-theorem.md) gives

$$
|\Lambda|=O(\log(|G|/|Y|))=O(\log(\alpha^{-1})),
$$

and maximality gives $\Gamma\subseteq\operatorname{Span}(\Lambda)$.

Put $B=B(\Lambda,1/(6|\Lambda|))$. If $y\in B$ and $\gamma\in\Gamma$, expressing $\gamma$ as a product of characters in $\Lambda$ and their inverses gives

$$
|\gamma(y)-1|\le1/6.
$$

For $f=1_{-A}*\mu_A$, [Parseval identity](../../../../../../parseval-identity.md) gives

$$
\widehat f(\gamma)=\frac{|\widehat{1_A}(\gamma)|^2}{\alpha},
\qquad
\sum_\gamma|\widehat f(\gamma)|=1.
$$

Also $\widehat\mu(\gamma)=|\widehat{\mu_Y}(\gamma)|^{2k}$. [Fourier inversion theorem](../../../../../../fourier-inversion-theorem.md) therefore yields

$$
|f*\mu(x+y)-f*\mu(x)|
\le\frac16\sum_{\gamma\in\Gamma}|\widehat f(\gamma)|
+2^{1-2k}\sum_{\gamma\notin\Gamma}|\widehat f(\gamma)|
\le\frac13
$$

once $k$ is large enough.

If $\Lambda$ is empty, interpret $B$ as $G$; the same Fourier estimate, using only the second term, is even stronger.

Part (iii) gives $\|f*\mu-f\|_\infty\le1/6$. Applying this at $x$ and $x+y$ and using the last estimate gives

$$
\boxed{|f(x+y)-f(x)|\le2/3.}
$$

Finally $f(0)=1$. Hence $f(y)\ge1/3>0$ for every $y\in B$, while the support of $f$ is $A-A$. Consequently

$$
\boxed{B\subseteq A-A.}
$$

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
