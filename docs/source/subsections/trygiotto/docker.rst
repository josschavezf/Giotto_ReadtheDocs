.. _DockerInformation:

#########################
Docker Image with RStudio
#########################

We have set up a `Docker Image <https://hub.docker.com/r/giottopackage/rstudio_master>`__ linked to RStudio with Giotto pre-installed.

Instructions
=============

Follow these instructions to create your own Docker container and run Giotto:

1. docker pull ``giottopackage/rstudio_master:latest``

2. docker run ``--rm -p 8787:8787 -e PASSWORD=mypassword giottopackage/rstudio_master:latest``

   1. You may use *any* port as long as it is not in use.
   2. You can set the password to *whatever* you like.

3. Open the browser of your choice and enter `localhost:yourport`.

   1. Where yourport is either 8787 or the port you assigned it in step 2.

4. You will be directed to an RStudio login.

   1. Username: rstudio
   2. Password: mypassword

      * **Note**: The password you enter will be whatever you declared in step 2.

5. Run the following **in RStudio**:

   1. library(Giotto)

6. Now you can run any analysis with Giotto!

###############################
Docker Image with bash terminal
###############################


If you prefer to run your analysis directly on the terminal, we have set up a `Docker Image <https://hub.docker.com/r/giottopackage/master>`__ able to run in a bash environment.

Instructions
=============

Follow these instructions to create your own Docker container and run Giotto:

1. docker pull ``giottopackage/master:latest``

2. docker run ``-ti giottopackage/master:latest /bin/bash``

3. R

4. Run the following **in R**:

   1. library(Giotto)

5. Now you can run any analysis with Giotto!



