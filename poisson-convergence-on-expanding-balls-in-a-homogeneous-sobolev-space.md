# Poisson convergence on expanding balls in a homogeneous Sobolev space

↑ **Parent:** [Homogeneous Sobolev space](homogeneous-sobolev-space.md)

In three dimensions let $f\in L^{6/5}(\mathbb R^3)$ have [compact support](compact-support.md). Let $v_R\in H_0^1(B_R)$ solve $-\Delta v_R=f$ and extend it by zero. There is a unique $v\in\dot H^1(\mathbb R^3)$ with $\int\nabla v\cdot\nabla\phi=\int f\phi$ for all $\phi\in\dot H^1$. Indeed [Holder inequality](holder-inequality.md) and the homogeneous [Sobolev inequality](sobolev-inequality.md) make the right side a continuous [linear functional](linear-functional.md) in the [gradient](gradient.md) [norm](norm.md), and the [Riesz representation theorem](riesz-representation-theorem.md) applies to this [Hilbert space](hilbert-space-split.md).

The [weak formulation](weak-formulation.md) says that $v_R$ is the [orthogonal projection](orthogonal-projection.md) of $v$ onto the closed subspace consisting of zero extensions of $H_0^1(B_R)$. These subspaces increase with $R$ and their union contains every [test function](test-function.md), which is dense by the definition of the [homogeneous Sobolev space](homogeneous-sobolev-space.md). The best-approximation property of [orthogonal projection](orthogonal-projection.md) therefore gives $\|\nabla(v_R-v)\|_2\to0$. The homogeneous [Sobolev inequality](sobolev-inequality.md) also gives $\|v_R-v\|_6\to0$. This convergence does not generally extend to the inhomogeneous [Sobolev space](sobolev-space-split.md) $H^1$, as the [spherical mean of a Poisson solution outside its source](spherical-mean-of-a-poisson-solution-outside-its-source.md) shows for a source of nonzero total mass.

## ↑ Ancestors (7)

1. [Homogeneous Sobolev space](homogeneous-sobolev-space.md)
2. [Sobolev space](sobolev-space-split.md)
3. [Functional analysis](functional-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-functional-analytic-methods-for-partial-differential-equations-course-of-the-university-of-oxford/2023/3/b/iv/solution.md)
