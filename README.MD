# ESEP Grade Calculator

## Overview

The ESEP Grade Calculator is a Go library designed to calculate
students' final course grades using weighted averages.

The calculator supports three categories:
- Assignments
- Exams
- Essays

Each category contributes a percentage toward the final grade.

## Requirements

- Go 1.24 or newer
- Git

## Installation

Clone the repository:

```bash
git clone https://github.com/giancarlov0729/esep-grade-calculator.git
```

Navigate to the Go module:

```bash
cd esep-grade-calculator/grade-calculator
```

Verify Go is installed:

```bash
go version
```

## Project Structure

- `README.md`: Project documentation and setup instructions.
- `go.mod`: Defines the Go module and required Go version.
- `grade_calculator.go`: Implements grade calculation functionality.
- `grade_calculator_test.go`: Contains unit tests for grade evaluation.

## Grade Calculation

The calculator determines a student's final numerical grade by
computing the average of each grade category and multiplying
those averages by their respective weights.

The weighted averages are added together to determine the
final numerical grade, which is converted into a letter grade.

The calculator also determines whether a student passes
or fails based on their final grade.

## Running Unit Tests

Navigate to the Go module directory:

```bash
cd grade-calculator
```

Run all tests:

```bash
go test ./...
```

For detailed test results:

```bash
go test -v ./...
```

## Measuring Code Coverage

Go includes built-in tools for measuring unit test coverage.

Generate a coverage report:

```bash
go test -coverprofile=coverage.out ./...
```

Display the total coverage percentage:

```bash
go tool cover -func=coverage.out
```

Generate an HTML coverage report:

```bash
go tool cover -html=coverage.out
```

## Development

The project includes automated unit tests that validate
the grade calculation functionality.

Developers should run the test suite after making changes
to ensure that existing functionality remains correct.

Note: The initial repository contains failing tests and
implementation issues that will be addressed in subsequent
development commits.