Abstract:
 Always while using public transport people face the issue with danger of pick pocketing and there is no direct way to identify pick pocketing person. So using Automated Fare Collection and Transit Record dataset which consists passenger travelling routes and by analysing person travelling behaviour that identify whether the person is normal passenger or a pick pocketing suspect. 
 To detect person abnormal behaviour, patterns employing Two-Step SVM which analysing person behaviour by using travelling frequency and Short Rides. If person has too many travelling frequency with short rides then that person will be pick pocketing suspect. So first , applying Two-Step algorithm to identify person behaviour and then employing SVM algorithm on person behaviour to calculate suspect prediction Precision and  FSCORE. 


User Manual:
 
 1. Introduction
This user manual provides step-by-step instructions on how to install, configure, and use the "Catch Me If You Can" system for detecting pickpocket suspects in public transportation networks using large-scale transit records.

2. System Requirements
To successfully run this project, ensure your system meets the following requirements:
•	Operating System: Windows 10 or later
•	Processor        : Intel Core i5 or higher
•	RAM            : 8GB or more
•	Storage          : At least 1GB of free space
•	Python Version  : Python 3.7.0 (required for compatibility)
•	IDE             : Visual Studio Code (recommended for viewing and editing code)

3. Required Libraries Installation
Before running the project, install the required Python libraries using the following commands:
pip install pandas
pip install numpy
pip install scikit-learn
pip install matplotlib
pip install plotly
pip install tk
These commands will install all necessary dependencies for running the project.

4. Technologies Used
•	Programming Language: Python
•	GUI Framework: Tkinter
•	Machine Learning Libraries: Scikit-learn
•	Data Processing: Pandas, NumPy
•	Visualization: Matplotlib, Plotly

5. Steps to Run the Project
1.	Download or clone the project repository
2.	Install the required dependencies using the above pip install commands
3.	Run the application using:
       run.bat
4.	The GUI window will open, allowing users to interact with the system.
  
6. Features and Functionalities
I.	Upload Transit Dataset
Users can upload the transit dataset, which contains passenger movement records, to the application for analysis.
II.	Data Preprocessing
•	Removes unnecessary attributes like pickup_datetime, dropoff_datetime, etc.
•	Filters data based on Passenger ID.
•	Normalizes the dataset for better model performance.
III.	Run One-Class SVM Detection
•	Detects potential pickpocket suspects based on an anomaly detection algorithm.
•	Predicts whether a passenger is suspicious or non-suspicious.
IV.	Run Two-Step SVM (TS-SVM) Detection
•	First applies Local Outlier Factor (LOF) for anomaly detection.
•	Then applies SVM-based classifiers for better accuracy.
•	Also provides a map-based visualization of suspect movements.
V.	Model Evaluation
•	Calculates performance metrics such as Accuracy, Precision, Recall, and F1-Score.
•	Compares different machine learning models for best performance.
VI.	Visualization & Graphs
•	Generates bar charts to compare the effectiveness of different classification models.
•	Displays a geo-map of passenger trips using Plotly.
VII.	Exit Application
•	Closes the application safely when the user clicks the Exit button.

7. Screens Explanation & Functionality
1.	Main Window: Displays the available features like dataset upload, preprocessing, and model execution.
2.	Dataset Upload Screen: Allows users to select and upload transit data.
3.	Preprocessing Screen: Displays the processed dataset and normalization status.
4.	Model Execution Screen: Shows buttons to run One-Class SVM and TS-SVM models.
5.	Visualization Screen: Displays model accuracy comparison graphs and geo-map plots.
6.	Results Screen: Presents suspect identification results.

8. Troubleshooting Common Issues
i.	 Python Version Compatibility Error
•	Ensure you have installed Python 3.7.0 as other versions may cause compatibility issues.
python --version
•	If a different version is installed, download and install Python 3.7.0 from the official Python website.
ii.	Missing Dependencies
•	If any module is missing, manually install it using pip install <module_name>.
iii.	Application Not Launching
•	Ensure all dependencies are installed correctly.
•	Run the application with run.bat instead of directly executing Python scripts.




