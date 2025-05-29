### Q&A
* **What is the survival rate by passenger class?** First class passengers had the highest survival rate (0.67), followed by second class (0.50), and third class (0.40).
* **What is the survival rate by gender?**  Males had a higher survival rate (0.67) than females (0.25) in this particular dataset slice.  This result might be an artifact of the small dataset.
* **How does family size relate to survival?** Passengers with larger families (4 or more) had a higher survival rate (1.00) in this small dataset.  The 'Small' category (0-1 family member) showed a NaN value, indicating no such passengers in the dataset subset.

### Data Analysis Key Findings
* **Missing Data Imputation:** Missing 'Age' values were filled with the median, 'Embarked' with the mode, and 'Cabin' with 'Unknown'.
* **Feature Engineering:** Created 'FamilySize' and 'Title' features. 'FamilySize' combines 'SibSp' and 'Parch'. 'Title' is extracted from passenger names.
* **Categorical Encoding:**  'Sex', 'Embarked', and 'Title' were one-hot encoded.
* **Survival Rate Discrepancies:**  The small dataset size may be influencing some results, such as the counterintuitive gender-based survival rate and NaN values for certain family size and age categories.  Survival rates varied significantly across passenger class, family size categories, age groups, fare categories, and titles.
* **Correlation Analysis:** A correlation heatmap was generated to visualize relationships between numerical features.


### Insights or Next Steps
* **Investigate Data Imbalance:** The small dataset size and potential for class imbalance should be addressed by using a larger and more representative dataset.
* **Refine Feature Engineering:** Explore additional features or transformations based on domain expertise or more sophisticated feature selection techniques.
