# VideoProctoring
Using a VLLM based workflow for analysing student attentiveness for Video Proctoring

Dependencies:
OpenCV2
Pillow
Transformers
PyTorch

Filename: VideoProctoringTest.ipynb

This single Jupyter Notebook contains code to:
1- Extract frames from the input video
2- Pass the extracted frames into a lightweight VLM - in this case, SmolVLM 500M for captioning and analysis
3- Storing the extracted frames in a JSON file
4- Passing the JSON captions into a lightweight LLM - in this case, Gemma3 1B for analysis and conclusion generation

Requirements:
This code was tested to work with Python 3.11.8
An NVIDIA GPU is recommended - especially for running the LLM.

Notes:
This workflow is remarkably performant, generating conclusions about a 26 second video in 1 minute 5 seconds - testing on a RTX 3050Ti 4GB

Contributing and Feedback:
Please do suggest improvements to the workflow, and do share any ideas you have regarding VLMs!
You can contact me on ramsundar289@gmail.com
