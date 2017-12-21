+++
# Date this page was created.
date = "2016-04-27"

# Project title.
title = "Improved exploration in random forest based classifiers"

# Project summary to display on homepage.
summary = "We use Upper Confidence Bound and Thompson sampling to determine split criteria at each node in a random forest in a bid to improve its exploratory capabilities when doing classification."

# Optional image to display on homepage (relative to `static/img/` folder).
# image_preview = "bubbles.jpg"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "optimization", "reinforcement-learning"]`
tags = ["machine-learning", "optimization", "reinforcement-learning"]

# Optional external URL for project (replaces project detail page).
external_link = "https://drive.google.com/file/d/0B2cLSd2WLeFidDZwQ2ZSUnU2SnM/view?usp=sharing"

# Does the project detail page use math formatting?
math = false

# Optional featured image (relative to `static/img/` folder).
[header]
# image = "headers/bubbles-wide.jpg"
# caption = "My caption :smile:"

+++

Extreme multi label learning (XML) is an important problem today, being addressed for document tagging, recommender systems and the like. Most of the classifiers though are conservative in their approach, trying to optimize on the evaluation metric and thus focussing almost exclusively on exploitation. This project tries to come up with various approaches to introduce a knob to control the extent of exploration / exploitation. This would help, for instance, to
discover novel items to be recommended to users.

As a starting point, we deal with binary classification, but the algorithms used can be generalized to multi label learning as well. We focus on hierarchical methods, trying to emulate the success of FastXML [1], a popular method for the task proposed by Prabhu et. al. We use the principle of Optimism in the Face of Uncertainty to modify a random forest to be able to use the UCB algorithm / Thompson sampling to select the split criterion at each node and use a ranking loss to evaluate the split. We compare our results against the general random forests
for some popular datasets for binary classification.
