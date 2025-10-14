# Prompts for News Angles
This repo contains the prompts we used to compute the News Angles for News Compass with the following model and configurations:

Model : ``gpt-5-nano-2025-08-07``   
Reasoning Effort: ``minimal``  (fastest for classification tasks)  
Text Verbosity: ``low``  (concise outputs)  
Max Output Tokens: 600  (room for 3 angles with reasoning)  

We selected GPT-5-Nano for this task using a human evaluation process, where we compared three LLMs (GPT-5-Nano, Phi-4, Gemma3-14b) + one encoder-decoder model (bart-large-mnli, cheaper than LLMs and popularly used for text classification tasks) for how appropriate and interesting their assigned news angles were, as judged by a human annotator. We also compared how well the model's confidence in its angle labels was calibrated against these human judgements (i.e., if a model has a high confidence score for a particular news angle, is that correlated to the human evaluator's judgements of appropriateness?). Full details of this evaluation process will be made available later. This repo presents the prompts and angle definitions for anyone interested in how we did this. 

``angle_definitions.txt``: Contains definitions of the different news angles.  
``prompt_template.txt``: Incorporates the angle definitions textfile to instruct the model for a JSON formatted list of news angles and confidence scores, along with a few-shot examples.  
``system_message.txt``: System prompt fed into the three models to ensure they follow instructions and do not assign angles without cause.   
