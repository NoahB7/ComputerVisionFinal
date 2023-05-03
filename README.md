# ComputerVisionFinal
All files included are just ones that I've modified. 
Replaced the deprecated libraries so that the cells run and created the modified model architecture, (which is working) just havent trained anything yet.
All that remains is being able to run the training portion so that we can train the original and the modified and compare the results.

Edits:

SANet.py and modified : keras_contrib.layers import InstanceNormalization -> from tensorflow_addons.layers import InstanceNormalization
utils.py : from skimage.measure import compare_psnr, compare_ssim -> from skimage.metrics import peak_signal_noise_ratio as compare_psnr
                                                                      from skimage.metrics import structural_similarity as compare_ssim

utils.py (line 328) reduce dimensions or something function arg name changed to axis

Running the cells up to this point assumes that the data is in a folder named "data" (same one with the file paths to the images)
