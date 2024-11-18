# Hyperparameter Tuning for SVM on the MNIST Dataset  

This project demonstrates the importance of hyperparameter tuning in improving machine learning model performance. The study focuses on applying grid search and random search techniques to optimize the parameters of Support Vector Machines (SVM) with radial basis function (RBF) kernels, using the MNIST handwritten digit dataset.  

## Project Overview  

Selecting a suitable machine learning algorithm is just one step in completing a machine learning project. To maximize model performance, careful tuning of hyperparameters is essential before deploying the algorithm. This repository documents the process of optimizing SVM hyperparameters to classify the MNIST dataset.  

### Key Components  

1. **Baseline Model (Linear SVM):**  
   - A baseline model using SVM with a linear kernel is trained on a subset of the MNIST dataset.  
   - Its accuracy is evaluated as a reference point for subsequent improvements.  

2. **Improved Model (RBF-SVM):**  
   - SVM with an RBF kernel is implemented to improve upon the baseline model.  
   - This model becomes the focus for hyperparameter tuning.  

3. **Hyperparameter Tuning:**  
   - **Parameters:** The key parameters tuned are:  
     - `C` (regularization parameter)  
     - `gamma` (shape parameter for the RBF kernel)  
   - **Methods:**  
     - **Grid Search:** Explores a predefined range of parameter values systematically.  
     - **Random Search:** Samples parameter combinations randomly within the specified ranges.  

4. **Search Space Definition:**  
   - Logarithmically spaced intervals are used to define the search space for `C` and `gamma`.  
   - Adjustments are made if optimal parameters are found at the search space boundaries.  

5. **Performance Comparison:**  
   - Both grid search and random search are evaluated in terms of computational efficiency (total runtime) and the quality of the optimal hyperparameters found.  
   - The final models are trained using the best parameters identified by each search method.  

6. **Evaluation:**  
   - Model performance with optimal parameters is compared.  
   - Insights are provided on which method (grid search or random search) yields the best results for this dataset.  

### Challenges and Considerations  

- **Subset of Data:** Due to hardware constraints, only 10% of the MNIST dataset is used, demonstrating the trade-offs between computational efficiency and accuracy.  
- **Real-World Relevance:** The project highlights practical issues such as limited time and computational resources when tuning models for real-world applications.  

### Technologies Used  

- **Python:** Programming language for model implementation and tuning.  
- **Scikit-learn:** For SVM implementation, grid search, and random search utilities.  
- **MNIST Dataset:** A well-known benchmark for digit classification.  

## Results and Insights  

- Analysis of the computational cost and effectiveness of grid search vs. random search.  
- Evaluation of the best performing model based on optimized parameters.  

Explore the repository to understand the process, results, and recommendations for hyperparameter tuning in machine learning projects.
