# Apache Beam in Colab Demo

## Overview
This repository showcases the capabilities of Apache Beam within a Google Colab environment. We leverage the FIFA ranking dataset to demonstrate various features of Apache Beam.

## Table of Contents
- [Dataset](#dataset)
- [Features Demonstrated](#features-demonstrated)
- [How to Run](#how-to-run)
- [Insights Gained](#insights-gained)
- [Dependencies](#dependencies)
- [References](#references)

## Dataset
- `fifa_ranking.csv`: A dataset containing historical rankings of national football teams.
   - **Source**: [FIFA International Soccer Men's Ranking (1993-Now) on Kaggle](https://www.kaggle.com/datasets/tadhgfitzgerald/fifa-international-soccer-mens-ranking-1993now)

## Features Demonstrated
1. **Pipeline IO**: Demonstrating the reading of data using Apache Beam's `beam.io.ReadFromText` method.
2. **ParDo**: Used for custom row-wise data processing. In our case, to detect significant rank changes.
3. **Composite Transform**: Incorporating a sequence of operations such as reading data, splitting rows, and detecting significant rank changes.
4. **Windowing and Triggers**: Techniques applied to group countries by their confederation and then calculate their average ranks over a set window of time.

## How to Run
1. Upload the `fifa_ranking.csv` dataset to your Colab environment.
2. Execute the Colab notebook sequentially to witness the results of each Apache Beam operation.

## Insights Gained
- Detected countries with notable rank changes.
- Grouped countries by their confederation to discern average ranks within a specified time frame.

## Dependencies
- Apache Beam
- Matplotlib (for visualization purposes)
- Seaborn (for visualization purposes)

## References
- [Apache Beam Documentation](https://beam.apache.org/documentation/)
- [BeamML Documentation](https://beam.apache.org/documentation/ml/about-ml/)
