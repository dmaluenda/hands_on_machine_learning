# Hands on Machine Learning course of Master in Photonics [UPC+UB+UAB+ICFO]

Set of Jupyter notebooks to learn deep learning for physics and photonics.

## Installation instructions

You can run these tutorials either in **1. Your Own Laptop** <ins>or</ins> in 
**2. Google Colab**, see the two subsections below:

### · 1 Using your own laptop

These tutorials are coded in Jupyter notebooks with Python language. 
Jupyter is included in the Anaconda environment, so we strongly recommend downloading 
and installing [Anaconda](https://www.anaconda.com/products/individual).
Open Anaconda on your computer and install Jupyter Notebook from the Anaconda Navigator.
Also install the Powershell prompt, if it is not already
(it is not needed, but it can be useful in some situations).

![Screenshoot of the Jupyter installation button](https://github.com/dmaluenda/hands_on_machine_learning/blob/master/resources/jupyter_install.png)

#### Dependencies

You can install the dependencies by running the
[00_install_dependencies.ipynb](00_install_dependencies.ipynb)
notebook. So, follow the next section below to run it as a demo, 
and then you will be ready for all the rest tutorials.


#### Run tutorials

Download the tutorials from the 
[course web at UPC-Atenea](https://atenea.upc.edu/course/view.php?id=85709) intranet.

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
Now, the tutorial should be opened in a new tab of your browser.
You can **edit** (`[DoubleClick]` or `[Enter]`) and  **run** (`[Shift]+[Enter]`) 
any cell in the Notebook.

Check the 
[Jupyter Documentation](https://jupyter-notebook.readthedocs.io/en/stable/notebook.html#notebook-user-interface)
for detailed information.


### · 2 Using Google Colab

If you prefer don't to run these tutorials in your own computer, 
you can run any tutorial on this repository in Google Colab.

Google Colab is a free service provided by Google that allows anyone to run Jupyter 
notebooks in the cloud. It is very easy to use, and it is a good option if you 
don't want to install anything in your computer.

You just need to go in to that specific tutorial (also from the pdf version) and 
click on the `Run in Google Colab` button on top of the file.
That's it!

#### Google Colab Pros:
- All is ready to run there, from the very beginning.
- You have one GPU (usually a Tesla4) to get faster. (Not needed for this course)

#### Google Colab Cons: 
- You need a Google account to use it.
- Only one notebook can run at once (in the free version).
- Probably, you cannot see the equation numbers (usful for the second tutorial).
- The code is not in your laptop, so you have to take care to save your changes.
- You need a quite stable internet connection.

The last two are the most important cons, have them in mind.
