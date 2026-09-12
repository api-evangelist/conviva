---
title: "We Replaced mmap with io_uring in Our Rust Query Engine. It Got Slower."
url: "https://www.conviva.ai/resource/we-replaced-mmap-with-io_uring-in-our-rust-query-engine-it-got-slower/"
date: "2026-09-01"
author: "Melissa Pieroni"
feed_url: "https://www.conviva.ai/feed/"
---
In the beginning, there was mmap. It was convenient: it let us lazily read huge numbers of Arrow IPC files from disk without managing memory ourselves. It fit our file format perfectly — Arrow IPC’s layout is designed for zero-copy random access, and mmap gives you exactly that.
