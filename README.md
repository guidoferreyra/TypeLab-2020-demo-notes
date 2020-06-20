# Create a virtual environment and install fontmake

1. Open the Terminal

2. Navigate to the folder where you want to create your virtual environment . For this case Im going to create it inside my  home folder. To navigate to that folder use:

```
cd ~
```

3. Create the virtual environment using the following command: 

```
virtualenv -p python3 myToolsEnv
```

`myToolsEnv` will be the name for the virtual environment and the directory that will contain all the dependencies. (You can use whatever name you want).

4. Before install any package or tool we need to activate the virtual environment with:

   ```
   source myToolsEnv/bin/activate
   ```

   You will notice that your environment is activated because the prompt will show the name of it .

5. Now we have to install the packages we are going to use: 
   For instance to install fontmake with pip we use the following command:

   ```
   pip install fontmake
   ```

   Alternative you can install packages from a requirements.txt file, this is very common to see in public font repositories.

   ```
   pip install -r requirements.txt
   ```

6. Now you can use fontmake or any other tool you have installed

   ```
   fontmake path/to/your/font
   ```

7. To exit of the virtual environment use:

   ```
   deactivate
   ```

8. To reactivate the environment you just need to use command from the step 4 . Hoewever is convenient to set an alias (shortcut) for this by adding the following line to your config file.

   ```
   alias myTools="source ~/myToolsEnv/bin/activate"
   ```

   This config file is a hidden file that can be diffrent depending with shell interpreter are you using. For example for bash the file can be located in `~/.bash_profile` and for zsh it can be at `~/.zshrc`

