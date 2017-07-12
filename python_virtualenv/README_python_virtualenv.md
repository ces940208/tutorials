# Setting up Python virtual environments

If you have or require different versions of python with a different set of libraries,
or if one of the programs you are using requires a particular python set-up that doesn't match 
your regular needs, stay a bit and read along.

The commands in this README file are also present as a bash script in the same directory.





## 1. Install pip

Some linux distributions already have 2 versions of python installed as default 2.7.X and 3.X.X,
check the links and executables installed and chose the one to work with.

```bash
ls -l /usr/bin/pyt*
```

Choose the default version of python you would like to use.
Beware not to update this version, since the libraries to use _virtualenv_ will depend on it.
We'll create virtual environments for the other versions you'd like to use.



### a. Install pip on 2.7.X

As of today, july 2017, `pip` will install pip on python 2.7.X.
After the installation you'll probably have to update it

```bash
sudo apt-get install pip
pip install --upgrade pip
```



### b. Install pip on 3.X.X

It's almost the same thing

```bash
sudo apt-get install python3-pip
```





## 2. Install virtualenv library

For 2.7.X:

```bash
pip install virtualenv
```

For 3.X.X:

```bash
pip3 install virtualenv
```




## 3. Create a directory where your environments will all be stored

The tutorials advise to put this directory in your home, so let's follow their directions

```bash
mkdir ~/Environments
```




