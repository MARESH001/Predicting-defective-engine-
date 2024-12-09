###Predictive Maintenance 

The dataset consists of 10,000 data points stored as rows with 14 features in columns.

## Features:
1. **UID**: Unique identifier ranging from 1 to 10,000.
2. **ProductID**: Identifier for the product quality variant:
   - **L**: Low quality (50% of all products).
   - **M**: Medium quality (30%).
   - **H**: High quality (20%).
   Each variant has a specific serial number.
3. **Air Temperature [K]**: Generated using a random walk process and normalized to a standard deviation of 2 K around 300 K.
4. **Process Temperature [K]**: Generated using a random walk process, normalized to a standard deviation of 1 K, added to the air temperature plus 10 K.
5. **Rotational Speed [rpm]**: Calculated from a power output of 2860 W, overlaid with normally distributed noise.
6. **Torque [Nm]**: Normally distributed around 40 Nm with a standard deviation (Ïƒ) of 10 Nm, ensuring no negative values.
7. **Tool Wear [min]**: Quality variants impact tool wear as follows:
   - **H**: Adds 5 minutes.
   - **M**: Adds 3 minutes.
   - **L**: Adds 2 minutes.
8. **Machine Failure**: Indicates whether the machine failed for any of the following failure modes:

## Target:
- **Failure or Not**: Binary target indicating machine failure status.

## Failure Types:
- Type of failure modes recorded in the dataset:
  - Tool wear failure.
  - Heat dissipation failure.
  - Power failure.
  - Overstrain failure.
  - Random failures
