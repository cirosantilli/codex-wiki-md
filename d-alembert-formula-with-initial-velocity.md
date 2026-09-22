<h1 id="d-alembert-formula-with-initial-velocity">D'Alembert formula with initial velocity</h1>

↑ **Parent:** [D'Alembert's formula](d-alembert-s-formula.md)

For the [wave equation](wave-equation-split.md) $u_{tt}=c^2u_{xx}$ with zero initial displacement and initial [velocity](velocity.md) $g$, [D'Alembert's formula](d-alembert-s-formula.md) becomes

$$
u(x,t)=\frac1{2c}\int_{x-ct}^{x+ct}g(s)\,ds.
$$

For $c=1$ this is the original speed-one form $u(t,x)=\tfrac12\int_{x-t}^{x+t}f(s)\,ds$ when the initial [velocity](velocity.md) is named $f$. The integral records the total initial kick inside the [domain of dependence](domain-of-dependence.md).

For a computed example, set $g(x)=V$ on $[-a,a]$ and zero elsewhere, with $V>0$. This discontinuous datum gives a [weak solution](weak-solution.md):

$$
u(x,t)=\frac{V}{2c}\,\operatorname{length}\bigl([x-ct,x+ct]\cap[-a,a]\bigr),\qquad t\geq0.
$$

At the centre, $u(0,t)=V\min(t,a/c)$. For $a=1\,\mathrm m$, $c=2\,\mathrm{m\,s^{-1}}$ and $V=0.4\,\mathrm{m\,s^{-1}}$, this is $0.1\,\mathrm m$ at $t=0.25\,\mathrm s$ and $0.2\,\mathrm m$ at $t=1\,\mathrm s$. Once $ct>a$, a central plateau $u=Va/c$ occupies $|x|\leq ct-a$. In contrast, [central zero region for odd compactly supported initial velocity](central-zero-region-for-odd-compactly-supported-initial-velocity.md) follows when the full integral of $g$ vanishes. [Finite propagation speed](finite-propagation-speed.md) permits an interior tail; it does not imply the [Strong Huygens principle](strong-huygens-principle.md).

**Table of contents**

- [Central zero region for odd compactly supported initial velocity](central-zero-region-for-odd-compactly-supported-initial-velocity.md)

## ↑ Ancestors (7)

1. [D'Alembert's formula](d-alembert-s-formula.md)
2. [Wave equation](wave-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Finite propagation speed](finite-propagation-speed.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/5b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-2/6b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-2/6a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3/14a/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-4/12b/iii/solution.md)
