# Data Visualisation App – Extension Ideas

This document lists possible features to extend the provided Data Visualisation App template using **only p5.js** and while maintaining the original project structure.

Each feature category respects the assignment requirements:

- No external libraries
- No replacing/restructuring the template
- No cloud-hosted dependencies
- All extensions must be integrated into existing files

---

## ✅ Global Application-Level Feature Ideas

### 1. Interactive Control Panel

- Use p5 DOM (sliders, buttons, checkboxes)
- Toggle elements (labels, grid, legends, smoothing)
- Example options:
  - Show/Hide labels
  - Enable/Disable data smoothing
  - Sort data by different attributes

### 2. Keyboard Shortcuts

- Change visualisations using number keys
- Toggle advanced options (`H` for help menu)
- Pause animations
- Reset visual state

### 3. Reusable Components

Suggested files:

- `helper-functions.js`
- `pie-chart.js`

Possible components:

- `Legend()`
- `Tooltip()`
- `Axis()`
- `Button()`

### 4. Export Visual as Image

- Use `saveCanvas()` to export PNG snapshots

---

## 📊 Extensions per Visualisation

---

## 1. Tech Diversity: Gender (Stacked Bar Chart)

### Possible Features

- Sorting based on:
  - Female proportion
  - Male proportion
  - Alphabetical company names
- Percentage labels on bars
- Hover tooltip display
- Highlighting currently hovered bar
- Industry average reference line
- Vertical scaling for smaller/larger datasets
- Colour themes toggle (e.g., high contrast mode)

### Coding Techniques

- Arrays of objects
- Sorting with `.sort()`
- Rectangle hit detection
- Mapping values to screen positions

---

## 2. Tech Diversity: Race (Pie Chart)

### Possible Features

- Dropdown to select a company
- Animated pie transitions
- Slice “explode” effect on hover
- Toggle between:
  - Pie representation
  - Stacked bar representation
- Dynamic legend displayed on canvas

### Coding Techniques

- Using `createSelect()`
- Arc math via `cos()/sin()`
- Handling slice angles cumulatively
- Object-based colour assignment

---

## 3. Pay Gap 1997–2017 (Line Graph)

### Possible Features

- Highlight selected year on mouse hover
- Dynamic range filtering (sliders to limit year range)
- Shade positive vs negative pay gap area
- Trend line (Moving average)
- Annotation for max/min gaps

### Coding Techniques

- Sequential plotting with `line()`
- Array model transformation from raw table rows
- Helper mapping functions
- Statistical calculation (mean, max, min)

---

## 4. Pay Gap by Job 2017 (Scatter Plot)

### Possible Features

- Represent magnitude of gap using point size
- Colour dots based on gap direction (male-favouring vs female-favouring)
- Click-to-pin tooltip labels
- Background quadrant shading
- Legend showing colour ranges

### Coding Techniques

- Mapping two variables to X/Y axes
- Colour scaling
- Object arrays storing job-level data
- Mouse interaction detection

---

## 5. Climate Change Visualisation (Temperature Line + Gradient)

### Possible Features

- Gradient background per year based on temperature
- Highlight years with highest anomalies
- Draw second comparison line (e.g. rolling average)
- Timeline scrubber for progressive reveal
- Legend showing colour-coded temperature scale

### Coding Techniques

- Gradients using `rect(...) + fill(...)`
- Mapping temperature values to colours
- Overlaying line data after background draw

---

## 🧠 Suggested Advanced Features for High Marks

These show strong programming skills:

### ✔ Reusable Class-Based System

Example file structure:
