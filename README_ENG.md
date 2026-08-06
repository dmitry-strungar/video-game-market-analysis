# Game Analytics Dashboards 

## Project Overview
Interactive Tableau dashboards for analyzing video game sales, genre trends, and platform performance.  
The project helps identify key revenue drivers, popular genres, and regional market differences to support business decisions in the gaming industry.

## Business Context

A game publisher needs to understand:

- Which game genres generate the most revenue
- Which platforms dominate in different regions
- How sales trends change over time
- Which games and publishers perform best

The analysis supports portfolio strategy, marketing focus, and platform prioritization.

## Objectives

- Analyze global and regional game sales
- Identify top-performing genres and platforms
- Compare sales across regions (NA, EU, JP, Other)
- Detect long-term sales trends
- Identify top games and publishers by revenue

## Dashboard Features

The Tableau dashboards include:

- Total sales overview
- Sales by platform
- Sales by genre
- Regional sales comparison
- Top games ranking
- Time series analysis of game releases and sales

Interactive filters allow exploration by:

- Year  
- Platform  
- Genre  
- Region  
- Publisher  

## Analytical Approach

- Aggregation of sales metrics
- Dimensional analysis by genre, platform, and region
- Trend analysis over time
- Ranking analysis for top performers
- Interactive visual exploration using Tableau

## Key Insights

### Genre Structure

- Action and Shooter dominate PS4 sales in North America, generating over 60% of total revenue.
- Shooter shows the highest average revenue per title (~0.75M).
- Sports ranks third (~17-18%), but the segment is highly franchise-driven.
- Niche genres (Strategy, Puzzle, Simulation) contribute a minimal revenue share.

### Regional Distribution

- North America (~284M) and Europe (~271M) are the largest markets.
- Together they generate more than 70% of global sales.
- Japan (~93M) represents a smaller but structurally different market.

### Platform Dynamics

- PS4 is the leading platform of the generation (~288M global sales).
- Sales peaked around 2015 (~42M in North America) and declined afterward.
- Lifecycle effects should be considered when planning releases.

### Market Characteristics

- Revenue distribution is highly skewed: a small number of titles generate a large share of total sales.
- Correlation between critic scores and sales is weak (R² ≈ 0.17).
- Commercial performance depends on marketing, IP strength, and release timing in addition to quality.

## Business Value
Identifies most profitable genres and platforms  
Highlights regional differences in revenue distribution  
Detects lifecycle trends across console generations  
Supports strategic decisions in game publishing and investment  

## Stakeholders
Game Publishers  
Marketing Teams  
Product Managers  
Investors  

## Stack of AI tools
During the work on the project, AI tools were used to accelerate development and improve the effectiveness of analytics.:

ChatGPT was used for:
1) Generating drafts of calculated fields to calculate the average revenue per game by genre and platform, as well as ranking top publishers by global sales
2) Prototyping the logic of comparing regional sales (NA, EU, JP, Other) and calculating the shares of each region in the total market volume
3) Search for ideas for visualizing the lifecycle of platforms (combining time series of sales with filtering by console generations)

DeepSeek was used for:
1) Improvements and optimizations of tabular calculations (checking the correctness of calculating cumulative totals by year, eliminating errors when filtering by region)
2) Checking the logic of identifying the correlation between critics' ratings and sales (R-squared calculation, interpretation of weak coupling)
3) Preparing descriptions of key insights for dashboard documentation (structuring conclusions based on genre trends, regional differences, and platform lifecycle)

All the key steps - designing the dashboard structure, configuring filters, visualizing and interpreting the results - were performed independently. AI was used as a tool to accelerate the development and verification of hypotheses.

## Tech Stack

- Tableau
- Excel
- Data Visualization  
- Exploratory Data Analysis

## How to Use

1. Download the `.twbx` file from the `dashboards` folder
2. Open it in Tableau Desktop or Tableau Public
3. Use filters to explore the data interactively

## Limitations

- Analysis is based on historical sales data only
- No user-level behavioral data available
- Does not include marketing spend or pricing data
- Some platforms have limited observations
