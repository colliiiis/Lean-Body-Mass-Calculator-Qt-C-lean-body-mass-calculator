# Lean Body Mass Calculator (Qt / C++)

A small desktop application that estimates lean body mass from a person's weight and height. It shows results for three published formulas (Boer, James, Hume) for men and women, plus the average of the three for each group.

> Disclaimer: educational project. Results are estimates and are not medical advice.

## Features
- Input of weight (kg) and height (cm)
- Calculation with three formulas, separately for men and women
- Average value for each group
- Input validation (empty values are rejected with a message)

## Tech stack
- C++17, Qt Widgets, QMake
- UI designed in Qt Designer (the interface language is Russian)

## Build and run
Requires Qt (Widgets) and QMake.

    cd Project
    qmake k1.pro
    make

## Project structure
    Project/
      k1.pro          QMake project file
      main.cpp        application entry point
      mainwindow.h    main window class
      mainwindow.cpp  validation and calculations
      mainwindow.ui   window layout

## Known limitations / ideas
- Add references for each formula and verify coefficients
- Add sex selection and realistic input ranges
- Move formulas into separate functions and add unit tests
- Add result history and export
