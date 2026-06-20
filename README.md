# Consumer Behavior Analysis for Bellabeat Marketing Strategy

## Project Overview

Bellabeat is a wellness technology company that develops smart products designed to help women monitor and improve their health and wellness. The company seeks to better understand how consumers use wearable fitness devices and how those insights can be leveraged to improve marketing strategies and customer engagement.

This project analyzes Fitbit fitness tracker data to identify trends in physical activity, sleep behavior, and overall device usage. The findings will be used to develop actionable recommendations for Bellabeat products and marketing initiatives.

The project follows the Google Data Analytics Case Study framework consisting of the Ask, Prepare, Process, Analyze, Share, and Act phases.

## Business Task

Analyze smart device usage data to identify behavioral trends among wearable device users and determine how those insights can be applied to Bellabeat products and marketing strategies.

### Business Questions

1. What trends exist in smart device usage?
2. How could these trends apply to Bellabeat customers?
3. How could these trends influence Bellabeat's marketing strategy?

## Stakeholders

- Bellabeat Executive Team
- Urška Sršen (Co-founder and Chief Creative Officer)
- Sando Mur (Co-founder)
- Bellabeat Marketing Analytics Team

### Intended Audience

This analysis is intended for business stakeholders who will use the findings to guide marketing strategy and product positioning decisions.

## Data Source

### Primary Dataset

**Dataset:** Fitbit Fitness Tracker Data

**Source:** Kaggle (Mobius)

**License:** CC0 Public Domain

### Description

This project uses Fitbit fitness tracker data made publicly available through Kaggle. The dataset contains activity, sleep, heart rate, and weight-tracking information collected from Fitbit users over multiple collection periods.

During the data inventory phase, two Fitbit exports were evaluated and consolidated into a single master dataset for analysis. The resulting dataset contains daily activity records spanning March 12, 2016 through May 12, 2016.

### Data Limitations

* Relatively small sample size
* Data collected during a limited time period
* No demographic information provided
* Data may not represent the broader wearable device market
* Potential self-selection bias among participants
* Limited ability to generalize findings beyond the study population

### Purpose

The dataset will be used to identify behavioral patterns among wearable device users and develop data-driven marketing recommendations for Bellabeat products.

## Data Inventory & Dataset Selection

### Data Inventory Findings

Two Fitbit exports were evaluated during the data inventory phase:

| Export   | Date Range                      | Users | Records |
| -------- | ------------------------------- | ----- | ------- |
| Export 1 | March 12, 2016 – April 12, 2016 | 35    | 457     |
| Export 2 | April 12, 2016 – May 12, 2016   | 33    | 940     |

Key findings:

* Export 2 contained a more complete collection of activity and sleep-related datasets.
* All 33 users present in Export 2 also appeared in Export 1.
* Only two users appeared exclusively in Export 1.
* The exports shared identical schemas and data types.
* Twenty-four overlapping user-date records were identified on April 12, 2016.
* Overlapping records contained differing activity values between exports.

### Dataset Selection Decision

The two exports were merged into a single master dataset after validating participant overlap, date continuity, schema compatibility, and record integrity.

A detailed review of overlapping records revealed that Export 2 contained more complete activity information for shared user-date combinations. As a result, overlapping records from Export 1 were removed and the corresponding Export 2 records were retained.

### Master Dataset Summary

* Total Records: 1,373
* Unique Users: 35
* Duplicate User-Date Records: 0
* Observation Period: March 12, 2016 – May 12, 2016

The resulting master dataset serves as the primary source for all subsequent analyses and contains 62 days of activity data spanning March 12, 2016 through May 12, 2016.