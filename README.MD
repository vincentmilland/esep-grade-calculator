# Grade Calculator

A GO library that is used for computing the final letter grade a student will receive from weighted exams, assignments, and essays.

# Runtime requirements:
Go 1.24.4+

# Package
esepunittests

# Run unit tests:
```
cd grade_calculator/
go test ./...
```

# Run unit tests with code coverage:
```
cd grade_calculator/
go test -coverprofile=coverage.txt ./...
```

# Usage
```go
gc := NewGradeCalculator()
gc.AddGrade("Homework 1", 90, Assignment)
gc.AddGrade("Midterm", 85, Exam)
gc.AddGrade("Essay 1", 92, Essay)
grade := gc.GetFinalGrade() // "A"
```
