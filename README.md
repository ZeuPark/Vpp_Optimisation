# VPP Optimization

**Objective**  
Optimize Virtual Power Plant scheduling to minimize energy cost or maximize profit using LP with realistic tariff structures.

## Dataset
- **Inputs**: Load forecast, PV generation forecast, battery specs, tariff data
- **Horizon**: 24 hours
- **Resolution**: 1 hour

## Methodology
1. Decision Variables: Battery charging/discharging, grid import/export, PV utilization
2. Constraints: Energy balance, capacity, efficiency, SoC bounds
3. Objective: Cost minimization
4. Solver: PuLP / OR-Tools

## Results
| Scenario         | Total Cost ($) | Cost Reduction |
|------------------|----------------|----------------|
| Baseline         | X,XXX          | -              |
| Optimized        | X,XXX          | YY%            |

**Sample Schedule Plot**  
![schedule](results/sample_schedule.png)

## How to Run
```bash
python src/lp_model.py --config configs/tariff.yaml
