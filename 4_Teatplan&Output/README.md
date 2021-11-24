# TEST PLAN

## Table no 1: High level test plan

| **Test ID** | **Description**                                              | **Exp I/P** | **Exp O/P** | **Actual Out** |**Type Of Test**  |    
|-------------|--------------------------------------------------------------|------------|-------------|----------------|------------------|
|  H_01       |Calculate the total parallel resistance when all the 3 resistor values are given as input| 68000,4700,560000|Total Parallel Resistance=4361.906738 ohm|Total Parallel Resistance=4361.906738 ohm|Requirement based |
|  H_02       |Calculate the total series resistance when less than 3 resistor values are given as input |68000,0,4700|Total series resistance=72700.00 ohm|Total series resistance=72700.00 ohm|Scenario based    |
|  H_03       |Calculate Resistance based on color code|5,11,10,2,10|Invalid Input|Invalid Input|Boundary based    |

## Table no 2: Low level test plan

| **Test ID** | **Description**                                              | **Exp IN** | **Exp OUT** | **Actual Out** |**Type Of Test**  |    
|-------------|--------------------------------------------------------------|------------|-------------|----------------|------------------|
|  L_1       |Calculate the parameters when complete required values are given as input|  |||Requirement based |
|  L_1.1   |Calculate the total series resistance| 30,20,40|Total series resistance=90.000000 ohm |Total series resistance=90.000000 ohm|Requirement based |
|  L_1.2   |Calculate the total parallel resistance|  6,5,4.3 |Total Parallel Resistance=1.668823 ohm |Total Parallel Resistance=1.668823 ohm|Requirement based |
|  L_1.3  |Calculate Resistance based on voltage and current(Current!=0)|  12,2.4 |Resistance=5.000000 ohm |Resistance=5.000000 ohm |Requirement based |
|  L_1.4     |Calculate Resistance based on color code|  6,8,0,2,10 |Resistor value=68000 +/- 5 % ohm |Resistor value=68000 +/- 5 % ohm|Requirement based |
|  L_2       |Calculate the parameters when non existable/empty values are given as input| |||Scenario based    |
|  L_2.1   |Calculate the total series resistance| 4.5,0,5|Total series resistance=9.500000 ohms |Total series resistance=9.500000 ohms|Scenario based |
|  L_2.2 |Calculate Resistance based on voltage and current(Current=0)|  12,0 |Invalid input:ampere |Invalid input:ampere |Scenario based |
|  L_2.3   |Calculate Resistance based on color code|  10,8,0,2,0 |Invalid Input|Invalid Input|Scenario based |

