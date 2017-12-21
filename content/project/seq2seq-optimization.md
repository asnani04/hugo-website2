+++
# Date this page was created.
date = "2016-04-27"

# Project title.
title = "Optimizing Sequence to Sequence Learning models for BLEU score"

# Project summary to display on homepage.
summary = "We came up with varied loss functions to try and improve the convergence properties of sequence to sequence learning models with respect to the BLEU score."

# Optional image to display on homepage (relative to `static/img/` folder).
# image_preview = "bubbles.jpg"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "optimization", "natural-language-processing", "text-generation"]`
tags = ["machine-learning", "optimization", "natural-language-processing", "text-generation"]

# Optional external URL for project (replaces project detail page).
external_link = "https://drive.google.com/file/d/1kFUSdBeYGJRpHzsO8Oe0loeIekJ45YTt/view?usp=sharing"

# Does the project detail page use math formatting?
math = false

# Optional featured image (relative to `static/img/` folder).
[header]
# image = "headers/bubbles-wide.jpg"
# caption = "My caption :smile:"

+++

In a bid to improve the optimization of sequence to sequence models for tasks like machine translation, we tried to construct loss functions that would approximate the most commonly used metric, BLEU score. We came up with variants of a ”Residual” Loss, and experimented with its combinations with cross entropy loss to see if we could detect improved performance. Our experiments provide a unique insight into the functioning of LSTM networks in general and seq2seq models in particular, with respect to the loss functions used.