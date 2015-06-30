* Bagging (bootstrap aggregation) 
	* used to decrease variance in decision trees
	* How it works:
		* train multiple trees using bootstrapped datasets
		* regression trees: average the predictions from all the trees
		* classification: take a majority vote of the predictions
			* majority vote: the class which occurs most frequently
	* Out of bag (OOB) error
		* Only a portion of the data is used to train each tree
		* The remaining data which wasn't selected can be used 
			to assess the tree's performance
			* (the response for each observation is predicted using
				only the trees that were not fit using that observation)
* Boosting
	* How it works:
		* Similar to bagging, but trees are grown sequentially
			* Each tree is created using information from previously grown trees 
* Random Forest
	* Build a number of decision trees using bootstrapped samples
	* At each split in the tree only a portion of the features are considered
		* a feature is selected from a subset of features not the whole feature space
		* the subset is usually sqrt(n.features)
	* This allows trees to be built without some of the strong features
		* decorrelates the trees, unlike bagging
