# 👋 Hi, I'm Amari

I’m a systems and backend engineer who loves working close to the metal.  
My GitHub is a mix of **low-level systems contributions** and **backend tooling in Go**.  
I enjoy solving problems where performance, correctness, and design all collide.

---

## 🚀 Notable Contributions

### 🔧 [snmalloc](https://github.com/microsoft/snmalloc) – High-performance allocator (Microsoft Research)
- **Contribution**: [PR #336](https://github.com/microsoft/snmalloc/pull/336)  
  - Rewrote the Apple PAL to use **native BSD and Mach APIs** to achieve Windows feature parity.  
  - Fixed App Store compliance issues by replacing `getentropy` with `SecRandomCopyBytes`.  
  - Rewrote semantics so that memory usage patterns were expressed to the XNU kernel, enabling proper reclamation of unused memory.  
  - Investigated decommit semantics and the 4 GiB kernel limit in XNU through a **deep-dive analysis of the kernel source (via Sourcegraph)**.  
- **Impact**: Brought Apple platform support to **parity with Windows allocator features**, improving reliability, security compliance, and long-term maintainability.

---

### 📚 [intrusive-rs](https://github.com/Amanieu/intrusive-rs) – Intrusive collections for Rust
- **Contribution**: [PR #46](https://github.com/Amanieu/intrusive-rs/pull/46)  
  - With the maintainer’s oversight, I **rewrote the library’s core architecture** to support **generic reference types**.  
  - Introduced `LinkOps` and `PointerOps` traits to decouple collection logic from raw pointers.  
  - Enabled collections to work with `Box`, `Rc`, `Arc`, `UnsafeRef`, and custom pointer types.  
  - Reduced code bloat and compile times by making core algorithms generic over `LinkOps`.  
- **Impact**: My rewrite reshaped nearly every major module, creating a more flexible, ergonomic, and safe foundation for intrusive collections in Rust — inspired by Boost.Intrusive but adapted to Rust’s type system.

---

### 🛠️ [bazelbuild/platforms](https://github.com/bazelbuild/platforms) – Bazel platform definitions
- **Contribution**: [PR #97](https://github.com/bazelbuild/platforms/pull/97)  
  - Added a new OS constraint `@platforms//os:uefi` to support UEFI firmware targets.  
  - Motivated by work on a **type‑1 hypervisor**, where we needed to build freestanding ELF binaries for UEFI.  
  - Coordinated with changes in `rules_rust` and `rules_go` so toolchains could properly target UEFI.  
- **Impact**: Enabled clean, upstream support for UEFI in Bazel’s platform model, unblocking Rust and C++ projects that target firmware and hypervisors.

---

## 🛠️ Original Projects

### [fxevent-zerolog](https://github.com/amari/fxevent-zerolog)
A lightweight adapter for using `zerolog` with Uber’s Fx framework.  
- Clean integration between structured logging and dependency injection.  
- Includes examples and benchmarks.  

### [cleta](https://github.com/amari/cleta) *(archived)*
A cloud metadata server written in Go.  
- Experiment in building a cloud-init server.

---

## 🌟 What I’m Building Next
- A Ceph-like Storage System

---

## 📫 Let’s Connect
- [GitHub](https://github.com/amari)  

---

⭐️ *Pinned repos highlight both my original work and my contributions to major open-source projects.*
