**<h1><p align="center">Visualising Netflix Data Using Amazon QuickSight</p></h1>**

**Project Overview**

This project demonstrates how to analyze and visualize Netflix data using Amazon QuickSight, leveraging the power of AWS services to create insightful dashboards. The primary focus is to visualize trends in Netflix's catalogue of TV shows and movies, exploring their release years, categories, and other metadata.

**AWS Services Used:**

**Amazon S3:** For storing the dataset.

**Amazon QuickSight:** For analyzing and creating visualizations.

**Steps to Recreate the Project**

**1. Upload Dataset to S3 Bucket**

Download the dataset (netflix_titles.csv) and manifest file (manifest.json).

Log in to your AWS Management Console.

Create an S3 Bucket with a unique name (e.g., quicksight-netflix-project).

Upload netflix_titles.csv and the manifest.json file to your S3 bucket.

Copy the S3 URL of the netflix_titles.csv file and update the manifest.json file with the correct URL.

**2. Create an Amazon QuickSight Account**

Go to Amazon QuickSight in your AWS account.

Sign up for the free trial (Enterprise edition) and ensure that the email matches your AWS account.

Enable permissions for your S3 bucket in QuickSight settings.

**3. Connect Dataset to QuickSight**

In QuickSight, navigate to Datasets > New Dataset.

Select S3 as the data source and provide a source name (e.g., kaggle-netflix-data).

Paste the updated manifest.json file URL from your S3 bucket.

Click Connect to load the dataset into QuickSight.

**4. Create Visualizations in QuickSight**

Open the dataset in QuickSight and select Visualize.

Drag and drop fields from the dataset to create different types of charts, including:

Bar Chart: Count of TV shows/movies by release year.

Donut Chart: Distribution of TV shows vs. movies.

Table: Listing of TV shows and movies per release year.

Stacked Bar Chart: Percentage breakdown of TV shows and movies by year.

Date Analysis: Identify the day Netflix added the most titles (e.g., January 1, 2020).

**5. Apply Filters and Experiment with Visualizations**

Use filters to refine data for specific use cases:

Filter by release year (e.g., 2015 or later).

Filter by categories (e.g., "Action & Adventure," "Thrillers," "TV Comedies").

Experiment with visualization types (e.g., bar charts, pie charts, and tables).

**6. Publish the Dashboard**

Combine all charts into a cohesive dashboard.

Edit chart titles to make the insights clear.

Publish and export the dashboard for sharing.

**Key Insights from the Dashboard**

**Release Trends:** Visualized the count of Netflix titles by release year.

**Category Breakdown:** Identified the most popular categories, such as "Action & Adventure" and "TV Comedies."

**Date Analysis:** Found that Netflix added the highest number of titles on January 1, 2020.

**Category Filters:** Analyzed specific categories and their contribution to the Netflix catalogue.

**How to Run the Project Locally**

1. Download the dataset (netflix_titles.csv) and manifest.json file.

2. Upload both files to an S3 bucket in your AWS account.

3. Configure Amazon QuickSight to connect to the dataset via the manifest.json URL.

4. Use the QuickSight interface to create visualizations.

**Example Visualizations**

Bar Chart: Number of titles released per year.

Donut Chart: Percentage of TV shows vs. movies.

Table: Count of titles in specific categories.

Stacked Bar Chart: Distribution of TV shows and movies across years.

**Summary**

In this project, I:

🪣 Uploaded the Netflix dataset to an S3 bucket.

🔗 Connected the dataset to Amazon QuickSight.

📊 Created insightful graphs, charts, and dashboards to analyze Netflix trends.

💄 Published a dashboard that highlights valuable insights into the Netflix catalogue.

This project showcases my ability to work with AWS services, analyze datasets, and create professional dashboards using Amazon QuickSight.

