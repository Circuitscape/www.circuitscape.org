+++
title = "Circuitscape"
+++

~~~
<p><img src="/assets/img/banner.png" alt="Circuitscape banner" /></p>
<p><img style="float: right; height: 267px; padding: 2px;" src="/assets/img/sa_sb2.jpg" alt="Circuitscape connectivity analysis example" /></p>
~~~

This site is home to [Circuitscape](/), [Omniscape](https://docs.circuitscape.org/Omniscape.jl/latest/), and [Gnarly Landscape Utilities](/gnarly-landscape-utilities/). LinkageMapper has now been moved to [its own website](https://linkagemapper.org/). All are free and open source. Circuitscape borrows algorithms from electronic circuit theory to predict connectivity in heterogeneous landscapes. Omniscape offers a “coreless” approach by applying Circuitscape iteratively in a moving window to predict omni-directional connectivity. Linkage Mapper uses least-cost corridor analysis, circuit theory, and barrier analysis to map corridors, detect pinch-points and restoration opportunities within them, and identify important core areas and corridors. Gnarly Landscape Utilities automates the creation of core area maps and resistance layers needed for connectivity modeling.

Click [here](/applications/) for a list of applications using Circuitscape. See the tabs above for more info, downloads, and other connectivity modeling tools and resources.

## Get Started with Circuitscape 5

Circuitscape 5 is written in [Julia](https://julialang.org) and delivers major performance improvements. Install it with:

```julia
using Pkg
Pkg.add(“Circuitscape”)
```

See the [documentation](https://docs.circuitscape.org/Circuitscape.jl/latest/) for usage instructions, or visit the [GitHub repository](https://github.com/Circuitscape/Circuitscape.jl) for source code and issue tracking.

## Authors

**Circuitscape was created by [Brad McRae](https://blog.nature.org/science/2018/04/26/innovation-for-conservation-brad-mcrae-1966-2017/) (1966-2017), Viral Shah, Tanmay Mohapatra, and Ranjan Anantharaman.** Brad's vision and dedication to conservation science continue to inspire the project. More details about the authors [**here**](/authors/).

## Acknowledgments

We are especially grateful to [NASA](https://appliedsciences.nasa.gov/) and [The Nature Conservancy](https://www.nature.org) for Circuitscape 5.0, a major upgrade to Circuitscape using the Julia language. The [Wilburforce Foundation](https://www.wilburforce.org/) funded [Circuitscape 4.0](/downloads/) and the Python version of Circuitscape. The [Cougar Fund](https://www.cougarfund.org/) also contributed to the original development. We also wish to thank the Washington Program of The Nature Conservancy and the [National Center for Ecological Analysis and Synthesis](https://www.nceas.ucsb.edu/) for supporting Brad McRae and the [University of California, Santa Barbara](https://www.ucsb.edu/) for supporting Viral Shah while they collaborated on the project.
