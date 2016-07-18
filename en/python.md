# Installation Guide: Python for Topic Modeling

![Python](https://upload.wikimedia.org/wikipedia/commons/f/f8/Python_logo_and_wordmark.svg)

[Python](https://www.python.org) is a general-purpose, interpreted and widely used programming language. Its design philosophy emphasizes code readability and simple syntax, as well as an extensive standard library and numerous packages available on [PyPI](https://pypi.python.org/pypi). Compared to other programming languages, Python code is considerably shorter.


Use this guide to install Python 3, [numpy](http://www.numpy.org), [matplotlib](http://matplotlib.org) and [gensim](https://radimrehurek.com/gensim/).

## Navigation
1. [Installation on Windows](#windows-installing-python-and-packages)
2. [Installation on OS X](#os-x-installing-python-and-packages)
3. [Installation on Linux](#linux-ubuntu-installing-python-and-packages)

***

#### Windows: Installing Python and packages
1. Click [here](https://www.python.org/ftp/python/3.5.2/python-3.5.2-amd64.exe) to download the installation file
2. Open the file `python-3.5.2.exe` and follow the instructions
3. Ensure that **Add Python to PATH** is selected
4. Open the terminal using the key combination **Windows key + R**
5. Upgrade the setup-tool **pip** with `pip3 install --upgrade pip`
6. `pip3 install numpy matplotlib gensim` will install all pertinent Topic Modeling packages

***

#### OS X: Installing Python and packages
1. Click [here](https://www.python.org/ftp/python/3.5.2/python-3.5.2-macosx10.6.pkg) to download the installation file
2. Open the file `python-3.5.2-macosx10.6.pkg` and follow the instructions
3. Open Spotlight search using the key combination **cmd + Spacebar**, type **terminal** and then press Enter
4. Upgrade the setup-tool **pip** with `pip3 install --upgrade pip`
5. `pip3 install numpy matplotlib gensim` will install all pertinent Topic Modeling packages

***

#### Linux Ubuntu: Installing Python and packages
**Note**: Ubuntu 16.04 comes with Python 3, in this case skip step two.

1. Open the terminal using the key combination **Ctrl + Alt + T**
2. Install Python 3 with `sudo apt-get install python3`
3. `sudo apt-get install python3-pip` will install the setup-tool **pip** (alternatively use `sudo pip3 install --upgrade pip` to upgrade)
4. Use `sudo pip3 install numpy matplotlib gensim` to install all pertinent Topic Modeling packages
