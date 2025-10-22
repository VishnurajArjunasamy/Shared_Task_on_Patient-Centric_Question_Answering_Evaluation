# Evaluation Script for NLP4Health QnA & Summary Evaluation

This repository provides a notebook-based evaluation script for computing key metrics such as **ROUGE**, **BERTScore**, **Exact Match**, **F1**, and **COMET** for multilingual QnA and summary datasets.

---

## Getting Started

### 1. Clone the Repository

``` bash
git clone https://github.com/VishnurajArjunasamy/Shared_Task_on_Patient-Centric_Question_Answering_Evaluation.git
cd Shared_Task_on_Patient-Centric_Question_Answering_Evaluation
```

### 2. Install Dependencies using uv

Install uv (if not already installed)

``` bash
curl -LsSf https://astral.sh/uv/install.sh | sh

Or on Windows PowerShell:
iwr https://astral.sh/uv/install.ps1 -useb | iex
```

```bash
uv venv
source .venv/bin/activate  # (Use `.venv\Scripts\activate` on Windows)
uv pip install -r requirements.txt
```

### 3. Folder Structure

The Prediction Dir foleder structure should follow the below format

<team_name>_<task_name>_<open/close>/
└── English/
    ├── QnA/
    │   ├── <team_name>_<task_name>_<open/close>_<dialogue_id>_QnA.json
    │   ├── ...
    ├── Summary_Text/
    │   ├── <team_name>_<task_name>_<open/close>_<dialogue_id>_SummaryText.txt
    │   ├── ...
    ├── Summary_KnV/
    │   ├── <team_name>_<task_name>_<open/close>_<dialogue_id>_SummaryKnV.json


If the the folder and file structure is different from the above, make sure to edit the evaluation_script.ipynb accordingly.


### 4. Update the Paths

Update the Paths for PRED_DIR, DT_DIR 



