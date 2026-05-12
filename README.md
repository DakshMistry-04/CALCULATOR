# Calculator

## 1. Table of Contents
* [About the Project](#2-about-the-project)
* [How It Works (Logic Flowchart)](#3-how-it-works-logic-flowchart)
* [Result and Analysis](#4-result-and-analysis)
* [Technology Used](#5-technology-used)

---

## 2. About the Project
The **Calculator** is a lightweight, client-side web application designed to perform basic arithmetic operations directly within a modern web browser. It features a responsive grid interface, structured CSS for visual clarity, and simple JavaScript for state management and mathematical evaluation. 

The goal of this project was to create a clean, functional UI mimicking a physical calculator, demonstrating efficient DOM manipulation and basic mathematical input handling without relying on complex backend infrastructure.

---

## 3. How It Works (Logic Flowchart)
The Calculator operates on a cyclical input-process-output model managed entirely by JavaScript. 

![Logic Flowchart](watermarked_img_10602067934641970635.png)

### Logic Breakdown:
* **User Input:** The cycle begins when the user interacts with the UI via `onclick` event listeners.
* **State Management:** The application maintains a single point of truth for the input using a `currentInput` string variable.
* **Process:** When the `=` button is pressed, the `calculate()` function triggers using the `eval()` method to process the string as JavaScript math.
* **DOM Manipulation:** The `updateDisplay()` function locates the screen element and updates its `innerText` to match the new state.

---

## 4. Result and Analysis

### Phase 1: Initial State
The code initializes with the display set to '0'. The CSS defines a dark theme with vibrant orange operators and a blue equals key.

![Initial State]<img width="225" height="332" alt="initial png" src="https://github.com/user-attachments/assets/67bc3d73-0d60-42b6-b294-ae58b7247006" />

### Phase 2: Successful Calculation
In this phase, mathematical strings (e.g., "7*10+5") are evaluated correctly to produce results like "75".

![Successful Calculation]<img width="225" height="332" alt="error png" src="https://github.com/user-attachments/assets/d87aaae8-0b87-44a9-a203-b7e4f4319362" />

### Phase 3: Error Handling
The application includes a `try...catch` block. If an invalid mathematical string is entered, the screen displays "Error" before resetting to "0" after 1.5 seconds via `setTimeout`.

![Error State]<img width="225" height="332" alt="success png" src="https://github.com/user-attachments/assets/4e220fe4-3e53-4615-9c27-8b0823349ca0" />

---

## 5. Technology Used

| Technology | Role |
| :--- | :--- |
| **HTML5** | Structure and Semantic Markup |
| **CSS3** | Responsive Grid Layout and Styling |
| **JavaScript (ES6)** | State Management and Evaluation Logic |
| **Gemma** | Efficiency logic consultation |
| **Gemini** | Layout analysis and CSS optimization |
| **Claude** | Error handling refinement |
| **Grok** | Implementation validation |
