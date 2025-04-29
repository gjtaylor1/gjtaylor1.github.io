'''mermaid
    flowchart TD
        A[Computer Fan Control Program] --> |Wait 30 s| B{CPU temp > 80°C}

        B -->|No| C[Decrease fan speed by 10%] --> E{Fan speed < 40%?}
        B -->|Yes| D[Increase fan speed to 100%] --> A

        E --> |No| A
        E --> |Yes| F[Set fan speed to  40%] --> A
'''