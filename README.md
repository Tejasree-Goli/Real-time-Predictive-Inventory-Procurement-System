### Real-time Predictive Inventory Procurement System

This project is part of the job simulation focused on AI for Cognizant’s Data Science team on Forage.


<h4> <b>Project Summary:</b> </h4>
<ul>
  <li> Conducted exploratory data analysis using Python and Google Colab for one of Cognizant’s technology-led clients, Gala Groceries. </li>
  <li> Prepared a Python module that contains code to train a model and output the performance metrics for the Machine Learning engineering team. </li>
  <li> Communicated findings and analysis in the form of a PowerPoint slide to present the results back to the business. </li>
</ul>


<h4><b>Project Background:</b></h4>
Gala Groceries is a technology-led grocery store chain based in the USA. They pride themselves on providing the best quality, fresh produce from locally sourced suppliers. Groceries are highly perishable items. If you overstock, you are wasting money on excessive storage and waste, but if you understock, then you risk losing customers. They use sensors to measure temperature storage facilities where products are stored in the warehouse, and they also use stock levels within the refrigerators and freezers in store. They want to know how to better stock the items that they sell.


<h4><b>Project Goal:</b></h4>
Accurately predict the stock levels of products based on sales data and sensor data on an hourly basis in order to more intelligently procure products from suppliers.


<h4><b>Implementation:</b> </h4>

**Task - 1**

1. Collect a sample dataset from Data Engineering team for the given problem statement.
   
2. Load the data into Google Colab and start performing exploratory data analysis.
    <ul>
      <li> Understand the features of data.</li>
    </ul>
3. Conduct Statistical Analysis
    <ul>
      <li> This helps is understanding the numerical features and the distribution of values.</li>
    </ul>
4. Initial Visualization
    <ul>
      <li> Play with various visualizations to understand the correlation between different features and significance of specific features.</li>
    </ul>
5. From the initial analysis of the data:
    <ul>
      <li> Document summary of the analysis</li>
      <li> Come up with questions or further requirements needed to proceed with the project</li>
      <li> Report these to the team leader and business stakeholders.</li>
    </ul>

**Task - 2**

1. Collect complete data from the client through data engineering team.
     <ul>
       <li> Validate with data models to ensure all data is provided that is required to solve the problem statement.</li>
     </ul>
2. Perform Data Cleaning
     <ul>
       <li> Check for null and missing values</li>
       <li> Check if the datatypes are correct -  The datatype for timestamp is transformed in this project</li>
     </ul>
3. Merge different tables into a single data frame
     <ul>
       <li> To tain a machine learning model, we have to perform feature engineering by extracting and transforming the features from all tables into one data frame.</li>
       a. Converted the timestamp in all tables into common hourly timestamp format as per the given problem.
       
       b. Aggregated the columns
   
       c. Combine the features
     </ul>
5. Conduct Feature Engineering
     <ul>
       <li> Transforming features into format suitable for training the machine learning model.</li>
           a. In this project, we are considering numerical columns for the analysis
       
           b. Transformed timestamp column
   
           c. Converted category columns into numerical by using dummy variables
   
           d. Dropped product_id column as it does not add value to the analysis.
     </ul>
7. Modeling
     <ul>
       <li> Install all the required libraries</li>
       <li> A supervised machine learning model - Random Forest Regressor is used in this project</li>
       <li> K-fold strategy is used for training the model</li>
       <li> mae (mean absolute error) and Accuracy metrics are used for measuring the performance the trained ML model</li>
     </ul>
5. Analyze results
    <ul>
      <li> Analyze the results of the trained machine learning model: </li>
        - what is accuracy? 
      
        - how is the model performing?
   
        - what can be concluded based on the performance?
   
        - What are thre recommendations?
    </ul>


**Note:** The python notebooks have detailed comments for each code block to make it readale and understandable.

**Task - 3**
1. After the conclusions are drawn from the model, sumamrize them and present it to the team leader.
2. If everything is approved, develop standard .py code file to provide the machine learning engineering team.
    <ul> 
      <li>The MLE team, optimizes the code to make it production ready and deploys it for testing with real-time data </li>
      <li> After monitoring the performance of the model, with the live data - the MLE team either approves the submission and continues to monitor its performance or gets back to the individual with their observations and recommendations on how we can improve the performance of the model. </li>
    </ul>
