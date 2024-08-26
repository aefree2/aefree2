---
title: "Knowledge Transfer from High-Resource to Low-Resource Programming Languages for Code LLMs"
collection: publications
category: preprint
permalink: /publications/2024-Knowledge-Transfer
excerpt: 'This paper presents an effective approach for boosting the performance of Code LLMs on low-resource languages using semi-synthetic data.'
date: 2024-2-20
paperurl: 'https://arxiv.org/pdf/2308.09895'
citation: 'Hu, Zichao, Francesca Lucchetti, Claire Schlesinger, Yash Saxena, <b>Anders Freeman<b>, Sadanand Modak, Arjun Guha, and Joydeep Biswas. "Deploying and evaluating llms to program service mobile robots." IEEE Robotics and Automation Letters (2024).'
---

Over the past few years, Large Language Models of Code (Code LLMs) have started to have a significant impact on programming practice. Code LLMs are also emerging as building blocks for research in programming languages and software engineering. However, Code LLMs produce impressive results on programming languages that are well represented in their training data (e.g., Java, Python, or JavaScript), but struggle with low-resource languages that have limited training data available. Low resource languages include OCaml, Racket, and several others.
This paper presents an effective approach for boosting the performance of Code LLMs on low-resource languages using semi-synthetic data. Our approach, MultiPL-T, translates training data from high-resource languages into training data for low-resource languages in the following way. 1) We use a Code LLM to synthesize tests for commented code from a high-resource language, filtering out faulty tests and code with low test coverage. 2) We use a Code LLM to translate Python code to a target low-resource language, and use tests to validate the translation. We apply this approach to generate tens of thousands of validated training items for Julia, Lua, OCaml, R, and Racket. Furthermore, we use an open model (StarCoderBase) with open training data (The Stack), which allows us to decontaminate benchmarks, train models without violating licenses, and run experiments that could not otherwise be done.
With MultiPL-T generated data, we present fine-tuned versions of StarCoderBase and Code Llama for Julia, Lua, OCaml, R, and Racket. On established benchmarks (MultiPL-E), these models outperform other open Code LLMs. The MultiPL-T approach is easy to apply to new languages, and is significantly more efficient and effective than alternatives such as training longer. 