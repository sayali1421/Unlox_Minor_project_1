# Unlox_Minor_project_1
# GroupDNA – WhatsApp Group Analytics

A Python-based project that analyzes a WhatsApp chat export and converts raw chat messages into a clean report showing group activity, word usage, response patterns, silent periods, and participant behavior.

## Project Overview

**GroupDNA** analyzes a WhatsApp `.txt` chat export and finds useful patterns from the conversation.

The project was tested on a dataset containing **3,127 messages from 6 participants**.

The analysis includes:

* Group overview
* Messages per participant
* Busiest day
* Busiest hour
* Top words
* Response time
* Silent streaks
* NumPy activity heatmap
* Personality archetypes
* Participant profile

##  Output Screenshot
<img width="431" height="633" alt="Screenshot 2026-08-21 144439" src="https://github.com/user-attachments/assets/bf07f76e-ed38-49e1-871a-82fdc3bef061" />
<img width="382" height="602" alt="Screenshot 2026-08-21 144503" src="https://github.com/user-attachments/assets/7bfbd9c2-7271-444c-bda4-a40fa98a59f8" />
<img width="463" height="197" alt="Screenshot 2026-08-21 144524" src="https://github.com/user-attachments/assets/ff36a937-de02-4c6c-aef0-c66b8c5ef8b1" />

##  Technologies Used

* Python
* NumPy
* Jupyter Notebook / Google Colab

##  Project Constraints

This project was intentionally developed using basic Python concepts and NumPy.

### Not Used

* ❌ Pandas
* ❌ Matplotlib
* ❌ Regular Expressions (`re`)

The activity heatmap is created using a **NumPy matrix** instead of a visualization library.

## 🔍 Main Features

### 1. WhatsApp Chat Parser

Reads the exported `.txt` file and extracts:

* Date
* Time
* Participant name
* Message text

It also handles unwanted entries such as system messages, deleted messages, and media placeholders.

### 2. Group Overview

Shows:

* Total messages
* Number of participants
* Date range
* Messages sent by each participant

### 3. Activity Analysis

Finds:

* Busiest day
* Busiest hour
* Participant activity by hour

### 4. Top Words

Counts frequently used words after removing common stop words.

### 5. Response Time

Calculates the average response time for participants based on consecutive messages from different participants.

### 6. Silent Streaks

Finds periods where participants were inactive.

### 7. NumPy Activity Heatmap

Creates a **participant × hour activity matrix using NumPy**.

The matrix is displayed as a simple text-based heatmap.

### 8. Personality Archetypes

Assigns one behaviour-based archetype to each participant using rules based on their messaging activity.

### 9. Participant Profile

The final profile shows:

| Participant | Messages | Contribution | Response Time | Peak Hour |
| ----------- | -------: | -----------: | ------------: | --------: |
| Participant |    Count |            % |       Minutes |      Hour |

## ▶️ How to Run

### Step 1 – Download the Repository

Clone or download this repository to your computer.

### Step 2 – Keep the Files Together

Make sure the project files are in the same folder:

```text
GroupDNA/
│
├── GroupDNA.ipynb
├── GroupDNA_privacy_variant.txt
├── groupdna_output.png
└── README.md
```

### Step 3 – Open the Notebook

Open `GroupDNA.ipynb` using:

* Jupyter Notebook
* JupyterLab
* Google Colab

### Step 4 – Run the Notebook

Run the cells from top to bottom.

The chat file should be available in the same working environment as the notebook.

### Step 5 – View the Output

The notebook prints the complete GroupDNA report in the output section.

##  Example Results

The analyzed dataset contains:

* **3,127 messages**
* **6 participants**
* **01/04/2024 – 30/05/2024**
* **Busiest day:** 04/05/2024
* **Busiest hour:** 18:00 – 18:59

The participant analysis also identifies contribution percentage, response time, peak activity hour, and a behaviour-based archetype.

##  What I Learned

Through this project, I practiced:

* Reading and cleaning raw text data
* File handling in Python
* Working with strings
* Lists and dictionaries
* Date and time calculations
* Basic data analysis
* NumPy arrays and matrices
* Designing readable console output
* Handling messy real-world chat data

##  Project

**Project:** GroupDNA – WhatsApp Group Analytics
**Language:** Python
**Main Library:** NumPy
**Project Type:** Data Analysis / Python Mini Project

