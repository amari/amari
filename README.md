# 👋 Hi, I’m Amari  

**Systems & Backend Engineer**

I live where performance, correctness, and design collide.  
I thrive on low‑level systems work, backend tooling, and solving problems close to the metal.  

---

## 🚀 Notable Contributions  

### 🔧 [snmalloc (Microsoft Research)](https://github.com/microsoft/snmalloc/pull/336)  
**Impact:** Brought Apple allocator support to Windows parity, improving reliability, security compliance, and long‑term maintainability.  
- Rewrote the Apple PAL with native BSD & Mach APIs  
- Fixed App Store compliance issues  
- Enabled proper kernel reclamation by expressing memory usage patterns to XNU  
- Investigated decommit semantics & the 4 GiB kernel limit in XNU  

---

### 📚 [intrusive-rs](https://github.com/Amanieu/intrusive-rs/pull/46)  
**Impact:** Made the library easier to extend to new data structures while improving flexibility, ergonomics, and safety.  
- Rewrote the core architecture with `LinkOps` & `PointerOps` traits  
- Decoupled collection logic from raw pointers  
- Enabled collections to work with `Box`, `Rc`, `Arc`, `UnsafeRef`, and custom pointer types  
- Reduced code bloat & compile times with generic algorithms  

---

### 🛠️ [bazelbuild/platforms](https://github.com/bazelbuild/platforms/pull/97)  
**Impact:** Enabled upstream support for UEFI in Bazel’s platform model, unblocking Rust & C++ firmware/hypervisor projects.  
- Added new OS constraint `@platforms//os:uefi`  
- Coordinated with `rules_rust` and `rules_go` for toolchain compatibility  
- Motivated by work on a type‑1 hypervisor targeting freestanding ELF binaries  

---

## 🛠️ Original Projects  

- **[fxevent-zerolog](https://github.com/yourusername/fxevent-zerolog)**  
  Adapter for using `zerolog` with Uber’s Fx framework.  
  - Clean integration between structured logging & dependency injection  
  - Includes examples & benchmarks  

- **cleta (archived)**  
  Cloud metadata server — an experiment in building a cloud‑init server.  

---

## 🌟 What I’m Building Next  

### **Mithril** — a Ceph‑like distributed storage system  
Inspired by **Meta’s Tectonic**, but focused squarely in Ceph’s niche.  

- **mithrild** — the storage daemon  
- **mithril library** — client/integration library  

**Roadmap:**  
- **Current focus:** rapid development to validate design and cluster behavior  
- **Planned evolution:** transition to a shared‑nothing architecture and integration with advanced I/O frameworks (**DPDK**, **SPDK**, **io_uring**) to maximize efficiency and eliminate runtime overheads  

---

## 📫 Let’s Connect  

- [Website](https://amari.codes)  
- [GitHub](https://github.com/yourusername)  

⭐️ Check out my pinned repos for both original work and major open‑source contributions.  
