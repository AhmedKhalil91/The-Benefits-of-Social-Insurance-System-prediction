
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


