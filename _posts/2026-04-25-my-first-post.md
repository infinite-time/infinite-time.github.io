---
layout: post
title: "Test Post"
date: 2026-04-25
---
$$
E = mc^2
$$
These learnings are based on Dwarkesh's [podcast episode](https://www.youtube.com/watch?v=Hrbq66XqtCo) with Jensen Huang.

## Part-1

### AI commoditizing software

Consider the below elements-

- As AI is lowering the barrier to entry for building software, does it imply that AI will commoditize software?

- Nvidia arrives at the design of the GPUs and prepares a GDS file to describe the physical layout of the chip. This [GDS2](#gds-2) file is provided to TSMC who builds the corresponding chip which includes the switch and the memory interface ([HBM](#hbm)). This is provided to [ODMs](#odm) to assemble into racks. So, Nvidia's description of the physical layout of the chip (GDS2 file) eventually gets translated into chips assembled into racks.

- This can be seen as equivalent to Nvidia providing software using which others manufacture hardware. 

Does this mean Nvidia may get commoditized?

- The transformation of electrons and tokens and making those tokens valuable is hard to completely commoditize. That is because the engineering, science, artistry and innovation behind making tokens valuable is not yet deeply understood.

- Nvidia continues to work to make this transformation more efficient. They do as much as necessary and "as little as possible" to make this transformation done incredibly. Here "as little as possible" means Nvidia's approach of identifying whatever they don't need to do and partner with others and make them part of the ecosystem. The part that Nvidia has to do is hard.

- [AI is a five layer cake](https://blogs.nvidia.com/blog/ai-5-layer-cake/) and Nvidia has ecosystems of partners across all the five layers.

So, it is very difficult to commoditize what Nvidia does.

Will AI commoditize software?

- Most software companies are tools makers. Ex: excel, powerpoint, compiler etc.

- The number of AI agents will continue to grow (and agents use tools) and this implies that the number of instances of the tools is going to grow as well.

### NVIDIA's purchase commitments

Nvidia's latest SEC filings show $100  Billion purchase commitments with foundries, memory and packaging. Does this mean that Nvidia's moat is that they have locked up many years of these scarce resources?

- Jensen Huang meets the CEOs of the upstream companies and discusses his views and reasons through clearly. 

- Upstream companies trust Nvidia's capacity to buy their supply and sell it to through their downstreams. An, this downstream is large.

- Nvidia brings their upstreams and downstreams together in GTC so that everybody can get a full view of the advances in AI. This helps the supply chain to see what Jensen would have talked to them about the AI universe.

- Jensen makes use of the GTC keynote to not only make announcements but to make sure that everybody understands what is the future and how big it is going to be by reasoning systematically.

- **Nvidia'a moat is they are able to build for the future.**

#### Nvidia's growth
- Revenue doubling year-over-year
- The processing speed of the Nvidia GPUs combined with the number of GPUs they are delivering is tripling year-over-year. This can be simplified as tripling the amount of FLOPS delivered.
*FLOPs delivered = factor of (processing speed of GPU, number of GPUs delivered)*

- Nvidia is-
  - the biggest customer on TSMCs [N3](#n3) node
  - one of the biggest customers on [N2](#n2) node
- AI will be 86% of N3 in 2027

#### Questions to think-
- How will Nvidia continue to doube the revenue year-over-year when it is the biggest customer?
- With this growth, how can the upstreams keep up?

#### Answers to the above questions across multiple axis-
##### Demand and supply
This growth means the instantaneous demand is greater than the supply. This is limited by the number of plumbers. Here 'plumbers' refers to the companies who work to setup the compute infrastructure by building data centers (GPUs, servers, wires, racks, network, cooling systems).

Example:
At one point, the instantaneous demand for [CoWoS](#cowos) was  higher than supply. TSMC continued to rapidly scale up CoWoS supply to keep up with the rest of the demands on logic and memory. Now, CoWoS is not just a speciality, it is part of the mainstream computing technology.

##### Influencing supply chain
Nvidia's ability to influence its supply chain is very good.
Example: Jensen and Sanjay's discussions on the future of AI and how Micron invested in [LPDDR](#lpddr) and [HBM](#hbm) memories.

##### Prefetching the bottlenecks
Systematically anticipate potential future bottlenecks and prepare from today to be ready for that.
Example:
Nvidia's investments in companies working on optical communication components (silicon photonics) - [Lumentum](https://www.lumentum.com/en), [Coherent](https://www.coherent.com/).

##### Technology inventions
Nvidia partnered with TSMC on [COUPE](#coupe) and invented new technologies and licensed those patents to the supply chain.

##### Manufacturing chips
To double the manufacturing of logic and memory chips, we need double the EUV machines. Nvidia is able to convince TSMC and ASML to invest in scaling up manufacturing.

##### Computing efficiency
In addition to increasing the manufacturing capacity, it is essental to improve the efficiency of computing. Nvidia GPU architecture and algorithms are significantly improving in terms of efficiency Compute efficiency increased 30x to 50x from [Hopper](https://www.nvidia.com/en-us/data-center/technologies/hopper-architecture/) to [Blackwell](https://www.nvidia.com/en-us/data-center/technologies/blackwell-architecture/). 

#### Constraint to this growth
Increasing manufacturing, building AI factories imply that energy consumption will significantly increase. Need ways of sustainable ways of producing more energy.

### TPUs and GPUs

#### Key differences
- Some AI models - Claude and Gemini were trained in [TPU](#tpu).
- TPU was built with a specific objective of accelerating neural network computations. GPU is built for accelerating general purpose paralle computing. So, GPUs have more broader usage.
- Companies which have home-built systems like TPU based systems need to provide the ability to operate as well as they are not meant for general operators.
- GPUs can be operated by anyone and are available on all Cloud providers.

#### Growth in AI
- AI technology is growing very fast. This needs accelerated parallel computing provided by Nvidia GPUs. Though GPUs are general purpose, as of now the mian driver of revenue is AI.
- TPUs are good for doing matrix multiplications.
- GPUs are more flexible and good when there are lots of branching and irregular memory accesses.
- the main use case for compute now is matrix multiplications in AI and AI is growing very fast. Doesn't it fit well with what TPU is built for?




### Key concepts

<a name="gds-2"></a>
**GDS2** - is the binary file format for capturing and exchanging the physical layout description of IC (integrated circuit).

<a name="hbm"></a>
HBM - High Bandwidth Memory is a memory interface for 3D stacked Synchronous Dynamic Random Access Memory.

<a name="odm"></a>
ODM - Original Design Manufacturer. They design and manufacture products which are bough and sold by other companies.

<a name="n3"></a>
N3 - 3nm MOSFET technology.

<a name="n2"></a>
N2 - 2nm MOSFET technology.

<a name="cowos"></a>
CoWoS - Circuit on Wafer on Substrate is a packaging technlogy developed by TSMC. It is about how different chips (compute, memory) are assembled together into a high performance unit.

<a name="lpddr"></a>
LPDDR - Low Power Double Data Rate is a type of synchronous dynamic random access memory optimized for lower power consumption than conventional memory.

<a name="euv"></a>
EUV - Extreme UltraViolet Lithography is a technology used for manufacturing integrated circuits.

<a name ="tpu"></a>
TPU - Tensor Processing Unit is [ASIC](#asic) developed by Google for neural networks.
TPUs and GPUs are built to accelerate computation.
- TPUS - for neural network related computation
- GPUs - for general purpose parallel computing.

<a name="asic"></a>
ASIC - Application Specific Integrated Circuit is an integrated chip customized for a specififc use.

<a name="cuda"></a>
CUDA - Compute Unified Device Architecture is a platform and programming model that enables one to use GPUs for general purpose computing.




