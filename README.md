# Effective and Ineffective Hockey Shots  
### Analysis of NHL Shot Data (2021–22 Season)

## Background  
Ice hockey is a complex, fast-paced sport influenced by many factors such as player positioning, shot angle, defensive pressure, and game state. The purpose of this project is to analyze shot events from the **2021–22 NHL season** to better understand:

- **What makes a shot effective?**  
- **Which on-ice features and game conditions correlate with a higher probability of scoring a goal?**

The dataset used in this project was obtained from Kaggle:  
**[National Hockey League Shots Dataset](https://www.kaggle.com/datasets/mexwell/national-hockey-league-shots)**

---

## Dataset Features Used  
Below is the list of main features we used in this analysis:

- **description**  
  A detailed string describing the shot event.

- **shot_outcome**  
  The result of the shot. Possible values include:  
  - `GOAL` — the shot resulted in a goal  
  - `MISSED_SHOT` — the shot missed the net  
  - `BLOCKED_SHOT` — the shot was blocked by a non-goalie player  
- **period**  
  Integer value of the game period  

- **home_score**  
  Integer value of the home team score after the event  

- **away_score**  
  Integer value of the away team score after the event  

- **home_name**  
  String name of the home team  

- **event_team**  
  String defining the team taking the shot  

- **empty_net**  
  Boolean indicating if the shot was during an empty net situation, `TRUE` if so, `FALSE` or `NA` if not  

- **x_fixed**  
  Numeric transformed x-coordinate of event in feet (home team always shoots right, away team left)  

- **y_fixed**  
  Numeric transformed y-coordinate of event in feet (home team always shoots right, away team left)  

- **shot_distance**  
  Numeric distance (in feet) to the center of the net for unblocked shot events  

- **shot_angle**  
  Numeric angle (in degrees) to the center of the net for unblocked shot events  

---

## 🛠 Methods  
- Data cleaning and preprocessing  
- Exploratory data analysis    
- Predictive modeling (logistic regression / tree-based models) to estimate goal probability  

---

## Results Summary  
- goal differential and shot distance impacted the liklihood of a goal the most
- tip-ins were the most effective shot type

---

## Open in Google Colab

1. Download the dataset from kaggle: [national hockey league shots](https://www.kaggle.com/datasets/mexwell/national-hockey-league-shots)
   
2. You can now open this notebook directly in Google Colab to run it without installing anything locally.

a. Click the **Open in Colab** badge below:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/charleynas/Effective-and-Ineffective-Hockey-Shots/blob/main/Effective_vs_ineffective_shots (1).ipynb)

b. Alternatively, you can open it manually:
   - Go to [Google Colab](https://colab.research.google.com/)
   - Click the **GitHub** tab
   - Paste this repository URL: `https://github.com/charleynas/Effective_vs_ineffective_shots (1).ipynb
   - Select the notebook you want to open


---
