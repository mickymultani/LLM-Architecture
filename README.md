# LLM-Architecture

_Note: Download the notebook, as its too big to display in GitHub_

## GPT-2 Medium Architecture Visualizations
Explore the architecture of the GPT-2 Medium model through a series of insightful and interactive visualizations. This repository provides tools to understand the model's attention mechanisms, neuron activations, token embeddings, and overall architecture.

## Table of Contents
1. Model Summary
2. Token Activations
2. Attention Visualization
2. Model Architecture 3D
3. Token Projections in 2D and 3D
5. Gradients and Saliency


### 1. Model Summary
Get a concise summary of the GPT-2 model's architecture and specifications.

How to Use:
```python
from visualize import model_summary

model_summary()
```

Interpretation:
This summary provides an overview of the model's architecture, including details like the number of layers, neurons, and attention heads. It offers a snapshot of the model's complexity and design.


### 2. Token Activations
Explore the activations of tokens across layers and understand the importance of each token.

How to Use:
```python
from visualize import plot_token_activations

sentence = "The quick brown fox jumps over the lazy dog."
plot_token_activations(sentence)
```

Interpretation:
Token activations provide insights into how each token is processed within the neural network. Observing the activations can help understand the significance of each token in the context of the model's understanding.

### 3. Attention Visualization
Visualize how the GPT-2 model's attention mechanism focuses on different parts of a given text.

How to Use:
```python
from visualize import plot_attention

sentence = "The quick brown fox jumps over the lazy dog."
plot_attention(sentence, layer=3, head=4)
```

Interpretation:
Attention scores represent the model's focus on different tokens when producing an output for a specific token. Higher attention scores between two tokens indicate a stronger relationship or dependency.


### 4. 3D Model Architecture
Visualize the entire architecture of the GPT-2 model in 3D space.

How to Use:
```python
from visualize import enhanced_3d_visualization

enhanced_3d_visualization()
```

Interpretation:
This 3D visualization offers a spatial representation of the model's layers and neurons, giving a tangible sense of the model's depth and structure.


### 5. Token Embeddings
Project token embeddings into 2D or 3D space to understand the relationships between tokens.

How to Use:
```python
from visualize import plot_token_embeddings

sentence = "The quick brown fox jumps over the lazy dog."
plot_token_embeddings(sentence)
```

Interpretation:
Token embeddings represent tokens in a high-dimensional space. By projecting them into 2D or 3D, we can visualize clusters of similar tokens or relationships between tokens.

### 5. Gradients and Saliency
Visualize the influence of each token on the model's output using gradients.

How to Use:
```python
from visualize import plot_gradients

sentence = "The quick brown fox jumps over the lazy dog."
plot_gradients(sentence)
```

Interpretation:
Gradients provide insights into which tokens influence the model's decision-making process the most. This can be especially useful for understanding the model's behavior on specific tasks.




## Conclusion
These visualizations serve as a window into the GPT-2 model, an dhopefully explain some of its operations and helping both beginners and experts gain a deeper understanding of its inner workings. If you're trying to debug, interpret, or simply appreciate the model, these tools offer valuable insights.

I'll write up more details on each of these aspects in the docs folder.

## License
MIT
