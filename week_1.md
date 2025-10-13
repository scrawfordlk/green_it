# Week 1
## Prelude
China is a problem in terms of sustainability.
Irreversible changes in the environment.

## Electric Load Disaggregation as a Means for increasing Energy Awareness and Reducing Energy Consumption.
Most computers are embedded. (By CPU count)
Using non-reneweable energy is a big issue for sustainability. How can we improve this (without simply turning off devives)
### Smart Meter Rollout
  - Goal was to have 80% of electricity consumers have this system.
### Problem with the current billing of energy consumption:
  - Much later after the consumption happened
  - No details on how the energy was used
  - In AT: An estimated bill is paid which is corrected afterwards

### Strategies for domestic energy consumption
  - audits (analysis)
  - smart metering (more frequent readings)
    + privacy concern: daily schedule, used devices can be inferred
      - fridges have short usage spikes
      - dish washer is a long term usage (heating time)
      - washing mashine uses more energy, but takes less time than dish washer
  - prepaid billing
  - adaptive tariff plans (incentives users to operate in off-peak periods)
  - Persuasive interfaces: Help users understand energy usage

### Non-intrusive Load Monitoring
  - monitor devices with central meter
    + modeled as knapsack problem: From set of devices find subset that machtes consumption as close as possible
    + => large search space, results change much even if power consumption change is marginal
    + works only for small sets of devices
  - split consumption into different devices: Particle Filter Based Load Disaggregation (PADLI)
    + appliance modeled as set of FSMs. USing the markov-model (household filter), the aggregated power load can be inferred.
  - Deep Learning Approach
    + model problems as classification problems
    + previosly measured power is input
    + train classifier with machine learning
    + needs large dataset
    + needs large dataset
    + disadvantage: black box model

### Dee NILMTKK Pipeline
  - source: IEEE Transactions on Industrial Informatics, pages 1-9, 9 2022

###  Automatic Labeling of Appliances's Events
  - Simulation of appliances
  - Some application's on/off events are easier to detect than others
  - routine of resident may be revealed (privacy concern)

### Private smart metering
  - measure energy consumption for own appliances
    + => identify energy hungry devices to optimise
  - open hardware design

### YoMo and YoMoPie Smart Meters
  - open source/hardware
  - low hardware costs, no licenses
  - household internal solution (=> private)
  - YoMo: arduino shield to create new energy system applications
    + measure voltage of appliance
    + communicate power data to raspberry pie webserver
    + visualise data
  - YoMoPie: YoMo for raspberry pie

### Training and Evaluation
  - Datasets required
    + common geographic region (different appliances,..)
    + common measurement frequency (also over long period, e.g. over all 4 seasons)
