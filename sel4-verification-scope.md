# seL4 verification scope

↑ **Parent:** [seL4](sel4.md)

[Formal verification](formal-verification.md) uses machine-checked [formal proofs](formal-proof.md) to establish [functional correctness](functional-correctness.md): the C implementation of verified [seL4](sel4.md) configurations conforms to its [formal specification](formal-specification.md). [Binary correctness](binary-correctness.md) connects compiled machine code to that C behaviour where supported. Separate security [formal proofs](formal-proof.md) cover integrity, resource-access availability and confidentiality under their configuration requirements; these properties are not all available in every configuration. For example, the documented confidentiality theorem separates scheduler security domains rather than arbitrary pairs of [software threads](thread-computing.md). [seL4 Proofs, High-level Proof Statements: Functional correctness; Binary correctness; Security; System initialisation; platform/configuration qualification](sel4-proofs-by-sel4-project.md)

The documented assumptions include correct hardware, selected handwritten machine-interface code, correct boot state, [translation lookaside buffer](translation-lookaside-buffer.md) and [memory cache](cache-computing.md) management, and noninterfering or trusted [DMA](direct-memory-access.md). The confidentiality result covers information channels in its model; the assumptions page explicitly excludes timing channels from that coverage. [What the Proofs Assume, The Assumptions: Assembly, Hardware, Hardware management, Boot code, DMA, Information side-channels](what-the-proofs-assume-by-sel4-project.md)

Return to `READ(7, 9, 0, 4)`. Correct [IPC](inter-process-communication.md) delivery does not establish that the service looked up the right [file](computer-file.md), returned `LIME`, or ever replied. A service can produce an incorrect payload while the [operating-system kernel](kernel-operating-system.md) exactly follows its [formal specification](formal-specification.md). The [formal proofs](formal-proof.md) therefore do not automatically prove all [user-space services](user-space-service.md), nor turn the resource-access availability theorem into a guarantee that this [file](computer-file.md) read completes. The verified foundation supports further [algorithm correctness](algorithm-correctness.md) and system reasoning; the service protocol and its recovery obligations still need their own justification.

// Destination: computer-science.bigb

## ↑ Ancestors (6)

1. [seL4](sel4.md)
2. [Microkernel](microkernel.md)
3. [Kernel (operating system)](kernel-operating-system.md)
4. [Operating system](operating-system-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)
