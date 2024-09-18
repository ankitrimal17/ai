Fuzzy Logic Assignment
Table of Contents

    Introduction
    Features
    Installation
    Algorithm Details
        Input and Output Variables
        Membership Functions
        Fuzzy Rules
        Control System
        Input Values
    Results

Introduction

This project implements a fuzzy logic system to evaluate the overall performance of students based on three key parameters: attendance, internal marks, and external marks. It uses a fuzzy inference system to generate a performance score based on fuzzy logic rules and membership functions.
Features

    Evaluates performance based on multiple parameters (attendance, internal marks, and external marks)
    Uses fuzzy logic for decision-making with trapezoidal membership functions
    Implements a set of fuzzy rules for generating performance outcomes
    Provides customizable input values for analysis

Installation

To run this project, ensure you have Python and the required libraries installed. Follow these steps to set up the environment:

    Clone the repository.
    Install the required Python libraries using pip:

    bash

    pip install numpy scikit-fuzzy

    Run the Python script in your preferred IDE or environment.

Algorithm Details
Input and Output Variables

The fuzzy logic system evaluates three input variables:

    Attendance (0-100)
    Internal Marks (0-100)
    External Marks (0-100)

The output variable is:

    Performance (0-100)

Membership Functions

Each variable is assigned membership functions based on ranges of values. The membership functions are categorized into:

    Poor
    Average
    Good
    Very Good
    Excellent

Fuzzy Rules

The fuzzy inference system follows 43 rules to determine the performance based on different combinations of attendance, internal marks, and external marks. Examples include:

    If attendance is poor, external marks are poor, and internal marks are poor, then performance is poor.
    If attendance is excellent, external marks are excellent, and internal marks are excellent, then performance is excellent.

Control System

A control system is implemented using the scikit-fuzzy library to simulate the fuzzy rules and membership functions. The ControlSystemSimulation class is used to compute the final performance score based on the input values.
Input Values

You can customize the input values for attendance, internal marks, and external marks to get a performance score:

    Example 1: compute_fuzzy(70, 20, 50)
    Example 2: compute_fuzzy(90, 30, 60)
    Example 3: compute_fuzzy(95, 90, 80)

Results

The system generates a performance score based on the provided input values. You can view the performance analysis by running the examples provided in the script. For example:

    Input: Attendance = 70, Internal Marks = 20, External Marks = 50
    Output: Performance = [generated value]
