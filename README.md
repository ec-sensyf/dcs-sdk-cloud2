dcs-sdk-cloud2
==============

DESCRIPTION

This repository contains the second approach of the usecase to test the deployment on the operational cloud environment.

IDEA: Get Landsat 8 data from the catalogue, for a defined region, and crop small ROIs defined on kml files.
      The parallelization on this approach is performed by < product,half_of_the_ROIs > (half of the ROIs are cropped on each task) on Hadoop.

Usecase numbers:

Regions of interest (ROIs) - 3380 (1690 ROIs per task)

--------------

INSTRUCTIONS

1. Before enter on the sandbox run on your local machine:

      $ssh-add < username >.pem
      
2. Enter on the sandbox:

      $ ssh -A -i < username.pem > sensyf-sdk@< sandbox_host >
      
3. Run the following commands:

      $ cd

      $ git clone git@github.com:ec-sensyf/dcs-sdk-cloud2.git
      
      $ cd dcs-sdk-cloud2
      
      $ mvn install

--------------

Copyright (C) DEIMOS Engenharia S.A.
