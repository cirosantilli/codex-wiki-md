<h1 id="section-a-i/2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[AFM image flattening](../../../../../../afm-image-flattening.md) estimates an unwanted background and subtracts it from the recorded height:

$$
z_{\rm corrected}(x,y)=z_{\rm measured}(x,y)-b(x,y).
$$

A plane removes overall tilt; a line-by-line constant or low-order fit removes line offsets or curvature. **For a tip-change height jump, align the baselines of unchanged reference regions on either side of the event**, using a piecewise offset or appropriately masked line fits. A single global plane cannot in general remove an abrupt step.

Exclude genuine features from the fit, use the same terrace as a reference where possible, and retain the unprocessed data. The corrected image has a consistent relative background; it does not establish that the interaction [force](../../../../../../force-split.md), tip shape or absolute height calibration remained unchanged. In particular, flattening is a correction for the offset component of a [tip-change artefact](../../../../../../tip-change-artefact.md), not a repair of every consequence of a changed tip.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Section A(i)](../../../section-a-i.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../split.md)
7. [MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../../mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
