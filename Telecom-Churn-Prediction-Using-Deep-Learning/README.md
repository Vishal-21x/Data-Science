"Predict which customers are likely to leave the telecom company so the business can take action to retain them."

It's a Telecom Customer Dataset with 7000+ customers containing info like:

1. Demographics → Gender, Age, Partner, Dependents
2. Services → Phone, Internet, Streaming, Security
3. Account info → Contract type, Monthly charges, Payment method
4. Target → Churn (Did the customer leave? Yes/No)


Built a Neural Network model to predict customer churn — meaning:

1. Prepared the data → removed unnecessary columns, converted text to numbers
2. Split the data → 80% to train, 20% to test
3. Built a Neural Network → using TensorFlow/Keras
4. Trained the model → 200 epochs, batch size 32
5. Saved the model → as .keras file to Google Drive
