	README

	Environment Set Up
		- Use the Docker container containing Jupyter Notebook from the earlier Labs

	Usage

	Preprocess
		- Data was processed with Regex to remove urls, digits, html tags, punctuation 
		- text converted to lowercase

	Feature Extraction
		- TFIDF used to vectorize data from text to term frequency attributes
		- Count Vectorizer was used to extract attributes from data in boolean form (0 if term absent 1 if present)
		- Create copy of data and remove stopwords, use stemmer

	Naive-Bayes
		- MultinomialNB run on Term Frequency attributes on TFIDF vector of unstemmed data
		- Hyperparameter tuning with grid search was performed
		- Results visualized

		- MultinomialNB run on Term Frequency attributes on TFIDF vector of stemmed, stop word removed data
		- Hyperparameter tuning with grid search was performed
		- Results visualized

		- MultinomialNB run on CountVectorized stemmed, stop word removed data
		- Hyperparameter tuning with grid search performed
		- Results visualized
	
	Random Forest
		*
	
	SVM
		- Co-locate `enron_spam_data.csv` with the `project_svm-linear.ipynb` and `project_svm-rbd.ipynb` notebook files
		- SVM with Linear Kernel
			- Run each section sequentially up to and including the section containing `# Define the target variable`
			- Run either the section with the 200MB cache size or the section with the 1000MB cache size
			- Continue running each section sequentially to get and visualize the results
		- SVM with Radial Basis Function (RBF) Kernel
			- Run each section sequentially up to and including the section containing `# Define the target variable`
			- Skip running the next two sections for running and evaluating the RBF kernel with a C value of 0.75
			- Run the section for the RBF kernel with a C of 1.0 and its following evaluation section
			- Skip running the next two sections for running and evaluating the RBF kernel with a C value of 1.25
			- Continue running each section sequentially to get and visualize the results
   
