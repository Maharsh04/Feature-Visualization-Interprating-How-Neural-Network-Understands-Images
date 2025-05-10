# Feature Visualization: Interpretation of How Neural Network Understands Images

This project demonstrates how to visualize the internal convolutional filters of a pre-trained neural network using feature activation analysis. We focus on identifying and interpreting the most activated filters in a specific layer when an input image (e.g., a cat) is fed into the network.

## 🔍 Key Features

- Load and preprocess an input image.
- Compute mean activations for all filters in a specified convolutional layer.
- Select and visualize the top-k filters with the highest activation values.
- Generate feature visualization images using optimization.

## 🖼 Example Output

- Original image.
- Bar chart of mean activations across filters.
- Visualizations of the top-k activated filters.

## 📁 Files

- `cnn_filter_visualization.ipynb`: Main notebook with code and visualizations.
- `Images/cat.jpg`: Input image used for analysis.
- `README.md`: This documentation.

## 🚀 Usage

1. Clone the repository or open the notebook in a Jupyter-compatible environment.
2. Ensure required dependencies are installed:
    ```bash
    pip install torch numpy matplotlib opencv-python
    ```
3. Place your input image in the Images folder.
4. Run the notebook or call the `visualize_features` function and feel free to play and visualize different layers:
    ```python
    visualize_features("Images/cat.jpg", selected_layer=25, top_k=3)
    ```

## 📚 References

- [Feature Visualization – Distill](https://distill.pub/2017/feature-visualization/)
