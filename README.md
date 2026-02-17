# Hands-on Machine Learning Course for the Master in Photonics [UPC+UB+UAB+ICFO]

A set of Jupyter notebooks designed to introduce deep learning concepts applied to physics and photonics.

## Installation instructions

You can run these tutorials EITHER on [**1. Your Own Laptop**](#-1-using-your-own-laptop)
OR on [**2. Google Colab**](#-2-using-google-colab), see the two subsections below:

### · 1. Using your own laptop

This course requires a working Conda environment. Basic familiarity with the terminal (command line) is also recommended.

Using the terminal is an essential professional skill in Machine Learning, research, data science, and industry.

You are not merely installing software; you are learning how real-world machine learning environments are structured and managed.


#### Install Conda (Miniconda Recommended)

If you already has any version of conda on your computer, 
go directly to [the next preparation point](using-the-command-line).

We recommend installing **Miniconda** instead of the full Anaconda distribution,
because Miniconda is lighter and more stable.
However, you can use the full Anaconda if you prefer.

* <ins>Download Miniconda</ins>:

  From [https://docs.conda.io/en/latest/miniconda.html](https://repo.anaconda.com/miniconda/)
  download the Miniconda3 that suits for your operating system, choose just from the sevent first options
  (latest versions for Windows, MacOs and Linux).

  > If you have a regular Windows, just take the first one.

* <ins>Install Miniconda</ins>:

  During installation: Use the default installation path, do NOT manually add to PATH (leave default settings),
  and allow the installer to initialize Conda.

#### Using the command-line

* <ins>Select an appropriate terminal</ins>:

  You must use a terminal where Conda works correctly.

  * On Windows: Windows key → type "Anaconda Prompt"

  * On macOS / Linux: Open the standard **Terminal** application.

  Then, for any OS, in your terminal, type:

  ```bash
  conda --version
  ```

  You should see something like `conda 24.x.x`. If you see an error such as `conda is not recognized`,
  close the terminal and open again the Anaconda Prompt, or restart your computer.

* <ins>Understand the Prompt</ins>:

  When Conda is active, your terminal should look like:
  
  ```
  (base) C:\Users\YourName>
  ```
  
  The `(base)` means Conda is active. If you do NOT see `(base)`, run:
  
  ```bash
  conda activate base
  ```

#### Creating and activating a specific ML environment 

* <ins>Create the Course Environment</ins>:

  Run the following command exactly as written (copy & paste):

  ```bash
  conda env create -f https://raw.githubusercontent.com/dmaluenda/hands_on_machine_learning/master/environment.yml
  ```

  This will download the environment configuration from GitHub: Python 3.10, Jupyter, NumPy 1.26, TensorFlow 2.16, Gymnasium.
  
  This step may take 5–15 minutes. Do not interrupt it.

* <ins>Activate the Course Environment</ins>:

  After installation finishes, activate it:
  
  ```bash
  conda activate hands-on-ML
  ```
  
  Your terminal should now look like:
  
  ```
  (hands-on-ML) C:\Users\YourName>
  ```
  
  If you still see `(base)` or no brackets at all, the environment is not activated.

* <ins>Launch Jupyter Notebook</ins>:

  Run:
  
  ```bash
  jupyter lab
  ```
  
  Your browser should open automatically.

#### Run tutorials

Download the tutorials from the 
[course web at UPC-Atenea](https://atenea.upc.edu/course/section.php?id=914018) intranet.

> <ins>Alternatively</ins>, you can download the file you want from this GitHub repository
(those files in the list above ending with `.ipynb`)
by entering the file and clicking the `Download notebook` button at the top of each file.
You will most likely need to `right-click` + `Save As`.
Make sure that it ends with the `.ipynb` extension.
Take into account that if one file is in GitHub but it is not yet in UPC-Atenea, 
it is probably not in its final version. **Use only the 'master' branch** 
(if you are not familiar with Git branches, you may ignore this remark).

We recommend downloading and working on all tutorials in a single specific directory on your computer,
and avoiding working in the `Downloads` directory.

**Every time you work on this course**, you must repeat these steps:

1. Open terminal: Windows key → Anaconda Prompt
2. Activate the environment:  `conda activate hands-on-ML`
3. Start Jupyter: `jupyter lab`

A webpage should open in your internet browser with the Jupyter Lab interface.
Locate the specific folder where the tutorials are stored and click on one of them.
The tutorial should open in a new tab of your web browser.

You can **edit** (`[DoubleClick]` or `[Enter]`) and **run** (`[Shift] + [Enter]`) 
any cell in the Notebook.

Check the 
[**JupyterLab Documentation**](https://jupyterlab.readthedocs.io/en/latest/user/interface.html) and 
[**Notebooks Documentation**](https://jupyterlab.readthedocs.io/en/latest/user/notebook.html)
for detailed information.


### · 2. Using Google Colab

If you prefer not to run these tutorials on your own computer, 
you can run any tutorial in this repository in Google Colab.

Google Colab is a free service provided by Google that allows anyone to run Jupyter 
notebooks in the cloud. It is very easy to use and is a good option if you 
do not want to install anything on your computer, 
nor learn how to manage conda environments and terminal commands.

You just need to go to the specific tutorial (also from the PDF version) and 
click on the `Run in Google Colab` button at the top of the file.
That's all!

#### Google Colab Pros:
- Everything is ready to run from the start.
- You have access to one GPU (usually a Tesla T4) for faster execution. (Not needed for this course)

#### Google Colab Cons: 
- You need a Google account to use it.
- Only one notebook can run at once (in the free version).
- <ins>The code is not stored on your laptop, so you must make sure to save your changes</ins>.
- You need a reasonably stable internet connection.

The last two points are the most important limitations and should be carefully considered.

Check also the 
[**Jupyter Documentation**](https://jupyter-notebook.readthedocs.io/en/stable/notebook.html#notebook-user-interface)
for detailed information.





