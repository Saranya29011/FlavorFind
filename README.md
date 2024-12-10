### Requirements:

### **Python Libraries**
1. **Streamlit**: For building the interactive web application.
2. **pymongo**: For connecting to and interacting with MongoDB.
3. **spacy**: For natural language processing (requires the `en_core_web_md` model).
4. **requests**: For API calls to fetch recipes from Edamam.
5. **pandas**: For data manipulation and analysis.
6. **scikit-learn**: For building and evaluating the Naive Bayes classification model.
   - `train_test_split`
   - `TfidfVectorizer`
   - `MultinomialNB`
   - `accuracy_score`
   - `make_pipeline`
7. **re**: For regular expressions to handle negation and excluded ingredients.

### **Other Requirements**
1. **MongoDB**: Local or remote MongoDB server with a database named `s1` and a collection named `recipe` containing recipes.
2. **Edamam API**: API ID and API Key for fetching external recipes.
3. **SpaCy Model**: Install the medium-sized English model `en_core_web_md`:
   ```bash
   python -m spacy download en_core_web_md
   ```

### **Dependencies File (requirements.txt)**
```plaintext
streamlit
pymongo
spacy
requests
pandas
scikit-learn
```

### **Additional Setup**
- MongoDB database should contain recipe data with fields like `recipe_name`, `recipe_type`, `ingredients` (array), and `instructions`.
- Replace placeholders in the code:
  - `EDAMAM_APP_ID` with your Edamam API ID.
  - `EDAMAM_APP_KEY` with your Edamam API Key. 

## Run the Streamlit App


streamlit run app.py

