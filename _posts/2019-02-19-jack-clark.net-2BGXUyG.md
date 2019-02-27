---

layout: post
category: product
title: "Import AI 134: Learning old tricks on new robots; Facebook improves translation with noise; Google wants people to train fake-audio detectors"
date: 2019-02-19 19:51:44
link: https://vrhk.co/2BGXUyG
image: 
domain: jack-clark.net
author: "Jack Clark"
icon: https://s2.wp.com/i/webclip.png
excerpt: "Why robots are the future of ocean maintenance:&hellip;Robot boats, robot copters, and robot underwater gliders&hellip;Researchers with Oslo Metropolitan University and Norwegian University of Science and Technology are trying to reduce the cost of automated sub-sea data collection and surveillance operations through the use of robots, and have published a paper outlining one of the key components needed to build this system &ndash; a cheap, lightweight way to get small sub-surface gliders to be able to return to the surface.
&nbsp; Weight rules everything around me: The technical innovations here involve simplifying the design to reduce the number of components needed to build a pressure-tolerant MUG, which in turn reduces the weight of the systems, making it easier for them to be deployed and recovered via drones.
&ldquo;Further development will add the ability to adjust pitch and yaw, improve power efficiency, add GPS and environmental sensors, as well as UAV deployment/recovery strategies&rdquo;, they write.
&nbsp; Why this esoteric non-AI-heavy paper matters: This paper is mostly interesting for the not-too-distant future it portends; one where robot boats patrol the oceans, releasing underwater gliders to gather information about the environment, and serving as a homebase for drones that can collect the gliders and transmit them back to the robot boat, and serve as a kind of airborne antenna to relay radio signals between the boats and the gliders. Now, just imagine what you&rsquo;ll be able to do with these systems once we get cheaper, more powerful computers and better autonomous control&amp;analysis AI systems that can be deployed onto them &ndash; the future is a world full of robots, sensing and responding to minute fluctuations in the environment.
&nbsp; &nbsp;Read more: Towards autonomous ocean observing systems using Miniature Underwater Gliders with UAV deployment and recovery capabilities (Arxiv).
+++
Sponsored:&nbsp;The O&rsquo;Reilly AI Conference&nbsp;&ndash; New York, April 15&ndash;18:
&hellip;What do you need to know about AI?&nbsp;From hardware innovation to advancements in machine learning to developments in ethics and regulation, join leading experts with the insight you need to see where AI is going&ndash;and how to get there first.&hellip;Register soon.&nbsp;Early price ends March 1st, and space is limited. Save up to $800 on most passes with code IMPORTAI20.
+++
DeepMind shows how to teach new robots old tricks:&hellip;Demonstrates prowess of SAC-X + augmented data approach via completion of a hard simulated and real world robotics task&hellip;Researchers with DeepMind are going backwards in time &ndash; after using reinforcement learning to solve a series of Atari games a few years ago, they&rsquo;re now heading to the beginning of the 20th century, as they try to teach robots to place a ball on a string inside a wooden cup. This is a challenging, worthwhile task for real-world robotics, as it involves complex movement policies, the need to predict the movements of the ball, and demands a decent interplay between perception and action to solve the task.
&nbsp; How they do it: To solve this, DeepMind uses an extension of its Scheduled Auxiliary Control (SAC-X) algorithm, which lets them train across multiple tasks with multiple rewards. Their secret to solving the tasks robustly on physical robots is to use additional data at training time, where the goal is &ldquo;simultaneously learn control policies from both feature-based representation and raw vision inputs in the real-world &ndash; resulting in controllers that can afterwards be deployed on a real robot using two off-the-shelf cameras&rdquo;.
&nbsp; &nbsp;Results: They&rsquo;re able to learn to solve the task in simulation as well as on a real robot. They&rsquo;re able to learn a robust, successful policy on the robot: &ldquo;The swing-up is smooth and the robot recovers from failed catches. With a brief evaluation of 20 runs, each trial running for 10 seconds, we measured 100% catch rate. The shortest catch time being 2 seconds.&rdquo; They also tested out the robot with a smaller cup to make the task more difficult &ndash; &ldquo;there were a slight slow-down in learning and a small drop in catch rate to 80%, still with a shortest time to catch of 2 seconds,&rdquo; they write. They&rsquo;re able to learn the task on the real robot in about 28 continuous hours of training (so more like ~40 hours when you account for re-setting the experiment, etc).
&nbsp; Why it matters: Getting anything to work reliably on a real robot is a journey of pain, frustration, pain, tedium, and &ndash; yes! &ndash; more pain. It&rsquo;s encouraging to see SAC-X work in this domain, and it suggests that we&rsquo;re figuring out better ways to learn things on real-world platforms.
&nbsp;&nbsp;Check out the videos of the simulated and real robots here (Google Sites).&nbsp;&nbsp;Read more: Simultaneously Learning Vision and Feature-based Control Policies for Real-world Ball-in-a-Cup (Arxiv).
+++
Want better translation models? Use noise, Facebook says:&hellip;Addition of noise can improve test-time performance, though it doesn&rsquo;t help with social media posts&hellip;You can improve the performance of machine translation systems by injecting some noise into the training data, according to Facebook AI Research. The result is models that are more robust to the sort of crappy data found in the real world, the researchers write.
&nbsp; Noise methods: The technique uses four noise methods: deletions, insertions, substitutions, and swaps. Deletions are where the researchers delete a character in a sentence; insertions are where they insert a character into a random position; substitutions are where they replace a character with another random character, and swaps are where two adjacent characters change position.
&nbsp; &nbsp;Results: They test the approach on the IWSLT machine translation benchmark by training over datasets with varying amounts of noise injected into the test data, and observing how they can influence the BLEU score of models trained against this data by injecting synthetic noise into the dataset. &ldquo;Training on our synthetic noise cocktail greatly improves performance, regaining between 20% (Czech) and 50% (German) of the BLEU score that was lost to natural noise,&rdquo; they write.
&nbsp;&nbsp;Where doesn&rsquo;t noise help: This technique doesn&rsquo;t help when trying to perform translations on text derived from social media &ndash; this is because social media errors tend to stem from content on having a radically different writing and tonal style to what is traditionally seen in training sets, rather than spelling errors.
&nbsp;&nbsp;Observation: Conceptually, these techniques seem to have a lot in common&nbsp;with domain randomization, which is where people generate synthetic data designed to explore broader variations than would otherwise be found. Such techniques have been used for a few years in robotics work, and typically improve real world model performance by increasing the robustness to the significant variations introduced by reality.
&nbsp; Why this matters: This is another example of the ways in which computers can be arbitraged for data: instead of needing to go and gather datasets with real-world faults, the addition of synthetic noise means you can instead algorithmically extend existing datasets through the augmentation of noisy data. The larger implication here is that computational resources are becoming an ever-more-significant factor in AI development.
Read more: Training on Synthetic Noise IMproves Robustness to Natural Noise in Machine Translation (Arxiv).
+++
In the future, neural networks will be bred, not created:&hellip;General-purpose population training for those who can afford it&hellip;Population Based Training (PBT) is a recent invention by DeepMind that makes it possible to optimize the weights and hyperparameters of a set of neural n…"

---

### Import AI 134: Learning old tricks on new robots; Facebook improves translation with noise; Google wants people to train fake-audio detectors

Why robots are the future of ocean maintenance:&hellip;Robot boats, robot copters, and robot underwater gliders&hellip;Researchers with Oslo Metropolitan University and Norwegian University of Science and Technology are trying to reduce the cost of automated sub-sea data collection and surveillance operations through the use of robots, and have published a paper outlining one of the key components needed to build this system &ndash; a cheap, lightweight way to get small sub-surface gliders to be able to return to the surface.
&nbsp; Weight rules everything around me: The technical innovations here involve simplifying the design to reduce the number of components needed to build a pressure-tolerant MUG, which in turn reduces the weight of the systems, making it easier for them to be deployed and recovered via drones.
&ldquo;Further development will add the ability to adjust pitch and yaw, improve power efficiency, add GPS and environmental sensors, as well as UAV deployment/recovery strategies&rdquo;, they write.
&nbsp; Why this esoteric non-AI-heavy paper matters: This paper is mostly interesting for the not-too-distant future it portends; one where robot boats patrol the oceans, releasing underwater gliders to gather information about the environment, and serving as a homebase for drones that can collect the gliders and transmit them back to the robot boat, and serve as a kind of airborne antenna to relay radio signals between the boats and the gliders. Now, just imagine what you&rsquo;ll be able to do with these systems once we get cheaper, more powerful computers and better autonomous control&amp;analysis AI systems that can be deployed onto them &ndash; the future is a world full of robots, sensing and responding to minute fluctuations in the environment.
&nbsp; &nbsp;Read more: Towards autonomous ocean observing systems using Miniature Underwater Gliders with UAV deployment and recovery capabilities (Arxiv).
+++
Sponsored:&nbsp;The O&rsquo;Reilly AI Conference&nbsp;&ndash; New York, April 15&ndash;18:
&hellip;What do you need to know about AI?&nbsp;From hardware innovation to advancements in machine learning to developments in ethics and regulation, join leading experts with the insight you need to see where AI is going&ndash;and how to get there first.&hellip;Register soon.&nbsp;Early price ends March 1st, and space is limited. Save up to $800 on most passes with code IMPORTAI20.
+++
DeepMind shows how to teach new robots old tricks:&hellip;Demonstrates prowess of SAC-X + augmented data approach via completion of a hard simulated and real world robotics task&hellip;Researchers with DeepMind are going backwards in time &ndash; after using reinforcement learning to solve a series of Atari games a few years ago, they&rsquo;re now heading to the beginning of the 20th century, as they try to teach robots to place a ball on a string inside a wooden cup. This is a challenging, worthwhile task for real-world robotics, as it involves complex movement policies, the need to predict the movements of the ball, and demands a decent interplay between perception and action to solve the task.
&nbsp; How they do it: To solve this, DeepMind uses an extension of its Scheduled Auxiliary Control (SAC-X) algorithm, which lets them train across multiple tasks with multiple rewards. Their secret to solving the tasks robustly on physical robots is to use additional data at training time, where the goal is &ldquo;simultaneously learn control policies from both feature-based representation and raw vision inputs in the real-world &ndash; resulting in controllers that can afterwards be deployed on a real robot using two off-the-shelf cameras&rdquo;.
&nbsp; &nbsp;Results: They&rsquo;re able to learn to solve the task in simulation as well as on a real robot. They&rsquo;re able to learn a robust, successful policy on the robot: &ldquo;The swing-up is smooth and the robot recovers from failed catches. With a brief evaluation of 20 runs, each trial running for 10 seconds, we measured 100% catch rate. The shortest catch time being 2 seconds.&rdquo; They also tested out the robot with a smaller cup to make the task more difficult &ndash; &ldquo;there were a slight slow-down in learning and a small drop in catch rate to 80%, still with a shortest time to catch of 2 seconds,&rdquo; they write. They&rsquo;re able to learn the task on the real robot in about 28 continuous hours of training (so more like ~40 hours when you account for re-setting the experiment, etc).
&nbsp; Why it matters: Getting anything to work reliably on a real robot is a journey of pain, frustration, pain, tedium, and &ndash; yes! &ndash; more pain. It&rsquo;s encouraging to see SAC-X work in this domain, and it suggests that we&rsquo;re figuring out better ways to learn things on real-world platforms.
&nbsp;&nbsp;Check out the videos of the simulated and real robots here (Google Sites).&nbsp;&nbsp;Read more: Simultaneously Learning Vision and Feature-based Control Policies for Real-world Ball-in-a-Cup (Arxiv).
+++
Want better translation models? Use noise, Facebook says:&hellip;Addition of noise can improve test-time performance, though it doesn&rsquo;t help with social media posts&hellip;You can improve the performance of machine translation systems by injecting some noise into the training data, according to Facebook AI Research. The result is models that are more robust to the sort of crappy data found in the real world, the researchers write.
&nbsp; Noise methods: The technique uses four noise methods: deletions, insertions, substitutions, and swaps. Deletions are where the researchers delete a character in a sentence; insertions are where they insert a character into a random position; substitutions are where they replace a character with another random character, and swaps are where two adjacent characters change position.
&nbsp; &nbsp;Results: They test the approach on the IWSLT machine translation benchmark by training over datasets with varying amounts of noise injected into the test data, and observing how they can influence the BLEU score of models trained against this data by injecting synthetic noise into the dataset. &ldquo;Training on our synthetic noise cocktail greatly improves performance, regaining between 20% (Czech) and 50% (German) of the BLEU score that was lost to natural noise,&rdquo; they write.
&nbsp;&nbsp;Where doesn&rsquo;t noise help: This technique doesn&rsquo;t help when trying to perform translations on text derived from social media &ndash; this is because social media errors tend to stem from content on having a radically different writing and tonal style to what is traditionally seen in training sets, rather than spelling errors.
&nbsp;&nbsp;Observation: Conceptually, these techniques seem to have a lot in common&nbsp;with domain randomization, which is where people generate synthetic data designed to explore broader variations than would otherwise be found. Such techniques have been used for a few years in robotics work, and typically improve real world model performance by increasing the robustness to the significant variations introduced by reality.
&nbsp; Why this matters: This is another example of the ways in which computers can be arbitraged for data: instead of needing to go and gather datasets with real-world faults, the addition of synthetic noise means you can instead algorithmically extend existing datasets through the augmentation of noisy data. The larger implication here is that computational resources are becoming an ever-more-significant factor in AI development.
Read more: Training on Synthetic Noise IMproves Robustness to Natural Noise in Machine Translation (Arxiv).
+++
In the future, neural networks will be bred, not created:&hellip;General-purpose population training for those who can afford it&hellip;Population Based Training (PBT) is a recent invention by DeepMind that makes it possible to optimize the weights and hyperparameters of a set of neural n…