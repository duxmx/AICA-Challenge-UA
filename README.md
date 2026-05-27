# AICA Challenge 2026 — Team UA



Our team's implementation for the \[IEEE SMC 2026 AI-Powered Collaborative Autonomy Challenge](https://utadnclab.github.io/AICA-Competition-Documentation-2026/).



## Overview



We control a QCar2 (ground vehicle) and a QDrone2 (aerial drone) in a simulated city to deliver 5 packages from a central pickup location to apartment buildings. The competition rewards efficient delivery time and bonus points for window deliveries to higher floors.



## Setup



### Prerequisites



- Windows 10/11

- Python 3.12

- Quanser QLabs + QUARC

- Quanser SDK Python packages

- AICA Challenge content subscription



See \[`docs/SETUP.md`](docs/SETUP.md) for detailed install instructions, gotchas, and troubleshooting.



### Quick start



1. Clone this repo:

```bash

&#x20;  git clone git@github.com:duxmx/aica-challenge-2026.git

&#x20;  cd aica-challenge-2026

```

2. Follow `docs/SETUP.md` to install Quanser tools and configure environment variables.

3. Open QLabs from the Start menu and wait for it to fully load.

4. Run the simulation:

```powershell

&#x20;  .\\run\_all.bat

```



## Project Structure



```

.

├── QCar2\_Navigator.py        # Car control and navigation

├── QDrone2\_Navigator.py      # Drone control and navigation

├── setup\_env.py              # QLabs environment setup (provided by Quanser, do not edit)

├── game.py                   # Simulation orchestrator (provided by Quanser, do not edit)

├── run\_all.bat               # Launches all components in order

├── spawn\_locations.txt       # Initial positions for vehicles

├── tools/

│   ├── QCar2\_PathPlanning/   # Pre-computed car paths

│   └── QDrone2\_PathPlanning/ # Pre-computed drone trajectories

├── virtual\_DriveStack.rt-win64    # Car real-time model

├── virtual\_FlightStack.rt-win64   # Drone real-time model

└── docs/                     # Team documentation

```



## Development



See \[`CONTRIBUTING.md`](CONTRIBUTING.md) for branch naming, commit conventions, and PR process.



## Team



- Maddux Taukave-Castro — \[Team Member]

- Esther Desroche — \[Team Member]

- Samin Yasar — \[Graduate Mentor, Team Membor]

- PI: Dr. Mahmoud Mahmoud, University of Alabama



## Acknowledgments



Starter code provided by Quanser and the AICA Challenge organizers.

