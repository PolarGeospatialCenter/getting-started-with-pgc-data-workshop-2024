# getting-started-with-pgc-data-workshop-2024

## Setup

The workshop utilizes `conda`, via the Anaconda distribution, to build the execution environment for the Jupyter notebook exercises.

1. Download the contents of this repository as a zip archive: [Download Zip](https://github.com/PolarGeospatialCenter/getting-started-with-pgc-data-workshop-2024/archive/refs/heads/main.zip).

2. Extract the zip archive content to an accessible directory on your local machine.

3. Open `Anaconda Prompt` and navigate to the directory of the extracted archive.

4. Set `libmamba` as the dependency solver. This will allow us to use the significant speed increases of `mamba` within the `Anaconda` ecosystem.
    ```bash
    conda config --set solver libmamba
    ```
   If you get a `CondaValueError` you might need to first install the `conda-libmamba-solver` package:
   ```bash
   conda install -n base conda-libmamba-solver
   ```

5. Create the workshop environment from the provided `environment.yml` file. This might take a few minutes to complete.
    ```bash
    conda env create --name pgc-user-workshop-2024 --file environment.yml
    ```

6. Activate the environment.
    ```bash
    conda activate pgc-user-workshop-2024
    ```

7. Launch Jupyter Lab.
    ```bash
    jupyter lab
    ```