# CGPA Calculator

A modern, responsive CGPA (Cumulative Grade Point Average) Calculator built with React.js and TailwindCSS.

## Features

- ✅ Clean, user-friendly interface with dark mode support
- ✅ Add/Remove multiple courses dynamically
- ✅ Comprehensive input validation
- ✅ Real-time CGPA calculation
- ✅ Detailed results display with course breakdown
- ✅ Print functionality for results
- ✅ Grade points reference table
- ✅ Fully responsive design

## Grade Points Mapping

| Grade | Grade Point |
|-------|-------------|
| A+    | 4.0         |
| A     | 3.7         |
| B+    | 3.3         |
| B     | 3.0         |
| C+    | 2.7         |
| C     | 2.3         |
| D     | 2.0         |
| F     | 0.0         |

## Installation

1. Install dependencies:
```bash
npm install
```

## Running the Application

1. Start the development server:
```bash
npm run dev
```

2. Open your browser and navigate to the URL shown in the terminal (usually `http://localhost:5173`)

## Building for Production

```bash
npm run build
```

The built files will be in the `dist` directory.

## Usage

1. Enter course details:
   - Course Name
   - Credit Hours (must be a positive number)
   - Grade (select from dropdown: A+, A, B+, B, C+, C, D, F)

2. Add more courses by clicking the "Add Course" button

3. Remove courses by clicking the "Remove" button (at least one course must remain)

4. Click "Calculate CGPA" to see your results:
   - Total Credit Hours
   - Total Grade Points
   - Final CGPA (rounded to 2 decimal places)
   - Course-by-course breakdown

5. Use "Reset" to clear all entries

6. Toggle dark mode using the theme button in the header

7. Print results using the "Print Results" button

## Technologies Used

- React.js 18.2.0
- TailwindCSS 3.3.6
- Vite 5.0.8

## Input Validation

The application validates:
- Course names are not empty
- Credit hours are positive numbers
- Grades are from the valid list (A+, A, B+, B, C+, C, D, F)
- All fields must be filled before calculation

## CGPA Calculation Formula

CGPA = Total Grade Points / Total Credit Hours

Where:
- Total Grade Points = Σ (Credit Hours × Grade Points for each course)
- Total Credit Hours = Sum of all credit hours

