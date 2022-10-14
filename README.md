# Acoustic-Fire-Extinguisher-Classification

###Data origin
On Acoustic_Extinguisher_Fire_Dataset_Citation_Request.txt you can read how this dataset was created and how his parameters where defined.

###Preprocessing
This project explore this dataset with the objective to create a model that can classify parameters like this and determined if the fire would be succefully extinguished or not. 

The Sizes came already interpreted on the original dataset because they come from different types of measurements, but we do have the original ones, like 1 represent a 7cm canister and 6 half throttle setting from this I generate a new columns for each fuel type. For each experiment we did: If that experiment didn't used a fuel type we designed 0 to that fuel respective column, for the fuel type he did used we put the size of the fuel on centimeters, but for gas fuel we did half throttle being 1 and full throttler 2.

###Spliting data
I split or data in 3 parts 80% for training, 20% for evaluation and 20% for test.

###Model
The model used was a simples MLP using tensorflow and 5 dense layers with a decreasing unity quantity.
