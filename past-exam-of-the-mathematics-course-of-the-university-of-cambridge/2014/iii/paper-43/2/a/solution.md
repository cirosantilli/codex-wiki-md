<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [left Grassmann derivatives](../../../../../../left-grassmann-derivative.md) and the usual contractions $\partial^2=\partial^\alpha\partial_\alpha$ and $\bar\partial^2=\bar\partial_{\dot\alpha}\bar\partial^{\dot\alpha}$. Set $a=\theta^1,b=\theta^2,c=\bar\theta^{\dot1},d=\bar\theta^{\dot2}$. The printed epsilon convention gives

$$
\theta_1=-b,\quad\theta_2=a,\qquad
\bar\theta_{\dot1}=-d,\quad\bar\theta_{\dot2}=c,
\qquad \theta\theta=-2ab,\quad\bar\theta\bar\theta=2cd.
$$

The reversal of the barred contraction is essential. The [left Grassmann derivative](../../../../../../left-grassmann-derivative.md) obeys the [graded Leibniz rule](../../../../../../graded-leibniz-rule.md), so $\partial_a(ab)=b$ but $\partial_b(ab)=-a$. With the index-raising convention,

$$
\partial^2=2\partial_b\partial_a,\qquad
\bar\partial^2=2\partial_c\partial_d.
$$

Applying these to the displayed [Grassmann algebra](../../../../../../grassmann-algebra.md) monomials gives **$A=B=-4$**. Since every antisymmetric two-index product is proportional to epsilon, the $12$ and $\dot1\dot2$ components give

$$
\theta^\alpha\theta^\beta=-\frac12\epsilon^{\alpha\beta}(\theta\theta),\qquad
\bar\theta^{\dot\alpha}\bar\theta^{\dot\beta}=\frac12\epsilon^{\dot\alpha\dot\beta}(\bar\theta\bar\theta).
$$

Thus **$C=-2$ and $D=2$**.

In the remaining contraction, moving the first barred [Grassmann variable](../../../../../../grassmann-variable.md) past the second unbarred one introduces a minus sign. Inserting the two spinor identities then gives

$$
\begin{aligned}
(\theta\sigma^\mu\bar\theta)(\theta\sigma^\nu\bar\theta)
&=\frac14(\theta\theta)(\bar\theta\bar\theta)\epsilon^{\alpha\beta}\epsilon^{\dot\alpha\dot\beta}
\sigma^\mu_{\alpha\dot\alpha}\sigma^\nu_{\beta\dot\beta}\\
&=\frac14(\theta\theta)(\bar\theta\bar\theta)\operatorname{Tr}(\sigma^\mu\bar\sigma^\nu)\\
&=\frac12(\theta\theta)(\bar\theta\bar\theta)\eta^{\mu\nu}.
\end{aligned}
$$

The trace normalization is the one explicitly supplied in the paper. These [two-component superspace contraction signs](../../../../../../two-component-superspace-contraction-signs.md) therefore give

$$
\boxed{(A,B,C,D,E)=(-4,-4,-2,2,2).}
$$

As a direct check in the mostly-minus convention, $\sigma^0=I$ gives $(ac+bd)^2=-2abcd$, whereas $(\theta\theta)(\bar\theta\bar\theta)=-4abcd$. Their ratio is $+1/2$. A convention with $\operatorname{Tr}(\sigma^\mu\bar\sigma^\nu)=-2\eta^{\mu\nu}$ would change this last metric-relative sign; it is not the printed trace convention.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
