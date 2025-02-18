---
title: 'Home'
date: 2023-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: hero
    content:
      title: Fine-Tune Stable Diffusion with LoRA
      text: An ultimate guide to creating wonderful images 🎉
      primary_action:
        text: About Us
        url: https://hugoblox.com/templates/details/docs/
        icon: rocket-launch
      secondary_action:
        text: Read the docs
        url: /docs/
      announcement:
        text: "Our blog posts."
        link:
          text: "Read more on our blog"
          url: "/blog/"
    design:
      spacing:
        padding: [0, 0, 0, 0]
        margin: [0, 0, 0, 0]
      # For full-screen, add `min-h-screen` below
      css_class: ""
      background:
        color: ""
        image:
          # Add your image background to `assets/media/`.
          filename: ""
          filters:
            brightness: 0.5
  - block: stats
    content:
      items:
        - statistic: "100+"
          description: |
            Stable Diffusion  
            Model
        - statistic: "10+"
          description: |
            Trained Models  
            LoRA
        - statistic: "1M+"
          description: |
            Parameter  
            for support
    design:
      # Section background color (CSS class)
      css_class: "bg-gray-100 dark:bg-gray-800"
      # Reduce spacing
      spacing:
        padding: ["1rem", 0, "1rem", 0]
  - block: features
    id: features
    content:
      title: Features
      text: Create your own stable diffusion model easily without the need to train all model. All you need 500 photos
      items:
        - name: Efficient Parameter Utilization
          icon: magnifying-glass
          description: LoRA fine-tunes only a small subset of parameters, reducing computational and memory requirements.
        - name: Faster Training
          icon: bolt
          description: Training times are shorter due to fewer trainable parameters, enabling quicker iterations.
        - name: Preservation of Pre-trained Knowledge
          icon: sparkles
          description:  LoRA minimally alters the original model, retaining its general capabilities.
        - name: Reduced Risk of Overfitting
          icon: code-bracket
          description: Fewer trainable parameters lower the risk of overfitting, especially with small datasets.
        - name: Scalability and Flexibility
          icon: star
          description: LoRA can be applied to various layers, making it adaptable to diverse tasks.
        - name: Cost-Effective
          icon: rectangle-group
          description: Lower resource requirements make LoRA a budget-friendly fine-tuning method.
  - block: cta-card
    content:
      title: "Ask Us any question you need"
      text: "Our docs are clear, concise, and packed with practical examples, making it easy to implement and troubleshoot. They save time and ensure success!"
      button:
        text: Get Started
        url: /docs/
    design:
      card:
        # Card background color (CSS class)
        css_class: "bg-primary-700"
        css_style: ""
---
