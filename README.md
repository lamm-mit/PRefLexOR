# PRefLexOR
Preference-based Recursive Language Modeling for Exploratory Optimization of Reasoning

We introduce PRefLexOR (Preference-based Recursive Language Modeling for Exploratory Optimization of Reasoning), a framework that combines preference optimization with concepts from Reinforcement Learning (RL) to enable models to self-teach through iterative reasoning improvements. Central to PRefLexOR are thinking tokens, which explicitly mark reflective reasoning phases within model outputs, allowing the model to recursively engage in multi-step reasoning, revisiting, and refining intermediate steps before producing a final output. The foundation of PRefLexOR lies in Odds Ratio Preference Optimization (ORPO), where the model learns to align its reasoning with human-preferred decision paths by optimizing the log odds between preferred and non-preferred responses. The integration of Direct Preference Optimization (DPO) further enhances model performance by using rejection sampling to fine-tune reasoning quality, ensuring nuanced preference alignment. This hybrid approach between ORPO and DPO mirrors key aspects of RL, where the model is continuously guided by feedback to improve decision-making and reasoning. Active learning mechanisms allow PRefLexOR to dynamically generate new tasks, reasoning steps, and rejected answers on-the-fly during training. This adaptive process enables the model to self-teach as it continually improves through real-time feedback and recursive processing. Our method diverges from traditional approaches by not relying on pre-generated datasets; instead, it dynamically generates new tasks, reasoning steps, and feedback on the fly, allowing the model to continuously adapt and improve in real time. Recursive optimization within the thinking token framework introduces iterative feedback loops, where the model refines its reasoning, much like policy refinement in RL, achieving deeper coherence, consistency, and adaptability. By recursively optimizing reasoning through feedback-driven learning, PRefLexOR achieves significant flexibility in its ability to handle complex tasks, learning and evolving its cognitive abilities autonomously. This framework advances the field of cognitive alignment by demonstrating that models can iteratively teach themselves to reason with greater depth and reflectivity, akin to an RL-based self-improving system capable of solving open-domain problems with superior reasoning depth and logic. Our implementation is straightforward and can be Incorporated into any existing pretrained LLM. The approach is demonstrated in use cases of materials design applications, where a small language model is trained to develop sophisticated reasoning capabilities. Thereby, PRefLexOR builds a dynamic knowledge graph by generating questions from random text and using Retrieval-Augmented Generation (RAG) to retrieve contextually relevant data from the entire corpus, facilitating recursive reasoning through complex interactions between similar nodes in the embedding space.
