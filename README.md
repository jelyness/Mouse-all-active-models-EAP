Associations between in vitro, in vivo and in silico cell classes in mouse primary visual cortex (Wei et al, 2021)

## Instructions

* 1)  Create a virtual environment
        ```
        $ conda create -n bmtk-ateam python=2.7 
        $ conda activate bmtk-ateam
        $ conda install pandas numpy matplotlib scikit-learn
        ```
        
* 2)  Install bmtk
      ```
       $ git clone https://github.com/yinawei/bmtk.git
       $ pip install -e /Users/yinawei/Documents/Allen/bmtk-ateam
      ```
     
* 3)  Install NEURON
        ```
       $ pip install neuron
       ```
       
* 4) Install ateam-tools
       ```
      $pip install -e ateam-tools
      ```
     
* 5)  Compile the modifiles

       After installing bmtk, run
       ```
       $ cd examples/biophys_components/mechanisms 
       $ nrnivmodl modfiles/ # this should create a directory x86_64
      ```
     If you have trouble in this step, make sure you have deleted "x86_84" before compling the modfiles.

* 6) Run simulations

      In the example folder "395830185", run the simulations using the following commands:
      ```
      $ python build_network.py
      $ python run_bionet.py
     ```
      
      
## Dependencies
 * Python 2.7
 * pandas
 * Matplotlib
 * scikit-learn
 * numpy

