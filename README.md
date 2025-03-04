# Particle Collision Simulation

This project implements a high-performance particle collision simulation that leverages grid-based spatial partitioning for efficient broad-phase collision detection and elastic collision resolution. It is designed to handle 10⁵ particles at a density of 0.9 over 1000 time steps, and it utilizes OpenMP for parallel computing, boosting performance on multi-core systems by up to 10×.

## How to Run

### Compile the Simulation
Run the following command in the project `simulation` directory to compile the simulation:
```
make
```

### Run the Simulation Manually
After compiling, run the simulation with:
```
./sim <test> <number_of_threads>
```
- `<test>`: Specify the test input file (e.g., `tests/standard/10k_density_0.7.in`).
- `<number_of_threads>`: Specify the number of threads to use.

### Running with SLURM
For batch execution using SLURM, navigate to the `slurm` folder and run the provided batch script:
```
cd slurmjob
./slurm_job.sh
```
For more details about the project and its performance evaluation, see **report.pdf**.

For more details, visit the [GitHub Repository](https://github.com/ChauuuLe/Particle-collision-simulation).