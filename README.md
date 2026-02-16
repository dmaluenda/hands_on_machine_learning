# Hands on Machine Learning course of Master in Photonics [UPC+UB+UAB+ICFO]

Set of Jupyter notebooks to learn deep learning for physics and photonics.

## Installation instructions

You can run these tutorials either in **1. Your Own Laptop** <ins>or</ins> in 
**2. Google Colab**, see the two subsections below:

### · 1. Using your own laptop

This course requires a working Conda environment and basic use of the terminal (command line) is a supplementary useful knowledge.

---

## 1. Install Conda (Miniconda Recommended)

We recommend installing **Miniconda** instead of the full Anaconda distribution,
because Miniconda is lighter and more stable.
However, you can use the full Anaconda if you prefer.

### Step 1: Download Miniconda

Go to:

https://docs.conda.io/en/latest/miniconda.html

Download:

- Miniconda3
- Python 3.10 or 3.11 version
- 64-bit installer for your operating system

On Windows: download the `.exe` installer.

### Step 2: Install

During installation:

- Install for **Just Me**
- Use the default installation path
- Do NOT manually add to PATH (leave default settings)
- Allow the installer to initialize Conda


## 2. Open the Terminal

You must use a terminal where Conda works correctly.

### On Windows

Press: Windows key → type "Anaconda Prompt"

Open **Anaconda Prompt**.

You may use PowerShell only if Conda works there.

### On macOS / Linux

Open the standard **Terminal** application.

---

## 3. Verify That Conda Works

In the terminal, type:

```bash
conda --version
```

You should see something like:

```
conda 24.x.x
```

If you see an error such as:

```
conda is not recognized
```

Close the terminal and open Anaconda Prompt instead, or restart your computer.

---

## 4. Understand the Prompt

When Conda is active, your terminal should look like:

```
(base) C:\Users\YourName>
```

The `(base)` means Conda is active.

If you do NOT see `(base)`, run:

```bash
conda activate base
```

---

## 5. Create the Course Environment

Run the following command exactly as written:

```bash
conda env create -f https://raw.githubusercontent.com/dmaluenda/hands_on_machine_learning/master/environment.yml
```

This will:

- Download the environment configuration from GitHub
- Install Python 3.10
- Install TensorFlow
- Install JupyterLab
- Install all required packages

This step may take 5–15 minutes. Do not interrupt it.

---

## 6. Activate the Course Environment

After installation finishes, activate it:

```bash
conda activate hands-on-ML
```

Your terminal should now look like:

```
(hands-on-ML) C:\Users\YourName>
```

If you still see `(base)`, the environment is not activated.

---

## 7. Launch Jupyter Lab

Run:

```bash
jupyter lab
```

Your browser should open automatically.

If it does not open:

- Copy the URL shown in the terminal
- Paste it into your browser manually

---

## 8. Test That Everything Works

Create a new notebook and run:

```python
import tensorflow as tf
import numpy as np

print("TensorFlow:", tf.__version__)
print("NumPy:", np.__version__)
```

If versions are printed and no errors appear, your setup is correct.

---

## Every Time You Work on This Course

You must repeat these steps:

1. Open terminal  
2. Activate the environment  

```bash
conda activate hands-on-ML
```

3. Start Jupyter  

```bash
jupyter lab
```

If you forget to activate the environment, things will not work.

---

## Common Problems

### "conda is not recognized"

Use Anaconda Prompt or reinstall Miniconda.

### Installation is slow

If you are:

- Inside a OneDrive folder
- On a university network
- Behind antivirus software

Installation may be slower. This is normal.

### "jupyter command not found"

Make sure you activated the environment first:

```bash
conda activate hands-on-ML
```

---

## Why We Use the Terminal

Using the terminal is an essential professional skill in:

- Machine Learning
- Research
- Data Science
- Industry

You are not just installing software — you are learning how real-world ML environments are managed.


#### Dependencies

You can install the dependencies by running the
[00_install_dependencies.ipynb](00_install_dependencies.ipynb)
notebook. So, follow the next section below to run it as a demo, 
and then you will be ready for all the rest tutorials.


#### Run tutorials

Download the tutorials from the 
[course web at UPC-Atenea](https://atenea.upc.edu/course/view.php?id=95161#section-3) intranet.

<ins>Alternativelly</ins> , you can download the file you want from this GitHub repository
(those files on the list above ended with `.ipynb`)
by means of entering and click the `Download notebook` button on top of every file.
Probably, you should `[RightClick]+SaveAs` to download the content in a 
certain file. Make sure that it ends with the `.ipynb` extension.

> Take into a count that if one file is in GitHub, but it is not in the UPC_Atenea yet, 
it is probably not in its final version. **Use only 'master' branch** 
(if you do not know what does branch mean, forget it).

We recommend to download and work on all tutorial in a single specific directory of your computer.

Then, open Anaconda and launch the Jupyter Notebooks App from the Anaconda Navigator.
A webpage should be opened in your internet browser with a kind of file browser.
Find here that specific folder where the tutorials are located and click on one of them.
Now, the tutorial should be opened in a new tab of your web browser.
You can **edit** (`[DoubleClick]` or `[Enter]`) and  **run** (`[Shift]+[Enter]`) 
any cell in the Notebook.

Check the 
[**Jupyter Documentation**](https://jupyter-notebook.readthedocs.io/en/stable/notebook.html#notebook-user-interface)
for detailed information.


### · 2. Using Google Colab

If you prefer do not run these tutorials in your own computer, 
you can run any tutorial on this repository in Google Colab (excepting for the 00_installing_dependencies.ipynb).

Google Colab is a free service provided by Google that allows anyone to run Jupyter 
notebooks in the cloud. It is very easy to use, and it is a good option if you 
do not want to install anything in your computer.

You just need to go in to that specific tutorial (also from the pdf version) and 
click on the `Run in Google Colab` button on top of the file.
That's all!

#### Google Colab Pros:
- All is ready to run there, from the very beginning.
- You have one GPU (usually a Tesla4) to get faster. (Not needed for this course)

#### Google Colab Cons: 
- You need a Google account to use it.
- Only one notebook can run at once (in the free version).
- <ins>The code is not in your laptop, so you have to take care to save your changes</ins>.
- You need a quite stable internet connection.

The last two are the most important cons, have them in mind.

Check also the 
[**Jupyter Documentation**](https://jupyter-notebook.readthedocs.io/en/stable/notebook.html#notebook-user-interface)
for detailed information.

