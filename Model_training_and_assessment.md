Model Training and Assessment
* Definitions:
	* Model Assessment: process of evaluating a model's performance
	* Model Selection : process of selecting the proper level of flexibility for a model
	* Train Error: Model error when predicting on training data as input
		* Not a reliable indicator of model performance
		* Often much lower than test error
	* Test Error: Model error when predicting using data not used in training
		* Use for model assessment
* Data Selection for Training and Testing Models
	* Train/Test Split
		* Split dataset into training data and test data
			* train model on training set
			* test on test set for model assessment
	* Bootstrap
		* Re-sample dataset with replacement and estimate parameters
			* Replacement: Each time data is sampled, all data is put back in
				and can be sampled again on the next iteration
		* Determine variability in parameter estimates based on
			the resulting estimated parameters from each iteration
			of the bootstrap
	* Cross Validation
		* k - folds: split data into k sets
			* train using k-1 sets
			* test on the remaining set
			* This is process is iterated k times
			* Keep model with lowest test error
* Model Performance Indicators/Visualizations
	* Area Under the Curve (AUC) (Classification)
		* Area under the Receiver Operator Characteristic (ROC)
			* True Positive Rate (Sensitivity) vs. False Positive Rate (Fall-out)
		* Provides a metric of model performance regardless of threshold used in classification
	* Activity Monitoring Characteristic (AMOC)
		* Similar to AUC/ROC, but used for activity monitoring/event detection models
			* Uses a scoring function for the True Positive Rate based on time
			* Uses false alarm rate in place of False Positive 
	* Model Sensitivity Analysis
		* Test all value of a single feature while keeping all other feature values
			stable (at a set quantile value, at the median, etc.)
		* Provides a visualization of how the model reacts when each feature is altered
	
