# Linear Regression: Sports Difficulty Ranking

## Project Goal
Predict the total difficulty score for 60 sports based on 12 characteristics (Endurance, Strength, etc.) using a linear regression model, and compare predicted vs actual ranks.

## Dataset
- CSV: `data/toughestsport.csv`
- Features: 12 characteristics scored 0–10
- Target: Total score (sum of characteristics)
- Derived: Rank (1 = most difficult sport)

## Model
- Linear regression using PyTorch
- Loss: Mean Squared Error (MSE)
- Optimizer: SGD
- Input features normalized only for training stability
- Output: predicted total scores → predicted ranks

## Output
- `outputs/results_table.csv` → Top sports with actual & predicted totals and ranks
- `outputs/feature_importance.csv` → Linear regression weights and importance of each characteristic

## How to Run
1. Place dataset in `data/`
2. Run `src/linreg_sports.py`
3. Check `outputs/` for result tables