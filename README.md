# ML-Projects
** Macine Learing Car Price Projection
When you train a LinearRegression model in scikit‑learn, it gives you insight into how your input features influence the target variable (in your case, car Price).

1. The Relationship Between Features and the Target. Linear Regression estimates a line (or hyperplane) that best fits your data.
It tells you:
- How much the price changes when a feature changes. (e.g., every extra year reduces price by X, every extra km reduces price by Y)
- Which features matter more (via the learned coefficients)
- Certain companies tend to have higher/lower prices  
- Certain fuel types influence price  
- Newer cars cost more  
- Less‑driven cars cost more  

2. The Predicted Price for New Inputs. This is the model applying the learned relationships to your input.

3. How Good the Model Is (R² Score of 0.6260966103962277)
This means:
- The model explains about 62.6% of the variation in car prices  
- The remaining 37.4% is noise, missing features, or non‑linear patterns
R² is the main performance metric LinearRegression provides.

4. How Each Feature Contributes (After Encoding)
Your pipeline:
- One‑hot encodes: `name`, `company`, `fuel_type`
- Passes through numeric: `year`, `kms_driven`
LinearRegression then learns:
- Which brands increase price  
- Which fuel types increase price  
- How age affects price  
- How mileage affects price  

This is the core interpretability benefit of linear regression.
