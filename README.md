# The Time Machine Problem

## Project Overview
This project analyzes historical text data across different time periods. It utilizes datasets from arXiv papers (post-1900), British Library Books (1500-1900), and American stories to visualize and understand trends over time.

## Project Structure
- `data_processors/`: Contains modules for processing different datasets.
  - `americanstories/`: Processes American stories from various periods.
    - `americanstories.py`: Processes American stories from [American Stories](https://huggingface.co/datasets/dell-research-harvard/AmericanStories).
    - `selected_stories/`: Contains randomly selected American stories output.
  - `arxiv/`: Processes academic papers from the arXiv repository.
    - `arxiv.py`: Processes academic papers from [arXiv](https://www.kaggle.com/datasets/Cornell-University/arxiv/data).
    - `selected_papers/`: Contains randomly selected arXiv papers output.
  - `britishlib/`: Processes historical books from British Library.
    - `british.py`: Processes books from [British Library Books](https://huggingface.co/datasets/TheBritishLibrary/blbooks).
    - `selected_british_books/`: Yet to run!
- `main.py`: The main script to run analyses.

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
