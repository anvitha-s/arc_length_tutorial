# arc_length_tutorial
The notebooks need to be opened on the jupyterlab/jupyter notebook interface in a conda environment created in a command below. If you don't know what any of this means use the instructions below to run these on the cluster in your browser.

## Using Princeton Clusters (web interface)

The steps have been described for adroit, but the same can be done on della using the mydella interface

New users of Adroit can request access to the Adroit cluster by submitting the form on this link : [https://forms.rc.princeton.edu/registration/?q=adroit](https://forms.rc.princeton.edu/registration/?q=adroit). This is usually automatically approved. 
New users start with a default of 10GB storage and existing users of adroit need to make sure their storage quota doesn't max out after installing fenics which takes ~3GB. You can check your cluster storage stats and/or request additional storage by following the instructions on the link below.

[Checking your quota and requesting quota increases](https://researchcomputing.princeton.edu/support/knowledge-base/checkquota)

Once you have access and enough storage on the cluster follow the steps below:

1. Go to MyAdroit([https://myadroit.princeton.edu/](https://myadroit.princeton.edu/)) and click on Clusters→shell on the top left corner, this should open a terminal to your account on Adroit. Run the commands below to install an environment with fenics.

   ```bash
   module load anaconda3/2020.11
   conda create -n fenics_tutorial -c conda-forge fenics matplotlib python=3.9.7 jupyterlab
   ```

2. In MyAdroit([https://myadroit.princeton.edu/](https://myadroit.princeton.edu/)) launch a Jupyter notebook(under Interactive Apps) by entering the "Number of hours" and “Number of cores”(1 is sufficient for this tutorial) on in the anaconda choose “Use your conda env fenics_tutorial”and then click on "Launch".When your session is ready click "Connect to Jupyter". 

3. Testing: The first cell in either of the notebooks should run without any errors
