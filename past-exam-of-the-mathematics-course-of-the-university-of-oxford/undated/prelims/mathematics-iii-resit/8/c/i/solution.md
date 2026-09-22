<h1 id="8/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

With two distinct [centroids](../../../../../../../centroid.md), [K-means clustering](../../../../../../../k-means-clustering.md) assigns points on opposite sides of their [nearest-centroid decision hyperplane](../../../../../../../nearest-centroid-decision-hyperplane.md), which in two dimensions is a straight [line](../../../../../../../straight-line.md). This constraint explains the typical outcomes in the three source plots; exact assignments depend on initialization and the realized points.

**Dataset A:** one [cluster in cluster analysis](../../../../../../../cluster-in-cluster-analysis.md) contains most of the horizontal cloud and the bottom of the vertical cloud; the other contains the upper part of the vertical cloud. The two visually elongated groups are poorly matched to squared [Euclidean distance](../../../../../../../euclidean-distance.md) from their [centroids](../../../../../../../centroid.md). Points at the lower end of the vertical group can be closer to the horizontal group's [centroid](../../../../../../../centroid.md), so the two original shapes need not be recovered intact.

**Dataset B:** a roughly straight cut divides the ring and generally the central cloud between the two [clusters in cluster analysis](../../../../../../../cluster-in-cluster-analysis.md). A [Voronoi cell](../../../../../../../voronoi-cell.md) for either [centroid](../../../../../../../centroid.md) is a [half-plane](../../../../../../../half-plane.md); it cannot select a surrounding ring while excluding its center. The cut's direction can vary because the geometry is approximately rotationally symmetric.

**Dataset C:** the two dense lower clouds typically receive different [centroids](../../../../../../../centroid.md). The much smaller upper cloud is absorbed into one or divided between both [clusters in cluster analysis](../../../../../../../cluster-in-cluster-analysis.md), according to the nearly vertical separating [line](../../../../../../../straight-line.md). With $K=2$, the objective usually benefits more from separating the two large clouds than from spending one [centroid](../../../../../../../centroid.md) on the sparse third group. These are typical qualitative outcomes, rather than guarantees about every initialization.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [8](../../../8.md)
4. [Mathematics III resit](../../../../mathematics-iii-resit-split.md)
5. [Prelims](../../../../split.md)
6. [Undated](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
