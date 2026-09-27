# MÖBIUS LAB

### Independent Systems Research · Low-Latency Computing · Secure Interfaces · Physical AI

I design and test computing systems from first principles.

My work focuses on building compact, verifiable architectures across software, hardware, control, and AI infrastructure — while keeping proprietary research isolated from the public surface.

---

## Research Focus

- Low-latency systems architecture
- Secure C ABI and isolation boundaries
- Reproducible and verifiable software builds
- Hardware / software co-design
- AI infrastructure and inference systems
- Robotics and Physical AI
- Control systems and digital twins
- Semiconductor and computing architecture research
- Experimental system design

---

## Public Engineering Principle

Most core research remains private.

The public layer is intentionally small and designed to expose:

- interfaces
- contracts
- tests
- reproducible measurements
- verification evidence

without exposing proprietary algorithms or internal architecture.

```text
Private Research Core
        │
        │  proprietary implementation remains private
        ▼
Isolation Boundary
        │
        ▼
Minimal Public Interface
        │
        ▼
Tests · Benchmarks · Verification

Expose proofs, interfaces, and reproducible measurements — not the core implementation.
Current Public Project
MOBIUS-BRIDGE
A minimal public interface layer for isolated ABI, benchmark, and verification testing.
The current public baseline includes:
C11 ABI contract
minimal 3-symbol exported interface
strict input and buffer semantics
boundary-condition testing
overlapping-buffer validation
insufficient-buffer preservation checks
ASan / UBSan testing
hardened Linux release builds
RELRO / immediate binding / non-executable stack checks
runtime dependency allowlisting
forbidden capability import checks
RPATH / RUNPATH rejection
TEXTREL rejection
Git history leakage scanning
reproducible-build verification
SHA-256 artifact verification
signed build provenance / attestation
attestation verification before artifact publication
public ABI benchmark measurement
The benchmark measures only the public bridge and stub path.
It does not expose or represent proprietary engine internals.
Public / Private Boundary
PUBLIC
├── ABI contracts
├── verification tests
├── benchmark harnesses
├── reproducible build evidence
├── hardened public binaries
└── signed provenance

PRIVATE
├── proprietary algorithms
├── internal reasoning engines
├── architecture internals
├── private repositories
├── experimental control logic
└── unreleased research
The public surface intentionally represents only a very small fraction of the broader research program.
Engineering Direction
My systems work generally follows four principles:
Isolation
Critical implementation details should not cross unnecessary trust boundaries.
Verification
Claims should be supported by tests, reproducible builds, or measurable evidence.
Minimalism
Public interfaces should expose the smallest surface required for useful interaction.
Cross-Domain Design
Software, hardware, AI, control, and physical systems are treated as one engineering space rather than separate disciplines.
Current Status
Public research surface : v0.1
Public ABI              : stable experimental baseline
Verification pipeline   : active
Benchmark pipeline      : active
Core architecture       : private
MÖBIUS LAB
Independent research in computing architecture, AI systems, control, robotics, and verifiable infrastructure.
Build the boundary. Verify the evidence. Keep the core private.
