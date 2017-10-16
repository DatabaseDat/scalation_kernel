# scalation_kernel

This project provides a [Scala+ScalaTion](http://cobweb.cs.uga.edu/~jam/scalation.html)
kernel for [Jupyter](http://jupyter.org). It uses the system's or container's
Scala installation for the underlying REPL. This implementation uses
```ipykernel``` and ```pexpect``` to allow the kernel to easily interact with
the REPL. 

![Screenshot](https://i.imgur.com/TTRigOG.png)

## Python Dependencies

Below are the Python packages that this project directly depends on:

* ```pexpect``` (>=4.2.1)
* ```ipykernel``` (>=4.6.1)

## Installation

To install the developer version of ```scalation_kernel``` using PIP:
```
$ git clone https://github.com/scalation/scalation_kernel.git
$ python3 -m pip install -e scalation_kernel
$ python3 -m scalation_kernel.install
```

## Run Jupyter

Before you run Jupyter, you need to make sure the following environment
variables are set with the full paths to the ScalaTion JAR files:
```
$ export SCALATION_MATHSTAT_JAR=/path/to/scalation_mathstat_2.12-1.3.jar
$ export SCALATION_MODELING_JAR=/path/to/scalation_modeling_2.12-1.3.jar
```

To run Jupyter, you might use the following command:
```
$ python3 -m jupyter notebook
```

## Using the ScalaTion kernel

**Notebook**: The *New* menu in the notebook should show an option for a
"ScalaTion" notebook.

