# CogniStream – Developer Flow-State & Cognitive Load Analytics

## Project Overview

CogniStream is a Developer Experience (DevEx) analytics platform designed to analyse engineering workflows, identify productivity friction, and understand the impact of frequent context switching on uninterrupted development time.

Traditional engineering productivity metrics, such as lines of code, commits, and completed tickets, primarily measure output rather than the quality of the development process. CogniStream addresses this limitation by integrating timestamped activity events from multiple developer tools, including GitHub, Jira, Slack, and VS Code ActivityWatch.

Using workflow orchestration, high-performance data processing, and analytical queries, the platform identifies interruption patterns, estimates context-switching overhead, and measures uninterrupted development sessions through observable activity indicators.

The processed insights are presented through an interactive dashboard, enabling engineering managers to identify workflow bottlenecks and make informed decisions about notification policies and developer experience improvements.

## Key Features

- **Multi-Source Data Ingestion:** Collects developer activity events from GitHub, Jira, Slack, and ActivityWatch.
- **Workflow Orchestration:** Uses Apache Airflow to schedule, automate, and monitor data extraction pipelines.
- **High-Performance Data Processing:** Leverages Python and Polars to clean, standardise, and transform heterogeneous event logs.
- **Analytical Data Storage:** Uses ClickHouse to store and query large volumes of timestamped developer activity data.
- **Flow-State Analysis:** Identifies uninterrupted development sessions using configurable activity and interruption thresholds.
- **Context-Switching Analytics:** Analyses application transitions, notification frequency, and estimated interruption-related overhead.
- **Custom Analytics Dashboard:** Uses React and Tremor.js to visualise developer activity patterns and team-level insights.
- **REST API Integration:** Uses FastAPI to securely expose aggregated analytical metrics to the frontend.

## Technology Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Workflow Orchestration | Apache Airflow |
| Analytical Database | ClickHouse |
| Data Processing | Polars, Pandas |
| Backend | FastAPI |
| Frontend | React.js |
| Visualization | Tremor.js |
| Data Sources | GitHub API, Jira API, Slack API, ActivityWatch |
| Database Querying | SQL |

## System Architecture

The platform follows an end-to-end data engineering and analytics architecture:

1. **Data Ingestion:** Extracts timestamped developer activity events from integrated platforms.
2. **Orchestration:** Apache Airflow manages scheduled extraction workflows and pipeline dependencies.
3. **Data Processing:** Python and Polars clean, normalise, and consolidate heterogeneous event data.
4. **Data Storage:** Processed events are loaded into ClickHouse for analytical querying.
5. **Analytics:** SQL and Python-based logic calculate focus-session durations, interruption frequency, and context-switching indicators.
6. **API Layer:** FastAPI exposes aggregated metrics through REST endpoints.
7. **Visualization:** React and Tremor.js present interactive analytics dashboards.

## Key Analytical Metrics

| Metric | Description |
|---|---|
| Focus Duration | Duration of qualifying uninterrupted development sessions |
| Flow Blocks | Number of continuous sessions meeting the configured focus threshold |
| Context Switch Count | Number of detected transitions between activities |
| Interruption Frequency | Frequency of interruption events over a defined period |
| Estimated Recovery Time | Estimated time associated with resuming work after interruptions |
| Context-Switching Tax | Estimated proportion of available focus time associated with interruption-related overhead |
| Notification Impact | Relationship between notification events and subsequent developer activity |

## Project Objectives

- Develop an automated data ingestion and orchestration pipeline.
- Integrate heterogeneous developer activity data into a unified analytical schema.
- Perform high-performance transformations on timestamped event data.
- Identify interruption patterns and quantify observable workflow friction.
- Build an interactive analytics platform for engineering workflow analysis.
- Support data-driven improvements in developer experience and notification management.

## Development Roadmap

| Week | Development Focus |
|---|---|
| Week 1 | API ingestion, mock event generation, Airflow setup, and React initialization |
| Week 2 | ClickHouse deployment, Polars transformations, and initial dashboard metrics |
| Week 3 | Flow-session detection, context-switching analysis, and advanced visualizations |
| Week 4 | FastAPI integration, frontend-backend connectivity, and dashboard optimization |

## Expected Outcome

CogniStream aims to provide an integrated developer workflow analytics platform that moves beyond conventional output-based productivity measurements.

By analysing activity patterns and interruption events, it helps engineering teams understand where development workflows experience friction and identify opportunities to improve uninterrupted working time.

**The central objective is to measure the quality of the development process, not simply the quantity of its output.**

---

*Note: This repository describes the intended project architecture and development roadmap. Actual integrations, analytical capabilities, and performance results will be documented as implementation progresses.*# -AtmoSync-Micro-Climate-Arbitrage-Analytics
