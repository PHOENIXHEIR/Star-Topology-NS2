### NS-2 Wireless Network Simulation

This repository contains a TCL script for simulating a wireless network scenario using NS-2 (Network Simulator version 2). The script sets up a network topology with mobile nodes, defines node movements, establishes TCP connections, and generates traffic between nodes using FTP applications.

### Overview

The simulation script (`simulation_script.tcl`) creates a network scenario with the following characteristics:

- **Topology**: Flat grid topology with dimensions 500x500.
- **Nodes**: 8 mobile nodes (`$val(nn)`), each configured with specific properties such as routing protocol (DSDV), link layer (LL), MAC type (802.11), etc.
- **Node Movements**: Nodes are configured to move over time according to predefined trajectories using the `setdest` command.

### Simulation Details

- **Traffic Generation**:
  - TCP traffic is simulated using FTP applications.
  - FTP agents are attached to TCP agents on specific node pairs to generate traffic.

- **Simulation Execution**:
  - The simulation script can be executed using NS-2 to observe the behavior of the network over time.
  - Trace files (`simple.tr`) and Nam visualization files (`out.nam`) are generated during the simulation for analysis and visualization purposes.

### Prerequisites

Before running the simulation, ensure you have the following installed:

- **NS-2**: Install NS-2 on your system. Refer to the [NS-2 website](https://www.isi.edu/nsnam/ns/) for installation instructions.
- **TCL**: Ensure TCL (Tool Command Language) is available on your system.

### Usage

1. **Clone Repository**:
   ```bash
   git clone https://github.com/PHOENIXHEIR/ns2-wireless-network-simulation.git
   ```

2. **Navigate to Repository**:
   ```bash
   cd ns2-wireless-network-si.mulation
   ```

3. **Run Simulation**:
   - Modify the simulation parameters in `simulation_script.tcl` if necessary.
   - Execute the simulation script using NS-2:
     ```bash
     ns simulation_script.tcl
     ```

4. **View Results**:
   - Analyze the simulation results using the generated trace (`simple.tr`) and Nam visualization (`out.nam`) files.

### Simulation Output

- **Trace File (`simple.tr`)**:
  - Contains event traces recorded during the simulation.
  - Can be analyzed using NS-2 tools or custom scripts for performance evaluation.

- **Nam Visualization (`out.nam`)**:
  - Provides a graphical representation of the network topology and node movements over time.
  - Use Nam (Network Animator) to visualize the simulation results:
    ```bash
    nam out.nam
    ```

### Contributing

Contributions to enhance or extend this simulation script are welcome. If you have suggestions or improvements, please feel free to submit a pull request.

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### Acknowledgments

This simulation script is based on a template provided by the [NS-2 Network Simulator](https://www.isi.edu/nsnam/ns/). Special thanks to the NS-2 community for their valuable contributions.

---


