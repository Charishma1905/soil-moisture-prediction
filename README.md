Phase 1: Baseline Model Development

Objective: Establish a simple predictive pipeline for soil moisture using basic environmental features.

Data Preparation:

Used a simulated dataset with Temperature (°C) and Humidity (%).

Preprocessed and split data into training and testing sets (80/20).

Modeling Approach:

Implemented Linear Regression as the baseline model.

Trained and evaluated the model to check feasibility of prediction.

Evaluation:

Metrics used: R² Score, RMSE, MAE.

Achieved moderate accuracy, showing soil moisture can be predicted but with limited precision.

Key Output:

Proof-of-concept that environmental factors (temp & humidity) can be used for soil moisture prediction.

Established the foundation for more advanced models in Phase 2.
<img width="1920" height="937" alt="1" src="https://github.com/user-attachments/assets/64ad2f01-d987-4124-b61e-765b862e9723" />


🔹 Phase 2: Advanced Modeling & Insights

Objective: Improve prediction accuracy by expanding the dataset and applying advanced ML algorithms, while aligning with sustainable agriculture practices.

Dataset Expansion:

Added Rainfall (mm) as an additional feature.

Normalized features using StandardScaler for consistent training.

Modeling Approach:

Trained and compared three models:

Linear Regression (baseline)

Random Forest Regressor

XGBoost Regressor

Used the same train/test split for fair comparison.

Evaluation:

Compared using R² Score, RMSE, MAE.

Results showed that Random Forest and XGBoost significantly outperformed Linear Regression.

Visualizations:

Soil Moisture vs Temperature, Humidity, Rainfall.

Predicted vs Actual values for each model.

Impact Assessment:

Applied an irrigation threshold: if soil moisture < 30%, irrigation is required.

Best-performing model correctly identified irrigation needs with ~XX% accuracy (replace with your result).

Demonstrates potential for water conservation in smart farming.

Lifecycle Alignment:

✅ Data Collection & Preprocessing

✅ Advanced ML Modeling

✅ Model Evaluation & Visualization

✅ Early Impact Assessment

Key Output:

Identified XGBoost/Random Forest as the most reliable models.

Delivered insights that connect prediction accuracy with real-world water-saving benefits, paving the way for Phase 3 (sensor integration and deployment).
<img width="1920" height="947" alt="2" src="https://github.com/user-attachments/assets/9258c0b1-70b0-42e2-b8e2-ace31ae42e45" />
<img width="1920" height="908" alt="3" src="https://github.com/user-attachments/assets/b53a3ebc-eea8-42f4-ae10-5341240d656a" />
<img width="1920" height="921" alt="4" src="https://github.com/user-attachments/assets/a6f335c5-6ece-46a0-9664-f0d57990661a" />



🔹 Phase 3: Real Sensor Integration & Deployment (Future Work)

Objective: Connect real-world hardware sensors with the trained ML model to enable live soil moisture prediction and automated irrigation decisions.

Sensor Hardware Setup:

Use Soil Moisture Sensors (Capacitive/Resistive) for direct soil readings.

Integrate DHT11/DHT22 sensors for temperature and humidity.

Optionally include Rain Gauge / API weather data for rainfall input.

Microcontroller: Arduino / ESP32 / Raspberry Pi to collect and transmit data.

Data Flow:

Sensors → Microcontroller → Data Transmission (via Wi-Fi/Serial) → Python Backend.

Pretrained ML model predicts soil moisture level and irrigation requirement.

Deployment Approach:

Develop a dashboard/web app to display live soil readings and predictions.

Implement threshold-based alerts: e.g., if soil moisture < 30%, send irrigation notification.

Optional automation: trigger relay module to control a water pump for smart irrigation.

Impact & Sustainability:

Ensures real-time decision-making for farmers.

Reduces over-irrigation and water waste.

Moves project from simulation → real-world IoT application.

Future Enhancements:

Cloud storage of sensor data for long-term trend analysis.

Mobile app integration for farmer-friendly use.

Integration with solar-powered systems for sustainable deployment.
<img width="1920" height="1037" alt="5" src="https://github.com/user-attachments/assets/713c3b23-0dea-4cc0-ac31-4f1300fc6fd8" />
<img width="1920" height="1064" alt="6" src="https://github.com/user-attachments/assets/68f80a8f-8fb1-4679-95b9-b7cacd529dfb" />
<img width="1920" height="1027" alt="8" src="https://github.com/user-attachments/assets/fff2ed36-c218-4401-8fa1-88b7feb0d715" />



