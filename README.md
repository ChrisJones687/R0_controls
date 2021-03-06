# Factors influencing R0 Simulation Experiment
The goal of this simulation study is to determine which factors have the greatest influence on epidemic outcomes. Here we are explicitly dividing the factors into two distinct categories: 1) disease ecology and 2) landscape structure.

## Glossary:
R0 = basic reproduction number\
P0 = initial population size\
B = Beta (simulation parameter for # spores dispersing per unit time under optimal conditions)\
LP = latent period\
IP = infectious period\
TA = treatment area (i.e. buffer around infected cell)\
TT = treatment timing\
HR = 
A1 = Alpha-1 or natural distance scale parameter\
PE = pesticide efficacy (pesticide is used to encompass (vaccinations, fungicides, pesticides, etc..)
PD = pesticide duration (how many time units does the pesticide provide resistance)
## Experimental Setup

Run all simulations on a 200 x 200 area. We are keeping total amount of host constant but varying spatial arrangement.

### Factorial of Lifecycle Factors (400 combinations)
5 B = (1.25, 2, 4, 8, 16)\
5 P0 = (1, 5, 10, 50, 100) % infection at the epidemic outbreak\
4 LP = (2, 4, 8, 16)\
4 IP = (0.5, 1, 1.5, 2 x LP)

### Add in Landscape complexity


### Add in treatment effects
#### Timing and size effects (16 combinations)
4 TT = (1.5, 2.0, 2.5, 3.0 x LP)\
4 TA = (1, 3, 5, 7 x cell size)

#### Vaccination/Pesticide/Fungicide effects 
4 PE = (0.95, 0.80, 0.65, 0.50)\
4 HR = (1.00, 0.75, 0.50, 0.25 in TA but always 1.00 in infected cell)
