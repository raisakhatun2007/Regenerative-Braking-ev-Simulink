# Regenerative Braking System for Electric Vehicles
### MATLAB & Simulink-Based Modelling and Performance Analysis

## Project Overview

Developed a simulation-based model of an Electric Vehicle (EV) regenerative braking mechanism using MATLAB/Simulink. The project explores how the vehicle's kinetic energy can be converted into electrical energy during deceleration and stored in the battery for future use.

The simulation focuses on evaluating braking performance, regenerative torque contribution, friction braking requirements, and overall energy recovery.

## System Design

The proposed model is divided into five interconnected functional units:

| Component | Description |
|---|---|
| Brake Demand Generator | Produces braking input based on the driver's applied brake command. |
| Braking Control Unit | Determines the appropriate balance between regenerative and mechanical braking. |
| Electric Motor-Generator | Simulates motor operation in generator mode to recover energy. |
| Vehicle Motion Model | Calculates vehicle acceleration, deceleration, and speed variations. |
| Battery Energy Monitor | Estimates recovered electrical energy and tracks battery energy gain. |

## Regenerative Braking Strategy

A speed-dependent braking approach is implemented to determine when regenerative braking should operate.

| Vehicle Speed | Braking Response |
|---|---|
| Below 5 m/s | Conventional friction braking |
| 5–15 m/s | Combined regenerative and friction braking |
| Above 15 m/s | Regenerative braking prioritized, subject to torque limits |

The controller continuously evaluates vehicle speed and braking demand to distribute the required braking torque while respecting the regenerative braking capacity.

## Simulation Parameters

| Parameter | Configuration |
|---|---:|
| Vehicle Weight | 1200 kg |
| Starting Velocity | 20 m/s |
| Maximum Regenerative Torque | 80 Nm |
| Battery Charging Efficiency | 95% |
| Simulation Environment | MATLAB / Simulink |

## Simulation Outcomes

The model was evaluated under a deceleration scenario to observe the amount of energy recovered through the motor-generator system.

| Performance Indicator | Simulated Result |
|---|---:|
| Initial Vehicle Kinetic Energy | 240,000 J |
| Recovered Electrical Energy | Approximately 28,000 J |
| Recovered Energy in kWh | Approximately 0.0078 kWh |
| Overall Energy Recovery Ratio | Approximately 11.6% |

## Technical Analysis

- Regenerative braking is restricted at very low vehicle speeds, where energy recovery becomes less effective.
- The controller uses friction braking to compensate whenever the required braking torque exceeds the motor's regenerative capacity.
- Energy regeneration takes place during braking rather than during normal acceleration or constant-speed operation.
- The simulation demonstrates the potential to recover a portion of otherwise dissipated kinetic energy and improve EV energy utilization.

## Simulation Visualizations

The following plots are used to evaluate the system's performance:

1. Vehicle Velocity Profile – Shows the reduction in vehicle speed throughout the braking cycle.
2. Regenerative Power Characteristics – Illustrates electrical power generated during deceleration.
3. Braking Torque Comparison – Displays the contribution of regenerative and friction braking.

## Software and Technologies

- MATLAB
- Simulink
- Electric Vehicle Dynamics Modelling
- Regenerative Energy Analysis
- Control System Simulation

## Project Author

**Raisa Khatun**  
Electrical Engineering  
Ramkrishna Mahato Government Engineering College, Purulia