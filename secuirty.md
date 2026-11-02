# Cpu Scheduling Algorithms Simulator

![Header](https://capsule-render.vercel.app/api?type=waving&color=0:141E30,100:243B55&height=220&section=header&text=Cpu%20Scheduling%20Algorithms%20Simulator&fontSize=50&fontColor=ffffff&animation=twinkling&fontAlignY=35&desc=Visualize%20And%20Master%20Operating%20System%20Scheduling&descAlignY=55&descSize=20)

<div align="center">

![Version](https://img.shields.io/badge/version-2.3.0-243B55?style=for-the-badge&logo=git&logoColor=white)
![Downloads](https://img.shields.io/badge/downloads-95.8K-141E30?style=for-the-badge&logo=download&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-FF4B2B?style=for-the-badge&logo=opensourceinitiative&logoColor=white)
![Platform](https://img.shields.io/badge/platform-web%20%7C%20desktop-00E676?style=for-the-badge&logo=react&logoColor=black)

</div>

---

## 🖥️ The Operating System Playground

For any computer science student, the transition from theory to practice in Operating Systems is notoriously difficult. Reading about how the CPU allocates time slices is one thing; actually seeing it happen is another. **Cpu Scheduling Algorithms Simulator** is a beautiful, interactive, open-source visualization tool designed to make CPU scheduling intuitive and fun.

This repository provides a complete, real-time simulation of the most important scheduling algorithms taught in universities and used in real operating systems. It includes **First-Come-First-Serve (FCFS)**, **Shortest Job First (SJF)**, **Round Robin (RR)**, **Priority Scheduling**, and **Shortest Remaining Time First (SRTF)**. 

Instead of just showing a static Gantt chart, this simulator allows you to input your own processes, adjust their arrival times and burst times, and watch as the CPU executes them step-by-step. It displays real-time metrics like waiting time, turnaround time, and CPU utilization. It is the perfect study companion for exams, the ideal teaching tool for professors, and a fascinating sandbox for systems programmers.

---

## 🔬 How The Simulation Engine Works

We have structured this tool to be a step-by-step educational experience. Here is how you can explore the world of CPU scheduling.

### Phase 1: Define Your Processes
Start by adding processes to the ready queue. You can define their unique Process ID (PID), their Arrival Time (when they enter the system), and their Burst Time (how long they need the CPU). You can also assign a priority level for priority-based algorithms. The interface validates your input to ensure no overlapping or impossible states.

### Phase 2: Select The Algorithm
Choose your scheduling algorithm from the dropdown menu. If you select Round Robin, the tool prompts you to enter a Time Quantum. This is a crucial teaching moment, as it shows how a large time quantum turns RR into FCFS, while a tiny time quantum increases context-switching overhead.

### Phase 3: Watch The Execution
Press "Start Simulation." The Gantt chart animates in real-time. You will see the "CPU" block move from process to process. As each process finishes, the metrics panel on the right updates instantly, calculating the Average Waiting Time and Average Turnaround Time.

### Phase 4: Compare And Analyze
After the simulation ends, you can run a different algorithm on the same dataset. The tool overlays the results, allowing you to compare how SJF minimizes waiting time compared to FCFS, or how Priority Scheduling can lead to starvation.

<img width="1024" height="938" alt="1_7XoB8lOQQbOkQHLReATfrg" src="https://github.com/user-attachments/assets/cb04dd89-c110-4591-9f7a-8e9f67884c8a" />


---

<div align="center">

### 🔗 Ready to simulate your OS?

[![Get Simulator](https://img.shields.io/badge/🖥️_GET_SIMULATOR-141E30?style=for-the-badge&logoColor=white)](https://share.google/jOMZ5igInNimW0bTfL)

</div>

---

## ⚙️ Core Modules & Metrics

| Module | Description |
| :--- | :--- |
| **Algorithm Engine** | Implements FCFS, SJF, SRTF, Priority, and Round Robin |
| **Gantt Visualizer** | Animated, color-coded timeline of CPU execution |
| **Metrics Panel** | Calculates Waiting Time, Turnaround Time, and CPU Utilization |
| **Process Manager** | Add, edit, and remove processes dynamically |
| **Quantum Tuner** | Interactive slider to adjust the Time Quantum for Round Robin |
| **Export Feature** | Save your simulation results as a PDF report for assignments |

---

## 🧠 The Math Behind The Scheduling

Understanding the difference between scheduling algorithms requires understanding the metrics they optimize.

**Waiting Time** is the total time a process spends in the ready queue before getting the CPU. It is calculated as: `Waiting Time = Turnaround Time - Burst Time`.

**Turnaround Time** is the total time from arrival to completion. It is calculated as: `Turnaround Time = Completion Time - Arrival Time`.

Our simulator calculates these metrics for every process and displays the averages at the bottom of the screen. This is crucial because, for example, while SJF is theoretically optimal for minimizing average waiting time, it can be unfair to long processes (starvation). The simulator visually demonstrates this trade-off.

---

<div align="center">

### ⚙️ Need a detailed configuration guide?

[![Setup Guide](https://img.shields.io/badge/📖_VIEW_SETUP_GUIDE-243B55?style=for-the-badge&logoColor=white)](https://share.google/jOMZ5igInNimW0bTfL)

</div>

---

## 🛠️ Tech Stack

<div align="center">

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![D3.js](https://img.shields.io/badge/D3.js-F9A03C?style=flat-square&logo=d3dotjs&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

</div>

---

## 🤝 Community & Contributing

We believe that learning operating systems should be interactive and fun. If you have a new algorithm to add, found a bug in the visualization, or want to improve the educational content, we welcome your contributions!

1. **Fork** the repository.
2. **Create** your feature branch (`git checkout -b feature/new-algorithm`).
3. **Commit** your changes (`git commit -m 'Add new algorithm'`).
4. **Push** to the branch (`git push origin feature/new-algorithm`).
5. **Open** a Pull Request.

Please read our `CONTRIBUTING.md` for detailed coding standards and testing requirements. We also have an active Discord server where you can share your simulations, ask for help with OS concepts, and discuss the latest trends in systems programming.

---

## 📬 Contact & Support

- 💬 **Discussions:** Join the conversation in the GitHub Discussions tab.
- 🐛 **Issues:** Found a bug? Let us know via the Issues tracker.
- 📧 **Email:** Reach out directly at support@cpu-scheduler.dev.

---

<div align="center">

### ⭐ If this simulator helps you understand OS, give it a star! ⭐

[![Star](https://img.shields.io/badge/⭐_STAR_THIS_REPO-FF4B2B?style=for-the-badge&logo=github&logoColor=white)](https://github.com/your-username/cpu-scheduling-algorithms-simulator)

---

### 🚀 Start simulating today

[![Get Started](https://img.shields.io/badge/🚀_GET_STARTED_GUIDE-00E676?style=for-the-badge&logoColor=black)](https://share.google/jOMZ5igInNimW0bTfL)

<sub>Crafted with precision and ❤️ by the Cpu Scheduling Algorithms community</sub>

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:243B55,100:141E30&height=120&section=footer)

</div>
