<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $q=\#k_K=p^f$. For every $a\in k_K$, the polynomial $F(T)=T^q-T$ has $a$ as a residue root and $\overline{F'}=-1$. By the [Hensel lemma](../../../../../../hensel-s-lemma.md) there is a unique element $[a]\in\mathcal O_K$ such that

$$
\boxed{\overline{[a]}=a,\qquad [a]^q=[a].}
$$

This defines the [Teichmuller lift](../../../../../../teichmuller-representative.md), including $[0]=0$. The two displayed properties determine each value uniquely by Hensel's uniqueness statement.

They also imply the standard [Teichmuller lift properties](../../../../../../teichmuller-lift-properties.md). The elements $0,1$ already satisfy their defining equations, so $[0]=0$ and $[1]=1$. The product $[a][b]$ reduces to $ab$ and satisfies $( [a][b])^q=[a][b]$, so uniqueness gives $[ab]=[a][b]$. Likewise $[a]^p$ reduces to $a^p$ and is fixed by its $q$th power, giving

$$
\boxed{[ab]=[a][b],\qquad [a^p]=[a]^p.}
$$

For $a\ne0$, division of $[a]^q=[a]$ by $[a]$ gives $[a]^{q-1}=1$. Thus the nonzero [Teichmuller representatives](../../../../../../teichmuller-representative.md) are precisely the prime-to-$p$ roots of unity lifting the nonzero residue classes. This is a multiplicative section of reduction; additivity is not asserted in mixed characteristic.

For the convergence, use the normalized [discrete valuation](../../../../../../discrete-valuation.md) $v_K$ with $v_K(\pi)=1$, and put $e=v_K(p)\geq1$. A useful binomial estimate is

$$
v_K(u^p-v^p)\geq\min\{e+r,pr\}\geq r+1
\quad\text{if }u,v\in\mathcal O_K,\ v_K(u-v)\geq r\geq1.
$$

Indeed, writing $u=v+\delta$, every intermediate coefficient $\binom pj$ is divisible by $p$, so all terms of $(v+\delta)^p-v^p$ have valuation at least $\min\{e+r,pr\}$. The [ultrametric inequality](../../../../../../ultrametric-inequality.md) gives the bound for their sum.

Finite fields are perfect, so the successive $p$th roots $x_n$ exist uniquely and satisfy $x_n^{p^n}=x$. Let $a_n=[x_n]$. Since $y_n-a_n$ lies in the maximal ideal, iterating the estimate $n$ times gives

$$
v_K(y_n^{p^n}-a_n^{p^n})\geq n+1.
$$

Multiplicativity, or the Frobenius identity above, gives $a_n^{p^n}=[x_n^{p^n}]=[x]$. Therefore

$$
\boxed{v_K(y_n^{p^n}-[x])\geq n+1,\qquad y_n^{p^n}\longrightarrow[x].}
$$

This proves the [approximation of Teichmuller lifts by iterated pth powers](../../../../../../approximation-of-teichmuller-lifts-by-iterated-pth-powers.md) for completely arbitrary choices of the lifts $y_n$, including $x=0$. The original PDF confirms $x\in k_K$, correcting the capital $K_K$ in the TeX transcription.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 123](../../../paper-123-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
