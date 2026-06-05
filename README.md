# Trossen Dataset Dashboard

Dashboard for analyzing LeRobot/Trossen datasets and monitoring data collection performance.

## Features

* Total recordings
* Total recording time
* Typical episode duration (median)
* Longest and shortest episodes
* Average setup time between episodes
* Total setup time
* Recording utilization
* Episode duration distribution
* CSV export functionality

---

## Installation

Installation only needs to be performed once per computer.

Open a terminal and run:

```bash
python3 -m venv ~/.venvs/trossen-dashboard

source ~/.venvs/trossen-dashboard/bin/activate

git clone https://github.com/YOUR_USERNAME/trossen-dataset-dashboard.git

cd trossen-dataset-dashboard

pip install -r requirements.txt
```

---

## Running the Dashboard

### Option 1: Use the default dataset path

```bash
source ~/.venvs/trossen-dashboard/bin/activate

cd trossen-dataset-dashboard

streamlit run dashboard.py
```

---

### Option 2: Specify a dataset path

```bash
source ~/.venvs/trossen-dashboard/bin/activate

cd trossen-dataset-dashboard

DATASET_PATH="/path/to/your/dataset" streamlit run dashboard.py
```

Example:

```bash
DATASET_PATH="$HOME/.cache/huggingface/lerobot/YourUser/trossen_ai_mobile" streamlit run dashboard.py
```

---

## Exporting Results

Click the **Export CSV** button inside the dashboard.

