# OS_LAB_PROJECT


# Process Scheduling Simulator

## Overview
The Process Scheduling Simulator is a Windows-based graphical application that simulates various process scheduling algorithms. Users can input process details, select a scheduling algorithm, and view the simulation results, including Gantt charts, average waiting times, and turnaround times.

## Features
- **Add Processes:** Input arrival time, burst time, and priority.
- **Set Time Quantum:** Specify the time quantum for the Round Robin scheduling algorithm.
- **Simulate Scheduling Algorithms:** 
  - First-Come, First-Served (FCFS)
  - Round Robin (RR)
  - Shortest Job Next (SJN)
  - Shortest Remaining Job First (SRJF)
  - Priority Scheduling
- **Visualize Gantt Charts:** Display the scheduling process using Gantt charts.
- **View Statistics:** Show average waiting time and turnaround time for the processes.

## Getting Started

### Prerequisites
- **Windows Operating System:** The application is developed for Windows and requires a Windows environment to run.
- **C++ Compiler:** A C++ compiler with support for the Win32 API (e.g., MinGW, MSVC,GNU Compiler).

### Building the Project
1. **Clone the Repository:**
    ```sh
    git clone https://github.com/yourusername/process-scheduling-simulator.git
    ```
2. **Navigate to the Project Directory:**
    ```sh
    cd process-scheduling-simulator
    ```
3. **Compile the Code:**
    ```sh
    g++ -o ProcessScheduler main.cpp -mwindows
    ```
    - Replace `g++` with your compiler if different.
4. **Run the Executable:**
    ```sh
    ProcessScheduler.exe
    ```

### Using the Application
1. **Launch the Application:**
   - Double-click `ProcessScheduler.exe` or run it from the command line.
2. **Add Processes:**
   - Enter the arrival time, burst time, and priority in the respective fields.
   - Click the "Add Process" button to add the process to the scheduler.
3. **Set Time Quantum (for Round Robin):**
   - Enter the time quantum in the designated field.
   - Click the "Set Time Quantum" button.
4. **Simulate a Scheduling Algorithm:**
   - Click the button for the desired scheduling algorithm (e.g., "FCFS", "Round Robin").
   - View the results, including Gantt charts and statistics, in the message boxes.

### Input Validation
- Ensure all input fields contain valid positive integers.
- Check that at least one process is added before starting the simulation.

## Code Structure
- **main.cpp:** Contains the entire application code, including the WinMain function, WndProc function, Process structure, and Scheduler class with various scheduling algorithms.

## Future Improvements
- Enhanced input validation and error handling.
- Improved visual presentation of Gantt charts.
- Separation of GUI code and scheduling logic for better maintainability.
- Additional scheduling algorithms as needed.

## Contributing
1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements
- Inspiration and guidance from various online resources on process scheduling algorithms and Win32 API programming.
