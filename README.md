
Fuzzy Time Series Markov Chain Model with Tree Partition Method

Overview

This project implements a model that combines a Tree Partitioning Method and a Fuzzy Time Series Markov Chain approach for time series prediction. The goal is to efficiently partition the time series data into intervals, optimize these intervals based on their frequency distribution, and then apply a Markov Chain-based model to predict future values.
Key Components

    TreePartitionMethod:
        Partitions the time series data into intervals.
        Optimizes the intervals by adjusting them according to the data point distribution within each interval.
        Designed to handle time series data for better prediction results.

    FuzzyTimeSeriesMarkovChain:
        Uses the intervals from the TreePartitionMethod to generate predictions for future values in the time series.
        Evaluates the prediction performance using statistical error metrics like RMSE, MAPE, and Thiel's U.

Dependencies

    Python 3.x
    numpy
    pandas
    scikit-learn

You can install the necessary libraries using the following command:

pip install numpy pandas scikit-learn

Parameters

    TreePartitionMethod(data, num_intervals):
        data: A list of time series data.
        num_intervals: Number of intervals to partition the data into.

    FuzzyTimeSeriesMarkovChain(data, intervals):
        data: Time series data used for training the model.
        intervals: Optimized intervals from the TreePartitionMethod used for the fuzzy time series model.

Output

    Optimized intervals for the time series data.
    Future time series predictions.
    Model evaluation metrics: RMSE (Root Mean Squared Error), MAPE (Mean Absolute Percentage Error), and Thiel's U statistic.

Evaluation Metrics

    RMSE: Measures the square root of the average of squared differences between actual and predicted values.
    MAPE: Measures the percentage difference between actual and predicted values.
    Thiel’s U: A relative accuracy measure comparing the accuracy of a forecasting model to a naive forecasting method.

License

This project is licensed under the MIT License. See the LICENSE file for more information.

For dataset

To clarify, the data in the MOISA dataset was indeed curated from the annual statistics books, specifically from Chapter/Section 17 titled "Social Care" during the period 1979-2019. I would like to clarify that the format and structure of the annual books have varied over the years. For instance, the design and chapter layout in the earlier years differ from the current ones. In the 2023 book, the chapters may end at 15, but in previous years, additional sections and chapters were included. From the link I shared, you can download the annual statistics books. However, please note that prior to 2017, you can download the entire book, including all sections and chapters. From 2017 onwards, you are able to download only the specific section that you wish to access.

Additionally, The dataset “Raw_data.xlsx” was indeed curated using the data from these books. To provide more clarity, I am attaching two copies of the annual statistics books from different years, as well as a screenshot from the 2013 edition. This screenshot shows the table from which we collected the data for the period 2003 to 2013, as an example in this driver link: https://drive.google.com/drive/folders/1iI9_36b09lwgnKH02AEFUaqLQVs7WBil?usp=sharing.

 
