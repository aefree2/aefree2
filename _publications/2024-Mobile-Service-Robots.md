---
title: "Deploying and Evaluating LLMs to Program Service Mobile Robots"
collection: publications
category: manuscript
permalink: "/publication/2024-Mobile-Service-Robots"
excerpt: 'We contribute CodeBotler, an open-source robot-agnostic tool to program service mobile robots from natural language, and RoboEval, a benchmark for evaluating LLMs' capabilities of generating programs to complete service robot tasks.'
date: 2024-04-01
venue: 'IEEE Robotics and Automation Letters'
paperurl: "http://dx.doi.org/10.1109/LRA.2024.3360020"
citation: 'Hu, Zichao, Francesca Lucchetti, Claire Schlesinger, Yash Saxena, <b>Anders Freeman<b>, Sadanand Modak, Arjun Guha, and Joydeep Biswas. "Deploying and evaluating llms to program service mobile robots." IEEE Robotics and Automation Letters (2024).'


---

Recent advancements in large language models (LLMs) have spurred interest in using them for generating robot programs from natural language, with promising initial results. We investigate the use of LLMs to generate programs for service mobile robots leveraging mobility, perception, and human interaction skills, and where accurate sequencing and ordering of actions is crucial for success. We contribute CodeBotler, an open-source robot-agnostic tool to program service mobile robots from natural language, and RoboEval, a benchmark for evaluating LLMs' capabilities of generating programs to complete service robot tasks. CodeBotler performs program generation via few-shot prompting of LLMs with an embedded domain-specific language (eDSL) in Python, and leverages skill abstractions to deploy generated programs on any general-purpose mobile robot. RoboEval evaluates the correctness of generated programs by checking execution traces starting with multiple initial states, and checking whether the traces satisfy temporal logic properties that encode correctness for each task. RoboEval also includes multiple prompts per task to test for the robustness of program generation. We evaluate several popular state-of-the-art LLMs with the RoboEval benchmark, and perform a thorough analysis of the modes of failures, resulting in a taxonomy that highlights common pitfalls of LLMs at generating robot programs.