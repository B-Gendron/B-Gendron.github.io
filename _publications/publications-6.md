---
layout: archive
title: "Bridging Symbolic Knowledge and Neural Text Generation: Ontology-Driven Conversational Control of LLMs"
collection: publications
---

## Abstract

This work investigates ontology-driven control of LLM-based conversational agents. Key conversational properties are defined in an ontology, complemented by a rule-based strategy specifying when agent utterances must satisfy predefined constraints. An initial LLM–ontology hybrid architecture enabled systematic control of English CEFR levels [1] through a simple strategy [2]. Since then, characteristics other than language level alone have been represented in the ontology, now covering three aspects of control. This allows us to test different fine-tuning scenarios by controlling a single aspect at a time (single-aspect) or several aspects (multi-aspect). To achieve conversational control that has a greater impact on LLM generation, I explored fine-tuning procedures based on reinforcement learning, typically using the GRPO algorithm [3]. The latter has significantly improved results in single-aspect controlled generation, while multi-aspect generation control appears to be a much more demanding task. This ontology-driven conversational control has been implemented in a conversational agent for the experimental use case of job interview practise. As part of my visit to DPKM, I am extending this framework to a complex real-world application: the development of a conversational agent to support ontology engineering. This involves regulating both the factual content and the stylistic dimensions of the interaction, thereby providing a substantial extension of the current control setup.

---

**References**

[1] Council of Europe. [Common European Framework of Reference for Languages (CEFR) – Level Descriptions.](https://www.coe.int/en/web/common-european-framework-reference-languages/level-descriptions)  

[2] Barbara Gendron, Gaël Guibon, Mathieu d’Aquin. [Towards Ontology-Based Descriptions of Conversations with Qualitatively-Defined Concepts.](https://arxiv.org/abs/2509.04926) TOTh International Conference, 2025.  

[3] Shao, Z., Wang, P., Zhu, Q., Xu, R., Song, J., Bi, X., Zhang, H., Zhang, M., Li, Y.K., Wu, Y., Guo, D. (2024). [Deepseekmath: Pushing the limits of mathematical reasoning in open language models.](https://arxiv.org/abs/2402.03300)