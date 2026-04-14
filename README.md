School of Electronic Engineering and Computer Science

Queen Mary University of London

Project Title: Low-cost Air Quality Sensor Calibration

Supervisor: Professor Stefan Poslad

Student name: Abigail Boatemaa Frimpong

Student e-mail: a.frimpong@se24.qmul.ac.uk

PROJECT AIMS:
Evaluate Performance of Low-Cost Sensors with respect to Medium and High-Cost Sensors Assess the accuracy, repeatability, and sensitivity of low-cost air quality sensors in measuring key pollutants such as PM2.5, PM10, NO₂, CO, VOCs and O₃ under real-world environmental conditions.
To investigate and evaluate methods for improving the data quality of low-cost air quality sensors through calibration against reference-calibrated sensors, using statistical and machine-learning calibration models applied to multi-pollutant datasets from real sensor deployments.

PROJECT OBJECTIVES:

Objective 1 – Data Acquisition and Pre-processing
Extract and clean multi-pollutant datasets from two sensor nodes (Node 3 and Node 5) including low-cost, mid-cost, and high-cost reference channels.
Harmonise timestamps, remove invalid entries, align pollutants across sensor types, and construct pollutant-specific datasets suitable for calibration analysis.

Objective 2 – Develop Calibration Models
Implement and compare multiple calibration approaches:
Linear regression
Second-degree polynomial regression
Random Forest regression
Fit calibration models independently for each pollutant on each node

Objective 3 – Evaluate and Compare Calibration Accuracy
Perform systematic model evaluation using train/validation/test splits (20/20/60).
Compute R², RMSE, residual plots, and 1:1 comparison plots to assess model quality.
Identify which calibration model best improves data quality for each pollutant and node.

Objective 4 – Investigate Cross-Node Transferability
Apply calibration models from Node 3 to Node 5 and vice-versa.
Evaluate performance drop or improvement to assess model generalisability and drift sensitivity.
Analyse whether calibration models trained in one environment remain valid elsewhere.

Objective 5 – Discuss Calibration
Investigate literature findings on calibration drift and environmental sensitivity.

Discuss whether calibration should be performed:
once at installation, periodically

Objective 6 – Draw Conclusions and Provide Recommendations
Summarise observed calibration performance across pollutants and models.

This project definition must be undertaken in consultation with your supervisor. 
The feasibility of the project should have been assessed and the project aims should be clearly defined.
Submission of this document implies that you have discussed the specification with your supervisor.
Provide guidance for future deployments of low-cost AQ sensors.

Recommend best-practice calibration methods for improving AQ data quality in practice.

Problem Definition

Air pollution is a major environmental and public health challenge, yet the monitoring networks used to quantify exposure often rely on expensive, reference-grade air quality (AQ) instruments. These instruments provide high accuracy and long-term stability, but their operational costs, power requirements, and maintenance demands limit their spatial coverage. In contrast, low-cost air quality sensors have gained significant traction due to their affordability and ease of deployment, enabling dense, hyper-local monitoring networks. However, these sensors often suffer from systematic bias, sensor drift, cross-sensitivity to other gases, environmental artefacts (temperature, humidity), and manufacturing variability, all of which degrade data quality.
As demonstrated in multiple field evaluations (Giordano et al., 2021; Huang et al., 2022; Zuidema et al., 2021), raw low-cost sensor measurements cannot be used as direct substitutes for reference-grade measurements. Their outputs typically require calibration, either using traditional statistical models or data-driven machine-learning approaches, to align with reference-calibrated instruments—when such reference instruments are available at all.
A further challenge arises because reference-calibrated sensors are not universally available for all pollutants (e.g., SO₂, VOCs), and even where available, their deployment alongside low-cost nodes may be temporary or intermittent. This raises critical questions about how to best transfer calibration models between nodes, how often calibrations must be updated due to drift, and whether a calibration built at one location remains valid for another.
The core problem, therefore, is the lack of reliable, generalisable calibration strategies that can transform low-cost sensor outputs into high-quality, scientifically usable air quality data across different pollutants and deployment contexts. This project addresses this gap by systematically evaluating calibration models for multiple pollutants across two real-world sensor nodes (Node 3 and Node 5) and assessing their transferability, stability, and utility.

METHODOLOGY:
Data Sources and Sensor Nodes
Sensor Deployment
Data Pre-Processing
Calibration Models
Linear Regression
Polynomial Regression (Second Degree)
Random Forest Regression
Cross-Node Calibration Transfer
Performance Metrics
Calibrated model outputs were evaluated using:
Coefficient of Determination (R²)
Measures proportion of variance explained.
Root Mean Squared Error (RMSE)
Evaluates absolute calibration error in original units (e.g., μg/m³, ppb).
Residual Analysis

REQUIRED KNOWLEDGE/ SKILLS/TOOLS/RESOURCES:

Phython, Google Colab
