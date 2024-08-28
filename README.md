# Music-Genre-Classification-CNN
## Data
GTZAN is a dataset that contains 1000 music experts from 10 different genres (hip hop, jazz, etc.) each one of them is 30 seconds long.
Data are seprated to 2 csv files, have the features of each track in the data. `features_30_sec` have the feature of every 30 second track, `features_3_sec` have the same tracks, but every track is devided to 10 rows, every row holds 3 seconds of the track.
## Libraries
* **NumPy:** Fundamental package for numerical computations.
* **Pandas:** Powerful data analysis library.
* **Matplotlib:** Plotting library for creating visualizations.
* **Seaborn:** High-level data visualization library.
* **Scikit-learn:** Popular machine learning library.
* **TensorFlow:** Open-source deep learning framework.
* **Keras:** High-level API for building neural networks.
* **Librosa:** Python library for music and audio analysis.
## Code
### Data Preprocessing

1. **Load and Combine Data:**
   - Loads audio features from CSV files.
   - Combines data from 3-second and 30-second features.

2. **Label Encoding:**
   - Creates dictionaries to map genre names to numerical indices and vice versa.
   - Encodes labels in the DataFrame.

3. **Feature Scaling:**
   - Scales features using standard scaling to normalize data.

4. **Data Splitting:**
   - Splits data into training, validation, and test sets, ensuring class distribution is maintained.

### Model Building and Training

1. **Define Model Architecture:**
   - Creates a sequential neural network with multiple dense layers and dropout for regularization.
   - Uses softmax activation in the final layer for multi-class classification.

2. **Compile Model:**
   - Sets optimizer (e.g., Adam), loss function (sparse categorical cross-entropy), and metrics (accuracy).

3. **Train Model:**
   - Trains the model on the training set, validating on the validation set.
   - Plots training and validation loss/accuracy curves.

### Evaluation

1. **Evaluate Model:**
   - Evaluates the trained model on the test set to assess performance.
