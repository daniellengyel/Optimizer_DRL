# Optimizer DRL

For the development and testing of Deep Reinforcement Learning (DRL) methods for HVAC control.

## Folder Structure

* DataManager
* Environments
  + Environment
    + Policy_Models
* Optimization_Results


#### Datamanager

Module to retrieve and cache data necessary for the training and execution of DRL methods.
The module uses the xbos-service-getter package to retrieve and process data.
Specialized for the development and testing of DRL methods.

#### Environments

Development of different *environments*.
An environment is defined by four components: 1) state space, 2) action space, 3) reward function and 4) transition function.
We can explore different HVAC control by changing one of the four components.
Different building may also necessitate the use of different environments.

We may develop various *policy models* for each environment.
Different architecture can be used as policy models which may improve the found policy.

#### Optimization

Stores the results of using a specific *optimization algorithm* to solve for the optimal policy given an *environment* and *policy model*.
