
### Paper 1: Advancing Neuromorphic Computing With Loihi: A Survey of Results and Outlook

Authors: Mike Davies et al.

Year: 2021

Publication: Proceedings of the IEEE

#### Research Focus

This paper surveys Intel's Loihi neuromorphic research processor, its architecture, experimental results, applications, and future research opportunities.

#### Architecture

Loihi supports spiking neural networks through neuromorphic cores, neuron and synapse state, and event-based communication. Its design aims to exploit sparse activity and temporal information while supporting computation distributed across processing cores.

#### Key Findings

- Neuromorphic computing can offer substantial efficiency advantages for particular workloads.
- Performance depends on the algorithm, network architecture, activity patterns, hardware implementation, and baseline used for comparison.
- Some reported experiments demonstrate promising energy or latency advantages, but those results cannot automatically be generalized to all applications.
- Conventional feedforward neural networks do not necessarily benefit as much as architectures specifically designed to exploit neuromorphic hardware.

#### Limitations and Research Considerations

- Neuromorphic systems are not universally superior to conventional processors.
- Latency, throughput, network scale, communication overhead, and workload characteristics can affect the outcome.
- Comparisons must account for the hardware, software, and measurement methods used.
- Results from one platform or task should not be treated as proof of general superiority.

#### Relevance to This Project

This paper supports investigating the conditions under which event-driven computation is beneficial. It suggests that future experiments should examine computational cost, data movement, latency, and task performance together rather than treating energy efficiency as the only measure.

The findings also caution against assuming that every alternative architecture will outperform conventional neural networks.

#### Follow-up Questions

- Which workload characteristics make event-driven computation advantageous?
- How much overhead is introduced by communication and state management?
- Can the benefits of sparse computation be retained as the workload scales?
- How should experiments compare neuromorphic and conventional architectures fairly?

#### Source

Davies, M., et al. (2021). Advancing neuromorphic computing with Loihi: A survey of results and outlook. Proceedings of the IEEE.

DOI: https://doi.org/10.1109/JPROC.2021.3067593


### Paper 2: Managing Burstiness and Scalability in Event-Driven Models on the SpiNNaker Neuromimetic System

Authors: Rast et al.

Year: 2012 (published online in 2011)

#### Research Focus

This paper investigates the performance and scalability of event-driven neural simulations on the SpiNNaker architecture.

#### Architecture

SpiNNaker uses a parallel multiprocessor architecture with asynchronous, event-driven communication. Neural events are transmitted as packets between processors.

#### Key Findings

- Event-driven neural simulation can support large-scale neural models.
- Network traffic patterns, spatial locality, and temporal relationships affect performance.
- Bursty event traffic can create processor congestion and communication challenges.
- Effective event handling and network mapping are important for scalability.

#### Limitations and Research Considerations

The results highlight the importance of communication overhead and traffic management. Performance depends on the workload and how neural models are mapped onto the hardware.

#### Relevance to This Project

This paper helps investigate a key question: can event-driven computation reduce unnecessary work while avoiding excessive communication overhead?

It also provides a comparison point for other neuromorphic architectures, including Loihi.

#### Source

Rast, A. D., et al. (2012). Managing burstiness and scalability in event-driven models on the SpiNNaker neuromimetic system. International Journal of Parallel Programming, 40, 553–582.

DOI: https://doi.org/10.1007/s10766-011-0180-7
