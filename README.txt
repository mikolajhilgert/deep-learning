Instructions for Running in Inference Mode:

1. Prepare Files:
   Please ensure the following are in the workspace:
   - `code.ipynb` (main notebook)
   - `data/test.csv` (test dataset)
   - `best_model.pt` (pre-trained `best` model weights)

2. Set Inference Mode:
   Open `code.ipynb` and set the following at the beginning of the notebook:
   - `ONLY_INFERENCE = True`: This ensures that the code will skip data preview, training, and validation steps, and only execute the inference section to generate predictions for the test dataset.
   - `ROUND_PRED_TO_INTEGER = False`: If you want to round the predicted Rings to the nearest integer during inference, set this to `True`.

3. Run the Notebook:
   Execute all cells in `code.ipynb` using Jupyter Notebook.

4. Output:
   Predictions will be saved in `test.csv`.