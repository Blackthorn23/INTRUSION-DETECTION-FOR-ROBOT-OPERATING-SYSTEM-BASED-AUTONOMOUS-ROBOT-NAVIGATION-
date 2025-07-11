# FYP: Intrusion Detection for Robot Operating System-Based Autonomous Robot Navigation

Author: Nawfal Syafi' Bin Zailan
Student ID: 1221301208
Faculty: FIST, Multimedia University
Submission: July 2025

================================================================================

## PROJECT DESCRIPTION
This project presents an intelligent intrusion detection system (IDS) built for ROS 1-based autonomous robots, specifically TurtleBot3, enhanced with AI to monitor and detect cyberattacks during real-time navigation. Attacks such as DoS, SSH brute-force, unauthorized publishing/subscribing, and reverse shell attacks were simulated and captured in real environments.

================================================================================

## SYSTEM REQUIREMENTS & TOOLS

### Operating System:
- Ubuntu 20.04 LTS (Recommended)
- Alternative: Ubuntu 18.04 LTS

### Core Software & Versions:
1. **ROS Noetic** (ROS 1)
   - Installation: http://wiki.ros.org/noetic/Installation/Ubuntu
   - Follow the "Desktop-Full Install" option

2. **Python 3.8+**
   - Usually pre-installed with Ubuntu 20.04
   - Verify: `python3 --version`

3. **TurtleBot3 Packages**
   - Installation guide: https://emanual.robotis.com/docs/en/platform/turtlebot3/quick-start/
   - Run: `sudo apt install ros-noetic-turtlebot3*`

### Hardware Requirements:
- **TurtleBot3 Burger** (Physical robot for real-world testing)
- **OAK-D Pro Camera** (Optional - for enhanced sensing)
- **Minimum 8GB RAM** (16GB recommended)
- **Ubuntu-compatible network interface**

================================================================================

## PYTHON LIBRARIES & DEPENDENCIES

### Install Required Libraries:
```bash
# Update system
sudo apt update && sudo apt upgrade

# Install pip if not available
sudo apt install python3-pip

# Install required Python packages
pip3 install pandas==1.3.3
pip3 install numpy==1.21.0
pip3 install scikit-learn==1.0.2
pip3 install matplotlib==3.4.2
pip3 install seaborn==0.11.1
pip3 install jupyter==1.0.0
pip3 install joblib==1.0.1
```

### CICFlowMeter Setup:
1. **Download CICFlowMeter**: https://drive.google.com/drive/folders/1mkWT3tgnr2qXnOkBwgO10VPyjArMNM_5
2. **Setup Tutorial**: https://www.youtube.com/watch?v=EaYyYy9uvt0&t=2s
3. Extract and follow the video instructions for installation

### Wireshark:
# Install wireshark if not available
sudo apt install wireshark

## RosPenTo Tool (ROS penetration testing) setup:
   - A pentest tool for exploring vulnerabilities in ROS nodes, topics, and services  
   - GitHub: https://github.com/jr-robotics/ROSPenTo

================================================================================

## DATASETS USED 

### 1. ROSIDS23 Dataset (Public Dataset)
**Download**: https://zenodo.org/records/10014434

**Setup Instructions:**
1. Visit the Zenodo link above
2. Click "Download all" to get the ZIP file
3. Create folder: `mkdir -p ~/fyp_project/datasets/rosids23/`
4. Extract contents: `unzip ROSIDS23.zip -d ~/fyp_project/datasets/rosids23/`
5. The dataset is already pre-processed in CSV format

### 2. NAVBOT25 Dataset (Self-Collected Dataset)
**Download**: https://zenodo.org/records/15336304

**Setup Instructions:**
1. Visit the Zenodo link above
2. Click "Download all" to get the ZIP file  
3. Create folder: `mkdir -p ~/fyp_project/datasets/navbot25/`
4. Extract contents: `unzip NAVBOT25.zip -d ~/fyp_project/datasets/navbot25/`
5. Use the CSV files directly for training and testing

================================================================================
#SOURCE CODES

## AI MODELS & KAGGLE NOTEBOOKS

### Attack Identification Models (ROSIDS23):
- Mutual Information + Decision Tree: https://www.kaggle.com/code/nawfal24/rosids23-ai-mi-dt
- Mutual Information + Random Forest: https://www.kaggle.com/code/nawfal24/rosids23-ai-mi-rf
- Mutual Information + K-NN: https://www.kaggle.com/code/nawfal24/rosids23-ai-mi-knn
- Chi-Square Test + Decision Tree: https://www.kaggle.com/code/nawfal24/rosids23-ai-cst-dt
- Chi-Square Test + Random Forest: https://www.kaggle.com/code/nawfal24/rosids23-ai-cst-rf
- Chi-Square Test + K-NN: https://www.kaggle.com/code/nawfal24/rosids23-ai-cst-knn
- ANOVA F-Test + Decision Tree: https://www.kaggle.com/code/nawfal24/rosids23-ai-anvt-dt
- ANOVA F-Test + Random Forest: https://www.kaggle.com/code/nawfal24/rosids23-ai-anvt-rf
- ANOVA F-Test + K-NN: https://www.kaggle.com/code/nawfal24/rosids23-ai-anvt-knn

### Attack Classification Models (ROSIDS23):
- Mutual Information + Decision Tree: https://www.kaggle.com/code/nawfal24/rosids23-ac-mi-dt
- Mutual Information + Random Forest: https://www.kaggle.com/code/nawfal24/rosids23-ac-mi-rf
- Mutual Information + K-NN: https://www.kaggle.com/code/nawfal24/rosids23-ac-mi-knn
- Chi-Square Test + Decision Tree: https://www.kaggle.com/code/nawfal24/rosids23-ac-cst-dt
- Chi-Square Test + Random Forest: https://www.kaggle.com/code/nawfal24/rosids23-ac-cst-rf
- Chi-Square Test + K-NN: https://www.kaggle.com/code/nawfal24/rosids23-ac-cst-knn
- ANOVA F-Test + Decision Tree: https://www.kaggle.com/code/nawfal24/rosids23-ac-anvt-dt
- ANOVA F-Test + Random Forest: https://www.kaggle.com/code/nawfal24/rosids23-ac-anvt-rf
- ANOVA F-Test + K-NN: https://www.kaggle.com/code/nawfal24/rosids23-ac-anvt-knn

### Attack Classification Models (NAVBOT25):
- Mutual Information + Decision Tree: https://www.kaggle.com/code/nawfal24/navbot25-ac-mi-dt
- Mutual Information + Random Forest: https://www.kaggle.com/code/nawfal24/navbot25-ac-mi-rf
- Mutual Information + K-NN: https://www.kaggle.com/code/nawfal24/navbot25-ac-mi-knn
- CNN-LSTM Model: https://www.kaggle.com/code/nawfal24/navbot25-ac-cnn-lstm
- CNN-MHA Model: https://www.kaggle.com/code/nawfal24/navbot25-ac-cnn-mha

### Attack Identification Models (NAVBOT25):
- Special AI Model: https://www.kaggle.com/code/nawfal24/navbot25-ai-mi-dt

================================================================================

