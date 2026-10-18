# Simulated Device Temperature Monitoring and Alert System

**Student Name:** Villanueva, Uan Timothy D.  
**Student Number:** 2500746  
**Section:** 1CPE-B  

---

## 1. Project Overview

The **Simulated Device Temperature Monitoring and Alert System** is a Python-based console application engineered to log, evaluate, and track simulated device thermal data. The application empowers users to display current temperature logs, register new validated entries, categorize readings into status thresholds, and compile automated statistical summaries. Additionally, it computes the system's global operational condition based on thermal distributions.

---

## 2. Core Objectives

1. Apply core programming paradigms in Python, including variables, control flow (loops & conditionals), dynamic lists, and modular functions.
2. Provide an interactive interface for retrieving and logging temperature entries.
3. Enforce strict input sanitization, accepting only integer values bounded between 0 °C and 100 °C.
4. Categorize recorded thermal metrics into discrete operational tiers: **NORMAL**, **WARNING**, and **CRITICAL**.
5. Compute key analytical metrics including summation, arithmetic mean, extremum bounds (min/max), category distributions, and global system status.
6. Practice industry-standard software practices including automated validation logic, systematic testing, error handling, and Git version control.

---

## 3. Key System Features

1. Pre-loads a baseline set of test readings: 28 °C, 31 °C, 35 °C, 37 °C, and 29 °C.
2. Facilitates real-time addition of new temperature data points.
3. Filters and rejects empty strings, non-numeric inputs, floating-point decimals, negative integers, and values exceeding 100.
4. Classifies temperatures strictly under 30 °C as **NORMAL**.
5. Classifies temperatures from 30 °C up to 35 °C (inclusive) as **WARNING**.
6. Classifies temperatures above 35 °C as **CRITICAL**.
7. Computes a detailed summary dashboard containing frequency distributions and percentage allocations.
8. Evaluates aggregate health metrics to assign an overall system status.
9. Runs an interactive menu loop until explicitly closed by selecting the Exit option.
10. Includes defensive programming mechanisms to gracefully handle invalid menu navigation without crashing.

---

## 4. Technical Requirements & Dependencies

- **Language:** Python 3.x
- **IDE/Editor:** Visual Studio Code (or preferred text editor)
- **Environment:** Command Line Interface (CLI) / Terminal
- **Version Control:** Git & GitHub

> **Note:** This project utilizes native Python libraries exclusively; no third-party package installations (`pip`) are required.

---

## 5. Execution Instructions

1. Save the main source code file as `device_monitor.py`.
2. Open the project root directory in your code editor or terminal.
3. Launch the application via Python 3:
   ```bash
   python device_monitor.py
