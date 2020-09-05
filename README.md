# **Reconstruction of Vehicle Trajectories**

## Generating and plotting data for visualization

### Using tools to visualize raw data

---

**Reconstruction of Vehicle Trajectories Project**

The goals / steps of this project are the following:

* Generate data save in pickled file for visualization later
* Reconstruct trajectories and compared with pickled file

[//]: # (Image References)

[image1]: ./Result_Images/1.png "1"
[image2]: ./Result_Images/2.png "2"
[image3]: ./Result_Images/3.png "3"

### README

- The generating data for visualization can be found [here](./Trajectories_Data_Generator.ipynb) and an example of accelerating and then turn 270 degrees left is shown:

![alt text][image1]

- The data generated by previous step was save in a pickled file and used [here](./Reconstructing_of_Vehicle_Trajectories.ipynb) for comparison.

### Steps used for vehicle trajectories.

#### 1. Generate data.

* A Car class was initialized with various functions such as reverse, forward, steer, gas, go, etc.

  - 1st Manuever: accelerate and then turn 270 degrees left

![alt text][image1]

   - 2nd Manuever: accelerate onto highway and change lanes

![alt text][image2]

   - 3rd Manuever: parallel parking

![alt text][image3]

#### 2. Reconstuct trajectory data

* The raw input data is saved in pickled files and can be loaded using a [helper function](./helpers.py)

  - The data list loaded contains four fields, correspond to:
   - timestamp (seconds)
   - displacement (meters)
   - yaw_rate (rads / sec)
   - acceleration (m/s/s)

* The job is to complete [functions](./solution.py), all of which take a processed data_list (with 𝑁 entries, each Δ𝑡 apart) as input to reconstruction the vehicle trajectories. 







