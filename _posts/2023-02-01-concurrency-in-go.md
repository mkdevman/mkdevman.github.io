---
title:  "Concurrency in Go "
layout: post
---

Before getting into the how and why, let’s briefly cover the what. There are two primary elements of Go’s concurrency model:

* Goroutines
* Channels
A Goroutine is a concurrent thread of execution. Compared to traditional threads, goroutines are computationally much cheaper to utilize. They have much faster startup times and take up minimal space on the stack. To spawn a new goroutine, you simply precede a function call with the keyword go.
