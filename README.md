# Monocular Depth Estimation OSDS Project.
## Demo

**You can use given notebook to load a model from the project and run it on an image you uploaded, to get the depth map. Once it has been saved, you can download it to use on platforms that support it (e.g. Facebook) to create 3d photos.**

**You can also use this notebook to load a model from the project and run it on an image you uploaded, to get the depth map. Once it has been saved, you can download it to use on platforms that support it (e.g. Facebook) to create 3d photos.**


In order to edit code files, you must save the notebook to your drive. You can do this by typing `ctrl+s` or `cmd+s` on mac.

**_NOTE: The downside of using google colab method (if you are not familiar with Colab) is that Google Colab will limit the amount of time an instance can be live, so you might be limited in your ability to train models for longer periods of time._**

This notebook is also a part of this project, in case it needs modification, in the `Notebooks` folder. You should not commit your version unless your contribution is an improvement to the environment.

#### Local
* Clone the repository you just forked by typing the following command in your terminal.
  
* Create a virtual environment or Conda environment and activate it
    ```bash
    # Create the virtual environment
    $ make env
  
    # Activate the virtual environment
    # VENV
    $ source env/bin/activate .
  
    # or Conda
    $ source activate __________
    ```
* Install the required libraries
    ```bash
    $ make load_requirements
    ```
  **_NOTE: Here I assume a setup without GPU. Otherwise, you might need to modify requirements, which is outside the scope of this readme (feel free to contribute to this)._**
    
#### Docker
* Clone the repository you just forked in your terminal.
  
* To get your environment up and running docker is the best way to go. We use an instance of [MLWorkspace](https://github.com/ml-tooling/ml-workspace). 
    * You can Just run the following commands to get it started.

        ```bash
        $ chmod +x run_dev_env.sh
        $ ./run_dev_env.sh
        ```

    * Open localhost:8080 to see the workspace you have created. You will be asked for a token – enter `dagshub_savta`
    * In the top right you have a menu called `Open Tool`. Click that button and choose terminal (alternatively open VSCode and open terminal there) and type in the following commands to install a virtualenv and dependencies:

        ```bash
        $ make env
        $ source activate _____
        ```
        
        Now when we have an environment, let's install all of the required libraries.
        
        **Note**: If you don't have a GPU you will need to install pytorch separately and then run make requirements. You can install pytorch for computers without a gpu with the following command:

        ```bash
        $ conda install pytorch torchvision cpuonly -c pytorch
        ```
        
        To install the required libraries run the following command:
        
        ```bash
        $ make load_requirements
        ```

* After you are finished your modification, make sure to do the following:
    * If you modified packages, make sure to update the `requirements.txt` file accordingly.

### TODO:
- [ ] Web UI
- [ ] Testing various datasets as basis for training
- [ ] Testing various models for the data
- [ ] Adding qualitative tests for model performance (visually comparing 3d image outputs)
