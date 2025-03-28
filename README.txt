Instructions for Running in Inference Mode:

1. Install Required Libraries:
   Run: `pip install torch numpy matplotlib pandas seaborn`

2. Prepare Files:
   Please ensure the following are in the workspace:
   - `code.ipynb` (main notebook)
   - `data/test.csv` (test dataset)
   - `best_model.pt` (pre-trained model weights)

3. Set Inference Mode:
   Open `code.ipynb` and set the following:
   - `ONLY_INFERENCE = True`: This ensures that the code will skip data preview, training, and validation steps, and only execute the inference section to generate predictions for the test dataset.
   - `ROUND_PRED_TO_INTEGER = False`: If you want to round the predicted Rings to the nearest integer during inference, set this to `True`.

4. Run the Notebook:
   Execute all cells in `code.ipynb` using Jupyter Notebook or convert it to a .py:
   `jupyter nbconvert --to script code.ipynb && python code.py`

5. Output:
   Predictions will be saved in `test_with_predictions.csv`.