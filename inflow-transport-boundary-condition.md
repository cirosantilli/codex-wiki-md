# Inflow transport boundary condition

↑ **Parent:** [Linear transport equation](linear-transport-equation.md)

For a [transport equation](transport-equation.md) on a domain, prescribe boundary data only where the velocity points into the domain. On $x>0$ with speed $a>0$, a bounded [weak solution](weak-solution.md) with initial data $u_0$ and inflow data $f$ satisfies

$$
\int u(\varphi_t+a\varphi_x)+\int u_0\varphi(0,x)+a\int f(t)\varphi(t,0)=0.
$$

The integrals are over the quadrant and its two boundary rays. Backtracking [characteristic curves](characteristic-curve.md) gives $u_0(x-at)$ when $x\ge at$ and $f(t-x/a)$ otherwise. Corner values need not match for a bounded [weak solution](weak-solution.md).

**Table of contents**

- [Corner compatibility for constant-speed transport](corner-compatibility-for-constant-speed-transport.md)

## ↑ Ancestors (7)

1. [Linear transport equation](linear-transport-equation.md)
2. [Transport equation](transport-equation.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-5/1/2/b/solution.md)
