🚦 Traffic Controller using Semaphores in C
This project is a simulation of a traffic controller system at a two-way intersection using POSIX semaphores and pthreads in C. The idea is to simulate how traffic from two or more directions can be managed efficiently without collisions using synchronization primitives (like semaphores).

This is useful for:
🚦 Traffic Controller using Semaphores in C
This project is a simulation of a traffic controller system at a two-way (or multi-way) intersection using POSIX semaphores and pthreads in C. It demonstrates how traffic from different directions can be managed efficiently without collisions by using synchronization primitives like semaphores.

This project is ideal for:

🎓 Demonstrating Operating Systems and Concurrency concepts

🛠️ Simulating Embedded Systems behavior

🧵 Learning and practicing thread synchronization with semaphores

🧠 Concepts Covered

Concept	Description
Threads	Simulate traffic from different directions using pthread. Each light or direction can be a separate thread.
Semaphores	Used to control access to the shared resource (the intersection) ensuring orderly flow.
Mutual Exclusion	Ensures only one thread (direction) can access the intersection at a time to prevent collisions.
Concurrency Control	Manages predictable traffic behavior even with multiple threads running simultaneously.
🔧 Technologies Used
C Programming Language

POSIX Threads (pthread)

POSIX Semaphores (semaphore.h)

Linux Environment for compilation and execution

🚀 How it Works
Traffic lights are simulated as threads.

Each light follows a timed cycle: RED → GREEN → YELLOW → RED.

Semaphores synchronize these threads to ensure only one light is GREEN at a time, simulating a safe traffic flow.

The system runs in an infinite loop mimicking a real-world traffic signal pattern.

📦 To Compile & Run
bash
Copy
Edit
gcc -pthread -o traffic_sim traffic_sim.c
./traffic_sim
Let me know if you'd like to include a sample output screenshot or animation in the README too — I can help you format that!
Operating Systems and Concurrency concept demonstrations
Embedded Systems simulations
Learning thread synchronization with semaphores
🧠 Concepts Covered
Concept	Description
Threads	Simulate vehicles arriving from different directions using pthread.
Semaphores	Used to control access to the critical section where only one direction of traffic can move at a time.
Mutual Exclusion	Only one thread (direction) can access the intersection at any given moment.
Concurrency Control	Ensures traffic simulation behaves predictably under concurrent execution.
