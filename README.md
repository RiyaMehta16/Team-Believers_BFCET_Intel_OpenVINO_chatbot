# Health-related Chatbot Project

## Project Title
Health-related GPT-2 Fine-tuned Chatbot with Intel® OpenVINO™ Optimization

## Description
This project addresses the challenge of "Running GenAI on Intel AI Laptops and Simple LLM Inference on CPU and Fine-tuning of LLM Models using Intel® OpenVINO™". It implements a chatbot using a fine-tuned GPT-2 model for health-related conversations, optimized for efficient inference on Intel CPUs. The project includes data preprocessing, model training, and optimization using OpenVINO, designed to understand and respond to health-related queries based on a custom dataset.

## Installation Instructions
1. Ensure you have Python 3.x installed.
2. Install the required packages:
   ```
   pip install transformers openvino openvino-dev datasets
   pip install pyarrow==14.0.1 requests==2.31.0
   pip install langchain
   pip install torch==2.3.0+cu121 torchvision==0.15.0+cu121 torchaudio==2.2.0+cu121 -f https://download.pytorch.org/whl/cu121/torch_stable.html
   pip install python-libarchive matplotlib-venn pydot cartopy
   pip install accelerate>=0.21.0 -U
   pip install --upgrade transformers
   pip install optimum[openvino]
   ```
3. Install system dependencies:
   ```
   apt install python3.10-venv
   apt-get -qq install -y graphviz
   ```
4. Set up Hugging Face token:
   - Create an account on Hugging Face (https://huggingface.co/) if you don't have one.
   - Generate an access token in your Hugging Face account settings.
   - Set the token as an environment variable:
     ```
     export HUGGINGFACE_TOKEN=your_token_here
     ```
   - Alternatively, you can use the token in your Python script:
     ```python
     from huggingface_hub import login
     login(token="your_token_here")
     ```
   This token is necessary to access and download models from the Hugging Face Model Hub.

## Usage
1. Prepare your dataset:
   - Ensure you have a CSV file named 'intents.csv' with columns 'tag' and 'responses__-'.
2. Train the model:
   - Run the script to fine-tune the GPT-2 model on your dataset.
3. Optimize the model:
   - The script includes steps to optimize the model using OpenVINO.
4. Run the chatbot:
   - Use the provided chatbot loop at the end of the script to interact with the model.

Example command to start the chatbot:
```python
python untitled4.py
```

## Contributing
Contributions to improve the chatbot or extend its capabilities are welcome. Please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature.
3. Commit your changes.
4. Push to the branch.
5. Create a new Pull Request.

## License
This project is open-source. Please ensure you have the necessary rights to use and distribute the dataset and models.

## Authors
- Riya Mehta (2172100)
- Harpreet Singh (2172105)
- Ajay Godara (2172102)
- Amandeep Singh Yadav (2172132)
- Mehak (2172088)

## Acknowledgments
- Mr. Abhishek Nandi Sir(Intel) for guidance and support.
- Mr. Sumeet Bharti Sir(mentor) for mentorship throughout the project.
- Thanks to the Hugging Face team for the transformers library and Model Hub.
- OpenVINO team for the optimization toolkit.
- Intel for providing the AI hardware and software ecosystem.
- Contributors to the various libraries used in this project.
