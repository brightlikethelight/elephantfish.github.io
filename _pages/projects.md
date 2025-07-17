---
layout: page
title: research projects
permalink: /projects/
description: Deep learning research spanning interpretability, vision-language models, and scientific applications
nav: true
nav_order: 2
display_categories: [interpretability, vision-language, scientific-ml, architectures]
horizontal: false
---

## Research Portfolio

My research focuses on advancing our understanding of deep neural networks through interpretability methods, novel architectures, and scientific applications. Below are the major research areas with representative projects from my MIT 6.S898 graduate coursework and ongoing investigations.

---

## 🔍 Neural Network Interpretability

Understanding how neural networks make decisions is crucial for their responsible deployment in critical applications.

### Sparse Autoencoders for Language Models
**Developing interpretable feature extraction methods for large language models**

- **Objective**: Create sparse representations that maintain model performance while providing interpretable feature extraction
- **Methodology**: Implementation of sparse autoencoder architectures with L1 regularization and feature visualization
- **Results**: Successful extraction of human-interpretable features from transformer hidden states
- **Impact**: Enables better understanding of what language models learn and how they process information
- **Blog Posts**: [Sparse Autoencoder Series]({{ site.baseurl }}/blog/tag/sparse-autoencoders/)

### CNN Activation Patching
**Advanced techniques for understanding convolutional neural network decision processes**

- **Objective**: Develop methods to trace how information flows through CNN architectures
- **Methodology**: Systematic intervention experiments on activation patterns across network layers
- **Results**: Identification of critical pathways for different types of visual recognition tasks
- **Applications**: Improved model debugging and robustness analysis
- **Blog Posts**: [CNN Interpretability Research]({{ site.baseurl }}/blog/tag/cnn-interpretability/)

---

## 🤖 Vision-Language Models

Investigating the intersection of computer vision and natural language processing through modern multimodal architectures.

### CLIP Visualization & Learning Dynamics
**Comprehensive analysis of vision-language model training and representation learning**

- **Objective**: Understand how CLIP models learn to align visual and textual representations
- **Methodology**: Training dynamics analysis, representation visualization, and feature attribution
- **Key Findings**: Characterization of multimodal learning phases and optimal training strategies
- **Publications**: Multiple blog posts documenting training dynamics and visualization techniques
- **Blog Posts**: [CLIP Research Series]({{ site.baseurl }}/blog/tag/clip/)

### Multimodal Representation Learning
**Analysis of learned representations in recommendation systems**

- **Focus**: How neural networks learn to represent items and users in collaborative filtering
- **Techniques**: Embedding analysis, dimensionality reduction, and similarity metrics
- **Applications**: Improved recommendation algorithms and user experience personalization
- **Blog Posts**: [Representation Learning Studies]({{ site.baseurl }}/blog/tag/representation-learning/)

---

## ⚙️ Scientific Machine Learning

Applying deep learning to scientific computing problems and integrating domain knowledge into neural architectures.

### Physics-Informed Neural Networks (PINNs)
**Neural network approaches to complex physical system modeling**

- **Objective**: Integrate physical laws and constraints directly into neural network training
- **Domains**: Fluid dynamics, heat transfer, and electromagnetic systems
- **Methodology**: Custom loss functions incorporating differential equations and boundary conditions
- **Results**: Improved accuracy and physical consistency compared to purely data-driven approaches
- **Blog Posts**: [Physics-Informed ML Series]({{ site.baseurl }}/blog/tag/physics-informed/)

### Ecological Modeling with Transformers
**Transformer-based approaches for environmental data analysis**

- **Application**: Time series prediction for ecological systems
- **Innovation**: Adaptation of attention mechanisms for environmental monitoring data
- **Impact**: Improved prediction accuracy for complex ecological interactions
- **Blog Posts**: [Ecological ML Research]({{ site.baseurl }}/blog/tag/ecological-modeling/)

### Single-cell RNA Analysis (scRNA-GNNs)
**Graph Neural Networks for biological data interpretation**

- **Problem**: Understanding cellular processes through gene expression data
- **Approach**: Custom GNN architectures designed for single-cell data characteristics
- **Results**: Improved cell type classification and trajectory inference
- **Biological Impact**: Enhanced understanding of cellular differentiation and disease processes
- **Blog Posts**: [scRNA-GNN Research]({{ site.baseurl }}/blog/tag/scrna-gnn/)

---

## 🏗️ Novel Architectures

Exploring innovative neural network designs and their applications across diverse domains.

### Transformers as Gamers
**Investigation of transformer applications in strategic decision-making**

- **Concept**: Applying attention mechanisms to game-theoretic scenarios
- **Implementation**: Custom transformer variants optimized for strategic reasoning
- **Evaluation**: Performance on classic game theory problems and strategic planning tasks
- **Blog Posts**: [Transformer Architecture Research]({{ site.baseurl }}/blog/tag/transformers/)

### Task-Specific Data Augmentation
**Custom augmentation strategies for domain-specific problems**

- **Approach**: Learning optimal data augmentation policies for specific tasks
- **Methodology**: Reinforcement learning and genetic algorithm approaches to augmentation design
- **Results**: Improved generalization and robustness across multiple domains
- **Blog Posts**: [Data Augmentation Studies]({{ site.baseurl }}/blog/tag/data-augmentation/)

---

## 🛠️ Technical Infrastructure

All research projects are supported by robust technical infrastructure ensuring reproducibility and scalability.

### Reproducible Research Pipeline
- **Docker Containers**: Complete experimental environments for consistent reproduction
- **Version Control**: Comprehensive Git workflows for all experiments and analysis
- **Documentation**: Detailed experimental protocols and implementation guides
- **Open Source**: All research code publicly available with clear licensing

### High-Performance Computing
- **Distributed Training**: Multi-GPU and cluster computing for large-scale experiments
- **Optimization**: Efficient implementations for resource-constrained environments
- **Monitoring**: Comprehensive logging and visualization of training dynamics

### Academic Standards
- **Literature Integration**: Thorough review and citation of relevant academic work
- **Statistical Rigor**: Appropriate statistical methods and significance testing
- **Peer Review**: Collaborative evaluation and feedback integration

---

## 📊 Research Impact

### Quantitative Metrics
- **100+ Research Blog Posts**: Detailed technical documentation across all research areas
- **Open Source Contributions**: Multiple repositories with active community engagement
- **Academic Presentations**: Research shared at MIT and broader academic community
- **Collaborative Projects**: Cross-disciplinary work with faculty and industry partners

### Qualitative Contributions
- **Methodological Advances**: Novel techniques for neural network interpretability and analysis
- **Cross-domain Applications**: Successful transfer of methods across multiple problem domains
- **Educational Impact**: Accessible documentation enabling others to build on this work
- **Scientific Rigor**: High standards for experimental design and result validation

---

## 🚀 Current Research Directions

### Active Projects
- **Advanced Sparse Architectures**: Developing next-generation sparse autoencoder methods
- **Multimodal Interpretability**: Extending interpretability methods to vision-language models
- **Scientific Discovery**: Applying deep learning to accelerate scientific research
- **Optimal Control**: Neural approaches to complex control problems

### Collaborative Opportunities
- **Industry Partnerships**: Translating research into practical applications
- **Academic Collaboration**: Working with faculty and researchers on publishable work
- **Open Source**: Contributing to community tools and frameworks
- **Mentorship**: Supporting undergraduate and graduate student research

---

## 📖 Featured Publications & Posts

### Recent Highlights
{% assign recent_posts = site.posts | where: "tags", "featured" | slice: 0, 6 %}
{% if recent_posts.size > 0 %}
<div class="row">
{% for post in recent_posts %}
  <div class="col-md-6 mb-4">
    <div class="card h-100">
      <div class="card-body">
        <h5 class="card-title">
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </h5>
        <p class="card-text text-muted small">{{ post.date | date: "%B %d, %Y" }}</p>
        {% if post.description %}
        <p class="card-text">{{ post.description }}</p>
        {% endif %}
        {% if post.tags %}
        <div class="mb-2">
          {% for tag in post.tags limit:3 %}
          <span class="badge badge-secondary mr-1">{{ tag }}</span>
          {% endfor %}
        </div>
        {% endif %}
      </div>
    </div>
  </div>
{% endfor %}
</div>
{% else %}
### All Research Areas
Explore research across multiple domains through our comprehensive blog archive:
- [All Research Posts]({{ site.baseurl }}/blog/)
- [Research by Category]({{ site.baseurl }}/blog/categories/)
- [Research by Tag]({{ site.baseurl }}/blog/tags/)
{% endif %}

---

## 🔗 Research Resources

### Code Repositories
- **GitHub**: [Complete research code repositories](https://github.com/{{ site.github_username }})
- **Documentation**: Detailed implementation guides and tutorials
- **Reproducibility**: Docker containers and environment specifications

### Academic Resources
- **Bibliography**: Comprehensive reference management
- **Datasets**: Curated datasets for research reproduction
- **Benchmarks**: Performance evaluation and comparison frameworks

### Community Engagement
- **Open Source**: Active contribution to community projects
- **Mentorship**: Supporting next-generation researchers
- **Collaboration**: Academic and industry partnership opportunities

---

*Each project represents a significant investment in understanding and advancing the state of deep learning. For detailed technical documentation, implementation code, and experimental results, please explore the associated blog posts and GitHub repositories.*