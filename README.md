# Prompts for News Angles
This repo contains the prompts we used to compute the News Angles for News Compass with the following model and configurations:

Model : ``gpt-5-nano-2025-08-07`` 
Reasoning Effort: ``minimal``  (fastest for classification tasks)
Text Verbosity: ``low``  (concise outputs)
Max Output Tokens: 600  (room for 3 angles with reasoning)

We selected GPT-5-Nano for this task using a human evaluation process, where we compared three LLMs (GPT-5-Nano, Phi-4, Gemma3-14b) + a one encoder-decore model (bart-large-mnli) for how appropriate and interesting their assigned news angles were, as judged by a human annotator, and how well the model's confidence in its angle labels was calibrated against these ratings. Full details of this evaluation process will be made available later. This repo presents the prompts and angle definitions for anyone interested in how we did this. 
