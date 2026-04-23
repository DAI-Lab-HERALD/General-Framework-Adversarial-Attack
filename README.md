# Realistic Adversarial Attacks for Robustness Evaluation of Trajectory Prediction Models via Future State Perturbation
This is the used framework for generating the Adversarial attacks in the [paper](https://dl.acm.org/doi/abs/10.1145/3799894). 

This is a clone of [STEP](https://github.com/DAI-Lab-HERALD/General-Framework/tree/main), a general framework for evaluating prediction models (including on perturbed data). Consequently, users who want to use our work should go there for a larger collection of models, datasets, and metrics.

To generate the resulting metric values reported in the paper, one has to do the following:
- Table 1, 2, and 3
  - Download the raw data for [*NuScenes*](https://github.com/DAI-Lab-HERALD/General-Framework-Adversarial-Attack/tree/main/Framework/Data_sets/NuScenes) and [*L-GAP*](https://github.com/DAI-Lab-HERALD/General-Framework-Adversarial-Attack/tree/main/Framework/Data_sets/CoR_left_turns)
  - Train *Trajectron++* on *NuScenes* and *L-GAP*, runing [simulations_train.py](https://github.com/jhagenus/General-Framework-update-adversarial-Jeroen/blob/main/Framework/simulations_train.py). The resulting model can be found in the [Results folder](https://github.com/DAI-Lab-HERALD/General-Framework-Adversarial-Attack/tree/main/Framework/Results/L-GAP%20(left%20turns)).
  - Generate adversarial attacks on *L-GAP* and the resulting metrics.
    - To get the results on the unperturbed data, run [simulations_no_perturbation.py](https://github.com/DAI-Lab-HERALD/General-Framework-Adversarial-Attack/blob/main/Framework/simulations_no_perturbation.py).
    - To get the main metrics on the perturbed data, run [simulations_perturbation.py](https://github.com/DAI-Lab-HERALD/General-Framework-Adversarial-Attack/blob/main/Framework/simulations_perturbation.py). 
    - To get the $CR_{FNC}$ metric on the perturbed data, run [simulations_perturbation_CR_FNC.py](https://github.com/DAI-Lab-HERALD/General-Framework-Adversarial-Attack/blob/main/Framework/simulations_perturbation.py). 
- Table 4
  - Download the raw data for [*HighD*](https://github.com/DAI-Lab-HERALD/General-Framework-Adversarial-Attack/tree/main/Framework/Data_sets/HighD_highways).  
  - Train *ADAPT* on *HighD*, runing [simulations_train_highD.py](https://github.com/jhagenus/General-Framework-update-adversarial-Jeroen/blob/main/Framework/simulations_train_highD.py). The resulting model can be found in the [Results folder](https://github.com/DAI-Lab-HERALD/General-Framework-Adversarial-Attack/tree/main/Framework/Results/HighD%20(Lane%20Change)).
  - Generate adversarial attacks on *HighD* and the resulting metrics.
    - To get the results on the unperturbed data, run [simulations_no_perturbation_highD.py](https://github.com/DAI-Lab-HERALD/General-Framework-Adversarial-Attack/blob/main/Framework/simulations_no_perturbation_highD.py).
    - To get the main metrics on the perturbed data, run [simulations_perturbation_highD.py](https://github.com/DAI-Lab-HERALD/General-Framework-Adversarial-Attack/blob/main/Framework/simulations_perturbation_highD.py). 
    - To get the $CR_{FNC}$ metric on the perturbed data, run [simulations_perturbation_CR_FNC_highD.py](https://github.com/DAI-Lab-HERALD/General-Framework-Adversarial-Attack/blob/main/Framework/simulations_perturbation_highD.py). 
- Table 5 and 6
  - Download the raw data for [*RounD*](https://github.com/DAI-Lab-HERALD/General-Framework-Adversarial-Attack/tree/main/Framework/Data_sets/RounD_round_about). 
  - Train *Trajectron++* and *ADAPT* on *RounD*, runing [simulations_train_rounD.py](https://github.com/jhagenus/General-Framework-update-adversarial-Jeroen/blob/main/Framework/simulations_train_rounD.py). The resulting model can be found in the [Results folder](https://github.com/DAI-Lab-HERALD/General-Framework-Adversarial-Attack/tree/main/Framework/Results/RounD%20(roundabout)).
  - Generate adversarial attacks on *HighD* and the resulting metrics.
    - To get the results on the unperturbed data, run [simulations_no_perturbation_rounD.py](https://github.com/DAI-Lab-HERALD/General-Framework-Adversarial-Attack/blob/main/Framework/simulations_no_perturbation_rounD.py).
    - To get the main metrics on the perturbed data, run [simulations_perturbation_rounD.py](https://github.com/DAI-Lab-HERALD/General-Framework-Adversarial-Attack/blob/main/Framework/simulations_perturbation_rounD.py). 
    - To get the $CR_{FNC}$ metric on the perturbed data, run [simulations_perturbation_CR_FNC_rounD.py](https://github.com/DAI-Lab-HERALD/General-Framework-Adversarial-Attack/blob/main/Framework/simulations_perturbation_rounD.py). 

A compressed version of the Results folder with all the perturbated data, predictions, and metrics can be found at 4TU.ResearchData. Simply extract the *Results.zip* file in the [Framework folder](https://github.com/DAI-Lab-HERALD/General-Framework-Adversarial-Attack/tree/main/Framework).


