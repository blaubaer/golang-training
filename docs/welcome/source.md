class: center, middle

# Golang Training

## Welcome to Golang!

???
Some note.

---

layout: true

.headline[Golang Training · Welcome!]

---

# What is Golang?

* It is a programming language. ;-)
* It will be directly translated to target machine code.
  * Similar to _C_, _C++_ and _Rust_
  * But in contrast to _PHP_ and _JavaScript_ which is interpreted at runtime
  * And in contrast to _Java_ and _C#_ which is translated to VM code and at runtime interpreted.
* The built result will shipped always shipped as executable .reference[1)]

.footnote[1) Some exceptions included]

---

# What are the dependencies, at build time?

1. A Golang SDK
   * Could be downloaded from [golang.org/dl](https://golang.org/dl/)
   * Available for Linux, FreeBSD, macOS .hint[(darwin)] and Windows

That's it!

---

# Why is not more required at build time? .reference[1)]

* Golang is always build from sources; this includes:
  * Everything in the SDK itself
  * and every included library .reference[2)]
* All dependencies are hosted via Git, SVN, Bazaar repositions
* Golang will download all required dependencies at build time automatically (if required)
* Golang can compile and like itself without need of platform tools of Linux or Windows

.footnote[1) If [Go Modules](https://github.com/golang/go/wiki/Modules) is enabled which are available from Go 1.11 on - this is highly recommended]
.footnote[2) Exceptions are possible if in extreme rare situations are static libraries are used]

---

# What are the runtime dependencies?

* Everything is s
* Usually really nothing!
*
* If build with `CGO_ENABLED=0`
* And
