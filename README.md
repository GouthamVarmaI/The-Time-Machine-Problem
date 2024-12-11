# The Time Machine Problem

## Project Overview
The Time Machine Problem is a project to evaluate LLMs (Language Models) on their understanding of historical texts. The project considers three datasets: American Stories, arXiv Papers, and British Library Books. The project evaluates the LLMs on British Library book data considering the diverse range of topics and languages in the dataset. We propose a new retrieval method "weighted RAG" that leverages the RAG and adds a weighting mechanism to improve the retrieval performance. We evaluate the weighted RAG on three models Mistral-7B, Phi-3 (~4b parameters), and gemma 1b. We show that the weighted RAG outperforms the RAG in terms of retrieval performance in the task of preciting the year of the text improving understanding of the historical texts.


## Project Structure
The project is structured as follows:
- `data_processors`: Contains the datasets used in the project.
- `evaluations`: Contains the evaluation files for the project.
- `notebooks`: Contains the outputs and also the codes.
- `main.py`: The main script to run the project.

## Setup
To set up the project, you need to install the required Python packages:
```bash
pip install -r requirements.txt
```
## Running the Project
To run the project, execute the following command:
```
python main.py
``` 

By default, you will see the randomly selected American stories and arXiv papers, and their visualizations from my runs. If you want to run the arXiv and American Stories data and visualizations, you can do so by uncommenting the relevant lines in `main.py`.

For the arXiv data, you need to download the [arXiv dataset](https://www.kaggle.com/datasets/Cornell-University/arxiv/data) and save it in the `datasets/arxiv` folder before running the project.

For the American Stories data, you need to set the hugging face token "HUGGINGFACE_TOKEN" from [Hugging Face tokens page](https://huggingface.co/settings/tokens) before running the project.

windows:
```
set HUGGINGFACE_TOKEN=<your_token>
```

mac/linux:
```
export HUGGINGFACE_TOKEN=<your_token>
```
