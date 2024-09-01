# PF_lab_2
flowchart TD
    A[Start] --> B[Input hoursParked]
    B --> C{hoursParked > 1}
    C -- Yes --> D[Set totalFee to $5]
    D --> E[Calculate additionalHours as hoursParked - 1]
    E --> F[Set totalFee to totalFee + (additionalHours * $3)]
    F --> G[Output totalFee]
    C -- No --> H[Set totalFee to $5]
    H --> G
    G --> I[End]
