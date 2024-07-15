# Health-related Chatbot Project

## Project Title
Health-related GPT-2 Fine-tuned Chatbot with Intel OpenVINO Optimization

## Description
This project caters to the problem statement of “Running GenAI on Intel AI Laptops and Simple LLM Inference on CPU and Fine-tuning of LLM Models using Intel® OpenVINO™”. It incorporates a health-oriented chatbot that is based on a GPT-2 model which is fine-tuned for inference on Intel CPUs. The concept of the project implies data preprocessing, model training and OpenVINO optimization for the search of Health related queries based on a set of heath related data.

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

1. Prepare the dataset:
- Make sure you have a CSV file with the name ‘intents (1).csv’ having two columns: ‘tag’ and ‘responses__-’.
2. Train the model:
- Execute the script to train GPT-2 on your data to get a new model.
3. Optimize the model:
- This plan also involves procedures on how OpenVINO can be used to fine-tune the model.
4. Run the chatbot:
- At the end of the script, incorporate the following chatbot loop to communicate with the model.

## Contributing

The chatbot could be improved or extended and contributions for these purposes are welcomed. Please follow these steps:

1. Fork the repository.
2. Develop a new branch in your feature.
3. Commit your changes.
4. Push to the branch.
5. Open a new Pull Request.

## License
This project is open-source. Make sure you have the rights for using and distributing the data set and the models.

## Authors
- Riya Mehta (2172100)
- Harpreet Singh (2172105)
- Ajay Godara (2172102)
- Amandeep Singh Yadav (2172132)
- Mehak (2172088)

## Acknowledgments

- Special thanks to Mr. Abhishek Nandi Sir(Intel) for his support and guidance.
- Mr. Sumeet Bharti Sir(mentor) for his guidance in the entire project.
- Special thanks to Hugging Face team for the transformers library and Model Hub.
- OpenVINO team for the optimization toolkit.
- Intel for accommodating the company through the provision of AI hardware and software environment.
- The authors of the different libraries used throughout the development of this project.
