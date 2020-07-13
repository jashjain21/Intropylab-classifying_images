# Intropylab-classifying_images
 Determining which CNN architecture model works best at classifying images of dogs and their breeds.

## Files present in this repository
* pet_images						: Contains 40 images 0f different breeds of dogs to be tested on the different architectural models
* uploaded_images					: Contains images uploaded to test whether it identifies isadog or not along with its breed	
* adjust_results4_isadog.py			: Create a function adjust_results4_isadog that adjusts the results dictionary to indicate whether or not the pet image label is of-a-dog, 
     								  and to indicate whether or not the classifier image label is of-a-dog.
* alexnet_pet-images.txt      		: Stats for pet_images on alexnet architecture  
* alexnet_uploaded-images.txt		: Stats for uploaded_images on alexnet architecture
* calculates_results_stats.py		: Calculates the statistics of the results of the program run using the classifier's model architecture to classify the images.
* check_images.py					: Main function to be run,Classifies pet images using a pretrained CNN model, compares these classifications to the true identity of the 										  pets in the images, and summarizes how well the CNN performed on the image classification task.Note that the true identity of the pet (or                                       object) in the image is indicated by the filename of the image.
* classifier.py						: Does the work of classifying the image when called and returns the index corressponding to the breed of the dog
* classify_images.py				: Create a function classify_images that uses the classifier function to create the classifier labels and then compares the classifier 											  labels to the pet image labels.
* dognames.txt						: Contains 223 names of different breeds of dogs
* get_input_args.py            		: Create a function that retrieves the following 3 command line inputs from the user using the Argparse Python module. If the user fails to 
							          provide some or all of the 3 inputs, then the default values are used for the missing inputs. Command Line Arguments:
     										1. Image Folder as --dir with default value 'pet_images'
     										2. CNN Model Architecture as --arch with default value 'vgg'
     										3. Text File with Dog Names as --dogfile with default value 'dognames.txt'
* get_pet_labels.py                 : Creates the pet labels from the image's filename. This function inputs:- The Image Folder as image_dir within get_pet_labels function and 
     								  as in_arg.dir for the function call within the main function. 
* imagenet1000_clsid_to_human.txt   : Dictionary containing various classes to classify even the non dog images 
* print_functions_for_lab_checks.py : This set of functions can be used to check your code after programming each function. The top section of each part of the lab contains
           							  the section labeled 'Checking your code'. When directed within this section of the lab one can use these functions to more easily check 										  your code.
* print_results.py					: Create a function print_results that prints the results statistics from the results statistics dictionary (results_stats_dic). It 
									  should also allow the user to be able to print out cases of misclassified dogs and cases of misclassified breeds of dog using the Results 
                                      dictionary (results_dic).  
* resnet_pet-images.txt				: Stats for pet_images on resnet architecture
* resnet_uploaded-images.txt		: Stats for uploaded_images on resnet architecture
* run_models_batch.sh				: Runs all three models to test which provides 'best' solution.Please note output from each run has been piped into a text file.
* run_models_batch_uploaded.sh		: Runs all three models to test which provides 'best' solution on the Uploaded Images.Please note output from each run has been piped into a 									   text file.
* test_classifier.py				: To demonstrate the proper usage of the classifier() function that is defined in classifier.py This function uses CNN model architecture 										  that has been pretrained on the ImageNet data to classify images. The only model architectures that this function 
          							  will accept are: 'resnet', 'alexnet', and 'vgg'. See the example usage below.
* vgg_pet-images.txt				: Stats for pet_images on vgg architecture
* vgg_uploaded-images.txt			: Stats for uploaded_images on vgg architecture

So basically run the run_models_batch file for printing out the results of the performance of the 3 models and run the run_models_batch_uploaded to test your own images against various networks.Name the file with the content of the images

Author:
Jash Jain [linkedin](https://www.linkedin.com/in/jash-jain-bb659a132)

License
This project is licensed under the MIT License - see the LICENSE.md file for details.
