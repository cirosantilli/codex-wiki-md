<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [product topology](../../../../../../product-topology.md) on $\mathcal C=[k]^{\mathbb Z}$, with $[k]$ discrete, and the [left shift](../../../../../../left-shift.md) $(\mathcal Lc)(j)=c(j+1)$. A basic [cylinder set](../../../../../../cylinder-set.md) specifies finitely many coordinates. This is a [compact metric space](../../../../../../compact-metric-space.md), and $\mathcal L$ is a [homeomorphism](../../../../../../homeomorphism.md). Write $Y=\overline{\{\mathcal L^n c:n\geq0\}}$ for the forward [orbit closure](../../../../../../orbit-closure.md). A [minimal point](../../../../../../minimal-point.md) means that $Y$ is a [minimal dynamical system](../../../../../../minimal-dynamical-system.md), equivalently that every point of $Y$ has a dense forward [orbit](../../../../../../orbit-dynamical-system.md) in $Y$; it need not be a [fixed point](../../../../../../fixed-point.md).

There is a convention needed in the source: the bounded-gaps property concerns every **finite** [integer interval](../../../../../../integer-interval.md) $I$, hence every finite [word over an alphabet](../../../../../../string.md). Literally allowing $I=\mathbb Z$ would make the displayed condition impossible for finite $U$, although a constant coloring is a [minimal point](../../../../../../minimal-point.md). Under the standard finite-word interpretation, the property is precisely [uniform recurrence](../../../../../../uniform-recurrence.md).

Suppose first that $Y$ is a [minimal dynamical system](../../../../../../minimal-dynamical-system.md). Its nonempty compact forward-invariant [subset](../../../../../../subset.md) $\mathcal L(Y)$ must equal $Y$. As the ambient [left shift](../../../../../../left-shift.md) is invertible, all [integer](../../../../../../integer.md) translates of $c$ belong to $Y$. Let $I=[a,b]\cap\mathbb Z$ have length $\ell=b-a+1$, and let $V=\{z\in Y:z|_I=c|_I\}$. This is a nonempty [clopen set](../../../../../../clopen-set.md). Each forward [orbit](../../../../../../orbit-dynamical-system.md) in $Y$ meets $V$, so $\{\mathcal L^{-n}V:n\geq0\}$ covers $Y$. By [compactness](../../../../../../compact-space.md), finitely many suffice; let $D$ be the largest index in this finite cover. For any [integer](../../../../../../integer.md) $u$, the point $\mathcal L^{u-a}c$ lies in $Y$, so some $0\leq n\leq D$ satisfies $\mathcal L^{u-a+n}c\in V$. The prescribed word therefore occurs at positions $[u+n,u+n+\ell-1]$, entirely inside $[u,u+D+\ell-1]$. Taking $M=D+\ell$ proves the bounded-gaps property for every interval of length at least $M$.

Conversely suppose $c$ is [uniformly recurrent](../../../../../../uniform-recurrence.md). Every finite word from any [integer](../../../../../../integer.md) translate of $c$ occurs arbitrarily far to the right, so every such translate belongs to $Y$. Moreover, the property that every length-$M$ block contains a specified word of $c$ passes to every $z\in Y$: a finite block of $z$ is a limit of blocks of forward translates of $c$, and the finite discrete [alphabet](../../../../../../alphabet.md) forces eventual exact agreement on that block. Given $I=[a,b]\cap\mathbb Z$, look for its word inside $z([a,a+M-1])$. An occurrence starts at $a+n$ for some $n\geq0$, so $\mathcal L^n z$ agrees with $c$ on $I$. Taking $I=[-r,r]\cap\mathbb Z$ for arbitrarily large $r$ proves that $c$ belongs to the forward [orbit closure](../../../../../../orbit-closure.md) of every $z\in Y$. That [closure](../../../../../../closure-topology.md) is a closed forward-invariant [subset](../../../../../../subset.md) of $Y$, so it also contains every forward translate of $c$ and hence all of $Y$. Every forward [orbit](../../../../../../orbit-dynamical-system.md) is therefore dense in $Y$, proving

$$
\boxed{c\text{ is a minimal point}\iff c\text{ is uniformly recurrent}.}
$$

The same conclusion holds if [orbit closure](../../../../../../orbit-closure.md) is defined using all [integer](../../../../../../integer.md) iterates: the bounded-gaps condition makes the forward and two-sided closures equal.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
