# References

## Research papers and articles

- [Current State of LLM Risks and AI Guardrails — Ayyamperumal and Ge (arXiv:2406.12934)](https://arxiv.org/pdf/2406.12934)
- [Artificial Intelligence in 6G Wireless Networks: Opportunities, Applications, and Challenges — Alhammadi et al. (2024)](https://onlinelibrary.wiley.com/doi/full/10.1155/2024/8845070)
- [The Roadmap to 6G: AI Empowered Wireless Networks — Letaief et al. (IEEE 8808168)](https://ieeexplore.ieee.org/abstract/document/8808168)
- [Does AI Need Guardrails? — Mulahuwaish et al., International Journal of Pervasive Computing and Communications](https://www.emerald.com/ijpcc/article-abstract/21/2/177/1240092/Does-AI-need-guardrails?redirectedFrom=fulltext)
- [AI-Native Network Controller: A Modular Framework for Safe Agentic Control of Multi-Domain Network Infrastructure — Dzaferagic (arXiv:2606.20565)](https://arxiv.org/pdf/2606.20565)
- [Big AI Models for 6G Wireless Networks: Opportunities, Challenges, and Research Directions](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10579546&tag=1)
- [Machine Learning for Wireless Networks with Artificial Intelligence: A Tutorial on Neural Networks — Chen et al. (PDF)](https://www.researchgate.net/profile/Samir-Touzani/post/Have_anyone_had_experience_in_Real_Time_Location_System_RTLS_for_Indoor_environment_such_as_supermarkets_and_applying_its_data_to_ML_and_AI/attachment/6169a07db3729f0f618c5f7b/AS%3A1079198231855104%401634312317507/download/Machine_Learning_for_Wireless_Networks_with_Artifi.pdf)
- [An SDN-Based Architecture for Next-Generation Wireless Networks — Wang et al. (IEEE 7864786)](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7864786)
- [Generative AI for the Optimization of Next-Generation Wireless Networks: Basics, State-of-the-Art, and Open Challenges](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10855897&tag=1)
- [AI-Assisted Network-Slicing Based Next-Generation Wireless Networks — Shen et al. (IEEE 8954683)](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8954683)

## Government guidance

- [DHS AI Safety and Security Guidelines for Critical Infrastructure (PDF)](https://www.dhs.gov/sites/default/files/2024-04/24_0426_dhs_ai-ci-safety-security-guidelines-508c.pdf)

## Paper link

- [Jump to the references list](#research-papers-and-articles)

## Notes from the pages

### AI Native Network Controller

*Exact paper: [AI-Native Network Controller](https://arxiv.org/abs/2606.20565).* The page title and notes about lightweight Python adapters and domain-specific control applications match its title and abstract.

Network elements are handled through lightweight Python adapters, while domain-specific control applications provide structured tools that AI agents can invoke safely.

Directly exposing critical infrastructure to autonomous decision-making introduces unexpected safety risks.

The notes mention starting with deep reinforcement learning for resource allocation and network optimization, then moving to large language models. *(The exact wording here is unclear.)*

**Command validation:** A mechanism in the main safety layer. It does not matter where a command comes from: an app, REST API, or agent.

With a conflict detector, AI can ask the registration plane which apps are active and what they control. It can:

- Check for conflicting objectives between apps.
- Coordinate between apps by adjusting states or parameters.
- Reason about the global network state across domains.

### Current State of LLM Risks and AI Guardrails

*Exact paper: [Current State of LLM Risks and AI Guardrails](https://arxiv.org/abs/2406.12934).* The page title matches this arXiv paper. The notes say effective guardrail design requires a deep understanding of an LLM's intended use case, relevant regulations, and ethical considerations. They also say, “no idea how many parameters, similar to first paper,” and “Do some testing.”

### Does AI Need Guardrails?

*Related paper: [“Does AI need guardrails?”](https://www.emerald.com/ijpcc/article-abstract/21/2/177/1240092/Does-AI-need-guardrails?redirectedFrom=fulltext).*

The notes describe AI as a black box because users cannot see what happens inside the model or how it makes decisions. *(The phrase after this point is unclear.)*

AI models do not make predictions with 100% confidence, as their understanding is just based purely on statistics. This is where human-in-the-loop AI comes into play: when AI encounters a problem it cannot solve, a human intervenes, creating a feedback loop that allows the model to learn and improve.

In critical decision-making, it can be important to know how AI arrived at a decision, such as in medical diagnosis or court decisions.

Privacy and security in AI are major issues. Passing confidential information to an agentic AI could result in that information being shared elsewhere.

The notes suggest encrypting data before analysis, anonymizing it, or removing identifying or confidential information. These methods may be computationally inefficient or remove valuable information, but the notes say this is important for AI in wireless networks.

Data masking, pseudonymization, generalization, data perturbation, and data swapping are listed. The notes also suggest trying federated learning and split learning.
