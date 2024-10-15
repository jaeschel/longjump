# longjump

# Fatigue Calculator

The Fatigue Calculator is a Python program designed to estimate anticipated fatigue levels based on various factors from long jump training sessions, academic demands, sleep, and more. It enables users to track their fatigue levels over time, visualize trends, and make data-driven adjustments to their routines.

## Features

- **Flexible Input Parameters**: 
  - Number of jumps
  - Number of steps (indicates daily activity level)
  - Landed or No Land (indicates session intensity)
  - Academic/Outside Fatigue (rating scale of 1-5)
  - Sleep Hours

- **Data Storage and Persistence**:
  - Saves fatigue levels after each session to a JSON file for tracking over time.
  - Loads past data to continue tracking fatigue without losing progress.

- **Data Visualization**:
  - Generates a line plot of fatigue levels across sessions using `matplotlib`.

## Setup Instructions

### Prerequisites
- Python 3.x
- `matplotlib` library (for data visualization)

### Installation
1. **Clone the Repository**:
    ```bash
    git clone https://github.com/your-username/fatigue-calculator.git
    cd fatigue-calculator
    ```

2. **Install Required Libraries**:
    ```bash
    pip install matplotlib
    ```

3. **Run the Program**:
    ```bash
    python fatigue_calculator.py
    ```

## Usage

1. **Start the Program**:
   - You will be prompted to enter data about your training session, academic fatigue, and sleep.

2. **Follow the Prompts**:
   - Enter values as prompted. For example:
     - `Enter the number of jumps:`
     - `Enter the total number of steps:`
     - `Did you land during the session? (yes/no):`
     - `Enter your academic/outside fatigue level (1-5):`
     - `Enter the number of hours you slept:`

3. **View Fatigue Level**:
   - The program calculates and displays your fatigue level for the session.

4. **Save and Visualize Data**:
   - The program saves your fatigue data to a JSON file and generates a plot to help visualize trends over time.

## Customization

- You can adjust the weight values for each factor within the `calculate_fatigue` method of the `FatigueCalculator` class to better match your specific experience and impact of each factor on your fatigue.

## Example

After entering your data:
```plaintext
Enter the number of jumps: 20
Enter the total number of steps: 15000
Did you land during the session? (yes/no): yes
Enter your academic/outside fatigue level (1-5): 3
Enter the number of hours you slept: 6
