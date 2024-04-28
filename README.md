# R Jupyter Notebooks in VS Code on MacOS

## Setup from scratch

- Install [Homebrew](https://brew.sh/)

- Install [VS Code](https://code.visualstudio.com/) using `brew install --cask visual-studio-code`

  - Install the [R extension](https://marketplace.visualstudio.com/items?itemName=REditorSupport.r)

  - Install the [Jupyter extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)

- Install [Python](https://www.python.org/)

  - Install using `brew install python`

- Set up your project

  - `mkdir r-notebook-example`

  - `cd example`

  - Create a virtual Python environment

    - Install using `python3 -m venv env`

    - Activate using `source env/bin/activate`

  - Install Jupyter using `pip3 install jupyter`

- Install [R](https://www.r-project.org/) using `brew install r`

  - Install the R kernel for Jupyter by running `R` to open R and then running:

    ```
    install.packages('IRkernel')
    IRkernel::installspec(user = FALSE)  # Installs the kernel system-wide
    ```

- Open your project in VS Code

  - `code .`

  - Create and open a new file called `example.ipynb`

  - Add the following code:

    ```r
    print("Hello, world!")
    ```

  - Select the R kernel in the top right

  - Run the code by clicking "Run All" in the top left
