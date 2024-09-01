---
title: "On the Robustness of Graph Reduction Against GNN Backdoor"
collection: publications
permalink: /publication/2024-07-02 On the Robustness of Graph Reduction Against GNN Backdoor
excerpt: "Yuxuan Zhu, Michael Mandulak, Kerui Wu, George Slota, Yuseok Jeon, Ka-Ho Chow, Lei Yu.<br/><img src='/images/graph.png'>"
date: 2024-07-02
venue: 'AISec 24: 17th ACM Workshop on Artificial Intelligence and Security'
paperurl: 'https://arxiv.org/abs/2407.02431'
# citation: 'Your Name, You. (2024). &quot;Paper Title Number 3.&quot; <i>GitHub Journal of Bugs</i>. 1(3).'
---

Graph Neural Networks (GNNs) are gaining popularity across various domains due to their effectiveness in learning graph-structured data. Nevertheless, they have been shown to be susceptible to backdoor poisoning attacks, which pose serious threats to real-world applications. Meanwhile, graph reduction techniques, including coarsening and sparsification, which have long been employed to improve the scalability of large graph computational tasks, have recently emerged as effective methods for accelerating GNN training on large-scale graphs. However, the current development and deployment of graph reduction techniques for large graphs overlook the potential risks of data poisoning attacks against GNNs. It is not yet clear how graph reduction interacts with existing backdoor attacks. This paper conducts a thorough examination of the robustness of graph reduction methods in scalable GNN training in the presence of state-of-the-art backdoor attacks. We performed a comprehensive robustness analysis across six coarsening methods and six sparsification methods for graph reduction, under three GNN backdoor attacks against three GNN architectures. Our findings indicate that the effectiveness of graph reduction methods in mitigating attack success rates varies significantly, with some methods even exacerbating the attacks. Through detailed analyses of triggers and poisoned nodes, we interpret our findings and enhance our understanding of how graph reduction influences robustness against backdoor attacks. These results highlight the critical need for incorporating robustness considerations in graph reduction for GNN training, ensuring that enhancements in computational efficiency do not compromise the security of GNN systems.
