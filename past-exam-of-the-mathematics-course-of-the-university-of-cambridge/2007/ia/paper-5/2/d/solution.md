<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Set-user-ID execution](../../../../../../set-user-id-execution.md) of a suitable executable makes its effective user identity that of the owner. When that owner is root, running it can give root privileges even to an otherwise unprivileged caller. World-write permission destroys the trust boundary: any user can alter the privileged executable, potentially substituting code which performs arbitrary privileged operations. World-execute permission then makes the compromised program available to everyone.

World-read access can reveal implementation details or embedded secrets, but reading alone is not the decisive privilege-escalation flaw; properly designed public set-user-ID utilities need not keep their code secret. Some Unix kernels clear the set-user-ID bit after an unprivileged modification. That is a mitigation, not a reason to maintain a world-writable privileged program: if the bit persists or is restored without validating the changed code, the privilege escalation remains. **Root-owned privileged executables must not be writable by untrusted users.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
