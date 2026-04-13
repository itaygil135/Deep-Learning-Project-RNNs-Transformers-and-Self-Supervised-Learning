Deep Learning Systems — RNNs, Transformers, and Self-Supervised Learning

Technologies:
Python, PyTorch, NumPy, Transformers, CLIP, DINO

Project Description:
This project focuses on implementing core deep learning architectures and modern representation learning methods from scratch.

The work includes:
- Implementation of Recurrent Neural Networks (RNNs) and Long Short-Term Memory (LSTM), including forward and backward passes
- Building an image captioning system trained on the COCO dataset
- Integration of attention mechanisms to improve caption generation by focusing on relevant regions in the image
- Full implementation of a Transformer architecture from scratch:
  - Multi-head attention
  - Positional encoding
  - Encoder-decoder structure
  - Residual connections
- Training Transformer models on sequence-to-sequence tasks
- Implementation of self-supervised learning using SimCLR, including augmentations and contrastive loss
- Application of CLIP for zero-shot image-text alignment and image retrieval
- Using-DINO features for semantic segmentation

Through this project, I gained strong hands-on experience with:
- Deep learning pipelines
- Sequence modeling
- Multimodal learning
- Representation learning

Project Structure (IMPORTANT):

There is necessary code in Python (.py) files inside the folder:
dl/
and in subfolders within dl/.

If you want to explore the full implementation, you are very welcome to go through these files.

HOWEVER — the real core of the project is:

The Jupyter Notebook files (.ipynb)

These notebooks contain:
- The main logic
- The experiments
- The training process
- The results

In other words:
The notebooks are the “main files” of the project.

Summary:
- Core logic and execution: .ipynb files
- Supporting implementation: dl/ folder and subfolders

Additional Note (GitHub Notebook Issue):

If a notebook does not render on GitHub and shows an error related to:
metadata.widgets

You can fix it by removing this metadata using:

import nbformat

path = "your_notebook.ipynb"

with open(path, "r", encoding="utf-8") as f:
    nb = nbformat.read(f, as_version=4)

if "widgets" in nb.metadata:
    del nb.metadata["widgets"]

with open(path, "w", encoding="utf-8") as f:
    nbformat.write(nb, f)

print("Removed metadata.widgets")

