[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pnavaro/ParallelWorkshop2019/master)

To convert these julia files to notebooks, use [jupytext](https://jupytext.readthedocs.io/en/latest/using-cli.html)

```bash
jupytext --to ipynb *.jl 
```


# JuliaCon 2019 Parallel Computing Workshop

This workshop will cover:

* Introduction to parallelism
    * What is happening to our computers?

* Parallelism strategies
    * SIMD and best single-core performance (brief overview)
    * Multi-threading (hands on)
    * Cooperative multi-tasking
    * Parallel algorithm design
    * Multi-process (hands on)
        * Shared memory
        * Distributed memory
    * GPU programming

* Challenges of parallel computing
    * Order of execution
        * execution of out order of Possibility
        * race conditions with simultaneous access and mutation
    * Data access and movement
    * Code access and movement
    * Appropriately matching the parallelism strategy to your machine capabilities
    * Appropriately matching the parallelism strategy with the problem at hand

## What is happening to our computers!?

![](https://raw.githubusercontent.com/JuliaComputing/JuliaAcademyData.jl/master/courses/Parallel_Computing/images/40-years-processor-trend.png)

Not only have we gained multiple cores, but processors have become extremely
complex, with multiple levels of caches, pipelines, predictions, speculations...

## What is hard about parallel computing
  * We don't think in parallel
  * We learn to write and reason about programs serially
  * The desire for parallelism often comes _after_ you've written your algorithm (and found it too slow!)

## Summary:
  * Current computer archetectures push us towards parallel programming for peak performance — even if we're not on a cluster!
  * But it's hard to design good parallel algorithms
  * And it's hard to express and reason about those algorithms

---

*This page was generated using [Literate.jl](https://github.com/fredrikekre/Literate.jl).*

