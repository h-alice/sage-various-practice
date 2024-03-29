# SageMath Practice Repository

Welcome to the SageMath Practice Repository!

This repository houses various practice materials (mostly in Jupyter notebook format) for SageMath. SageMath is a powerful open-source mathematical tool in Python, it has been used across diverse mathematical domains, even including cryptography challenges encountered in Capture The Flag (CTF) competitions.

**Important Note:** Before exploring the notebooks in this repository, ensure you have SageMath installed on your system. Refer to the [official website](https://doc.sagemath.org/html/en/installation/index.html) for installation instructions.

These notebooks are intended for practice purposes. Expect to encounter errors and mistakes as you work through them.

**How did you find this repository?** Regardless, you can utilize it as a reference for using SageMath.

## Installation of SageMath

To install SageMath, please follow the instructions provided on the [official website](https://doc.sagemath.org/html/en/installation/index.html).

## Syntax Highlighting for SageMath in VSCode
NOTE: These instructions are tested on MacOS. The steps may vary for other operating systems.

1. Check the SageMath jupyter kernel location by running the following command in the terminal:
    ```bash
    sage -sh -c 'echo $JUPYTER_PATH'
    ```
    In my environment, the output is:
    ```bash
    /var/tmp/sage-10.3-current/Resources/jupyter
    ```
2. Locate the `site-packages` directory for the SageMath kernel, it may be inside the `venv` folder of SageMath.  
    In my environment:
    ```bash
    /var/tmp/sage-10.3-current/venv/lib/python3.11/site-packages
    ```
3. Add the path of `site-packages` to the search path of Pylance in VSCode.  
    Create a `settings.json` file in the `.vscode` directory of your project, and add the line below:
    ```json
    "python.analysis.extraPaths": [ "/var/tmp/sage-10.3-current/venv/lib/python3.11/site-packages" ],
    ```
4. Close, and reload the VSCode window, everything should work fine now.

## Reference Material

For further learning and exploration, consider referring to the following resources:

- [SageMath Documentation](http://doc.sagemath.org/html/en/index.html)
- [SageMath Tutorial](http://doc.sagemath.org/html/en/tutorial/index.html)
- [Abstract Algebra: Theory and Applications](http://abstract.ups.edu/sage-aata.html)
- [Learning and Experiencing Cryptography with CrypTool and SageMath](https://www.cryptool.org/en/documentation/ctbook/)

Hopy you find this repository useful.