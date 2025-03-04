SSD Implementation in Pytorch
========

### Instructions
1. First get to the SSD-PYTORCH directory and then run `pip install -r requirements.txt` command to make sure that you have the 
   compatible versions of the libraries
2. The download the VOC 2007 dataset from this link - http://host.robots.ox.ac.uk/pascal/VOC/voc2007 

   Step1: On clicking on this link you will be redirected to a page, go to the Development Kit section

   Step2: Download the training/validation data (450MB tar file)

   Step3: Go to Test Data section 

   Step4: Download the annotated test data (430MB tar file)

   After downloading the above two tar files, extract them.

   After extracting them, head to a directory `VOC2007` for both train/val and test files (path `VOCdevkit` -> `VOC2007`)

   Rename the test `VOC2007` directory from `test` data download to `VOC2007-test` 

   Place the above two directories in a directory named `data`

   After completing the above steps your tree structure should look like the structure below


      ```
      SSD-Pytorch
          -> data
              -> VOC2007
                  -> Annotations
                  -> ImageSets
                  -> JPEGImages
                  -> SegmentationClass
                  -> SegmentationObject
              -> VOC2007-test
                  -> Annotations
                  -> ImageSets
                  -> JPEGImages
                  -> SegmentationClass
                  -> SegmentationObject
              
          -> tools
              -> train.py
              -> infer.py
          -> config
              -> voc.yaml
          -> model
              -> ssd.py 
          -> dataset
              -> voc.py
      ```
3. Now that we are all set we can go ahead and train the model

   To train the model on the VOC dataset run the command : `python -m tools.train`

   Run `python -m tools.infer --evaluate False --infer_samples True` for generating inference predictions

   Run `python -m tools.infer --evaluate True --infer_samples False` for evaluating on test dataset


4. Output:

   Outputs will be saved according to the configuration present in yaml files.

   For every run a folder of `task_name` key in config will be created

   During training of SSD the following output will be saved

   Latest Model checkpoint in `task_name` directory

   During inference the following output will be saved

   Sample prediction outputs for images in `task_name/samples`

5. Configuration:

   To try out different model configurations, you can make changes to
   
   `config/voc.yaml` file



