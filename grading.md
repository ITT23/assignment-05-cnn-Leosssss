## Liu (5.5/15P)

### 1 Exploring Hyperparameters (2.5/5P)

 * hyperparameter values make sense
   * choosing only one neuron turns the network into a simple function - therefore, your results in this condition are not really surprising
   * the values from 32 to 256 make sense
   * the higher values are way overkill for the problem
   * you get half a point (0.5P)
 * networks were trained correctly
   * yes (1P)
 * there are results
   * yes (1P)
 * report and visualization
   * results regarding accuracy can be found in the notebook...
   * ... but the presentation is not appropriate (0P)
     * the notebook is very long with lots of duplicate code - one single cell for training and a variable for the neuron count would have been sufficient
     * there are individual plots for each condition but there are no aggregated results (e.g. a list of accuracies or a plot with all five accuracy curves)
   * inference time is missing (inference time is the time to make a prediction - not training time)

### 2 Dataset (3/5P)

 * sufficient images captured
   * yes (1P)
 * sufficient images annotated
   * yes (2P)
 * annotations compatible with HaGRID dataset
   * it is "no_gesture", not "no-gesture" so I had to fiddle around a bit to get things working. I wonder how you evaluated it?
   * bounding boxes are shifted - this might have been the fault of the tool, but why did you just accept this instead of correcting it?
   * those are both obvious and easily fixable shortcomings (0P)
 * predictions and confusion matrix

I think you got the task a little bit wrong. The idea was to train a model on the HaGRID dataset and then make predictions on your dataset. However, the test data set used during training has to be a subset of the training dataset. Predictions on your data should be made with the final model after training has finished. And from those predictions, a confusion matrix should have been created and saved.
I can't give you points for that (0P).

### 3 Media Controls (0/5P)

 * three hand poses are tracked and distinguished reliably
 * three media control features implemented
 * mapping works and makes sense
 * low latency

