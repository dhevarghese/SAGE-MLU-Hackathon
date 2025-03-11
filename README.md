# **Welcome to the SAGE-MLU Hackathon!**

## **Overview**

We're excited to have you join us for this hackathon, as part of the [**First Workshop on Structure & Generalization in Multimodal Language Understanding (SAGE-MLU)**](https://sites.google.com/view/sage-mlu-2025/home?authuser=0). This event is an opportunity to collaborate in small groups and explore a key research question:

> **How do language-only models and vision-language models differ in their understanding of linguistic or conceptual phenomena?**

To investigate this, we suggest that each team:

1.  **Identify a specific phenomenon** where these models might behave differently.
2.  **Develop a mini challenge set** to test this phenomenon.
3.  **Evaluate a minimal pair of models** (e.g., Gemma vs. PaliGemma) on the challenge set.
4.  **Present findings** at the end of the day.

To help you get started, we’ve prepared an example setup using **PaliGemma 2-3B**, but note that inference code may vary across models. Refer to **`sample-inference.ipynb`** for a short walkthrough!

### **Suggested Model Pairs**

We encourage you to explore differences between models using these pairs:

-   **Gemma 2** vs. **PaliGemma 2**
-   **Qwen** vs. **Molmo**
-   **LLaMA** vs. **LLaVA**

(Feel free to choose different models if relevant to your task!)

We hope that some of these ideas will spark further collaborations beyond the workshop!

## **Sample Task Setup: Decoding Semantic Geometry in VLMs**

In this setup, we'll be exploring, implementing, and extending ideas from the paper [**"The Geometry of Categorical and Hierarchical Concepts in LLMs"**](https://arxiv.org/abs/2406.01506), published at ICLR 2025. We dive into the representation geometry of Large Language Models (LLMs) and explore how concepts are encoded in their latent spaces. By the end, we aim to have insights into the representation geometry of *Vision Language Models (VLMs)*.

**Key Concepts & Resources:**

*   **WordNet:** A lexical database organizing words into hierarchical sets of synonyms. A useful resource for exploring relationships. More info: [WordNet](https://wordnet.princeton.edu/).

*   **Representation Spaces:**  LLMs convert words into high-dimensional vectors (embeddings). The arrangement of these vectors reflects semantic relationships. Learn more: [HuggingFace Blogpost](https://huggingface.co/blog/getting-started-with-embeddings), [3D Visualization](https://tomhazledine.com/mapping-llm-embeddings-in-3d/).

*   **Linear Representation Hypothesis:**  The idea that semantic concepts are encoded as linear directions or subspaces within an LLM's representation space. [Prior work](https://arxiv.org/abs/2311.03658) has demonstrated this for binary concepts (e.g., gender opposites like male↔female). This paper extends this work to represent categories (e.g., {mammal, bird, reptile}) and hierarchical structures (e.g., animal → mammal → dog).

**Why Is This Interesting?**

* **Interpretability**: Understanding how LLMs structure conceptual knowledge is helpful to interpretability.
* **Better Probing & Steering**: If concepts are geometrically structured, we can develop better ways to extract and modify knowledge in LLMs.
* **Generalization**: Insights into hierarchical encoding could improve compositionality in multimodal models.

## Hackathon Goals: Extend to Vision Language Models!

Our focus is to investigate the representation geometry in VLMs. We aim to:

*   **Replicate:**  Confirm the original paper's findings on different LLMs and explore additional geometric properties.
*   **Extend to Multimodal:**  Does the geometric structure of semantic concepts hold for VLMs? How do visual (e.g., *cat* image) and textual concepts relate geometrically?

## Let's Get Hacking!

You've got the background, now let's get to work! 