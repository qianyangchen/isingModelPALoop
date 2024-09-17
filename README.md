# Ising model as Perception-Action Loop
This project contains code that uses the JIDT library to run various information-theoretic computations. Please follow the instructions on [JIDT home page](https://github.com/jlizier/jidt) to install the package. Some file paths in the code need to be customised based on your system setup.

## Setup Instructions
### Step 1: Clone the Repository
Clone this repository to your local machine:
```bash
git clone https://github.com/qianyangchen/isingmodelPALoop.git
```

### Step 2: Install Dependencies
Ensure that you have the required Python packages installed. You can install them via pip:
```bash
pip install -r requirements.txt
```

### Step 3: Create the Configuration File
In order to run the code properly, you will need to create a config.json file to specify local paths for the JIDT library and other resources.

Create a config.json file in the root directory of the project (where the Jupyter Notebook is located).
The structure of the config.json file should look like this:
```json
{
  "infodynamics_path": "/path/to/your/infodynamics-dist-1.6.1/demos/python",
  "jar_location": "/path/to/your/infodynamics-dist-1.6.1/infodynamics.jar"
}
```

Example config.json

If you have the JIDT library located in your home directory under /Users/username/, your config.json should look something like this:
```json
{
  "infodynamics_path": "/Users/username/infodynamics-dist-1.6.1/demos/python",
  "jar_location": "/Users/username/infodynamics-dist-1.6.1/infodynamics.jar"
}
```

### Step 4: Running the Jupyter Notebook
Once you have set up the config.json file, you can run the Jupyter Notebook as usual:
```bash
jupyter notebook
```
Ensure that the paths in your config.json file point to the correct locations where you have stored the necessary resources.

## Troubleshooting
FileNotFoundError: If you encounter this error, double-check the paths in the config.json file. Ensure the infodynamics_path and jar_location point to the correct files and directories.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
