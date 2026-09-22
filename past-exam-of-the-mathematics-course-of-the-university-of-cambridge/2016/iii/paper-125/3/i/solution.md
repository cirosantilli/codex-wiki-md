<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Here a formal group means a one-dimensional commutative [formal group law](../../../../../../formal-group-law.md). Over a ring $R$, it is a [formal power series](../../../../../../formal-power-series.md) $F(X,Y)\in R[[X,Y]]$ satisfying

$$
F(X,0)=X,\quad F(0,Y)=Y,\quad F(F(X,Y),Z)=F(X,F(Y,Z)),\quad F(X,Y)=F(Y,X).
$$

In particular, $F(X,Y)=X+Y+$ terms of total degree at least $2$. A formal inverse $\iota(T)=-T+\cdots$ with $F(T,\iota(T))=0$ is obtained recursively. An [isomorphism of formal group laws](../../../../../../isomorphism-of-formal-group-laws.md) from $F$ to $G$ is a series $h(T)\in TR[[T]]$ with invertible linear coefficient and

$$
h(F(X,Y))=G(h(X),h(Y)).
$$

Its compositional inverse exists over $R$ by coefficient recursion.

For $R=\mathcal O_K$, all these series converge on $\pi\mathcal O_K$; the operations preserve that set and make it the group $F(\pi\mathcal O_K)$. Use the [uniformizer](../../../../../../uniformizer.md) $\pi$ and normalize the valuation by $v_K(\pi)=1$, and write $e=v_K(p)$.

We explicitly construct its [formal logarithm](../../../../../../formal-logarithm.md). Define

$$
f(T)=\frac{\partial F}{\partial Y}(T,0)=1+\cdots\in\mathcal O_K[[T]],\qquad
\frac1{f(T)}=\sum_{j\geq0}a_jT^j,\quad a_j\in\mathcal O_K.
$$

Then put

$$
\boxed{\log_F(T)=\int_0^T\frac{dt}{f(t)}=\sum_{j\geq0}\frac{a_j}{j+1}T^{j+1}.}
$$

This is a formal series over $K$ with linear coefficient $1$. Differentiating associativity in its last variable at $Z=0$ gives

$$
\frac{\partial F}{\partial Y}(X,Y)f(Y)=f(F(X,Y)).
$$

It follows that the $Y$-derivative of $\log_F(F(X,Y))$ is $1/f(Y)$, the same as that of $\log_F(Y)$. Evaluating at $Y=0$ therefore proves

$$
\boxed{\log_F(F(X,Y))=\log_F(X)+\log_F(Y).}
$$

The differential $dT/f(T)$ is the [invariant differential of a formal group law](../../../../../../invariant-differential-of-a-formal-group-law.md).

Choose an integer $m>e/(p-1)$. In degree $n\geq2$, the coefficient of $\log_F(T)$ has valuation at least $-e\,v_p(n)$. Thus the scaled series

$$
H(U)=\pi^{-m}\log_F(\pi^mU)=U+\sum_{n\geq2}c_nU^n
$$

has

$$
v_K(c_n)\geq(n-1)m-e\,v_p(n)>0.
$$

Here $v_p(n)\leq(n-1)/(p-1)$, and the coefficient valuations tend to infinity. Consequently $H(U)=U+\pi R(U)$ with $R$ a convergent integral power series on $\mathcal O_K$. Such a series is $1$-Lipschitz. For any $a\in\mathcal O_K$, the equation $H(U)=a$ is equivalent to $U=a-\pi R(U)$, a strict contraction, to which the [contraction mapping theorem](../../../../../../contraction-mapping-theorem.md) applies on the complete ring $\mathcal O_K$. It has exactly one solution.

The [deep logarithm subgroup of a formal group](../../../../../../deep-logarithm-subgroup-of-a-formal-group.md) is obtained as follows. The [formal group exponential](../../../../../../formal-group-exponential.md) is the formal compositional inverse $\exp_F(T)$ of $\log_F(T)$, obtained recursively; equivalently it solves $\exp_F'(T)=f(\exp_F(T))$, with $\exp_F(0)=0$. The preceding contraction, applied to the scaled series, constructs its convergent inverse on $\pi^m\mathcal O_K$ and agrees with that formal inverse. This supplies the required convergence sketch for $\exp_F$ as well as a bijectivity proof for the logarithm.

The integral formal law and inverse preserve $\pi^m\mathcal O_K$, so this is a subgroup. The logarithm identity and bijectivity give

$$
\boxed{F(\pi^m\mathcal O_K)\xrightarrow{\ \pi^{-m}\log_F\ }(\mathcal O_K,+)\quad\text{an isomorphism}.}
$$

Reduction of the formal law modulo $\pi^m$ has kernel $F(\pi^m\mathcal O_K)$. Its underlying image set is $\pi\mathcal O_K/\pi^m\mathcal O_K$, which has size $q^{m-1}$, where $q=\#(\mathcal O_K/\pi)$. Thus this subgroup has finite index, explicitly $q^{m-1}$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
