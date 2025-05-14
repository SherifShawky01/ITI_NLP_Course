# “Attention Is All You Need” paper

| Core Idea | Why It Matters in Practice |
|-----------|---------------------------|
| **Pure Transformer (no RNN/CNN)** | Enables *fully parallel* training & inference — huge speed-ups on GPUs/TPUs. |
| **Self-attention over every token pair** | Constant path length → much better at capturing long-range dependencies. |
| **Multi-head attention** | Lets the network focus on multiple relational sub-spaces at once → richer context. |
| **Positional encoding** | Injects order info without breaking parallelism. |
| **Residual + LayerNorm** | Stabilises deep stacks and speeds convergence. |
| **Position-wise feed-forward blocks** | Simple, shared, matrix-multiply kernels → hardware-friendly & easy to implement. |
| **Scales cleanly with data & compute** | Foundation for BERT, GPT, T5, ViT, Speech & RL Transformers. |
| **Immediate SOTA in machine translation** | Early proof of power; accelerated community adoption. |

>By replacing recurrence with self-attention, the paper gave us a faster,
easier-to-scale architecture that now underpins virtually every modern large-scale AI system.
