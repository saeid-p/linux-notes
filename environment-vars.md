To add an environment variable to a Linux shell, you can use the export command.

Environment variables are key-value pairs that define various aspects of your shell environment, such as paths, settings, or custom values that programs can use.

Here's how you can add an environment variable to your shell:

## Temporary Environment Variable:
If you want to set an environment variable for your current shell session only, you can use the export command directly in the terminal. For example, to set a variable named MY_VARIABLE with the value my_value, you would run:

```
export MY_VARIABLE=my_value
```

This variable will only be available in the current terminal session. Once you close the terminal, the variable will be lost.

## Permanent Environment Variable (For a User):
To set an environment variable that will be available every time you log in, you'll typically want to add the variable to your shell's configuration file. The specific file depends on the shell you're using:

- For Bash: Add the export command to ~/.bashrc.
- For Zsh: Add the export command to ~/.zshrc.
- For Fish: Use set -Ux in ~/.config/fish/config.fish.
- For example, to set MY_VARIABLE as a permanent environment variable in Bash:

```
echo 'export MY_VARIABLE=my_value' >> ~/.bashrc
source ~/.bashrc
```

The source ~/.bashrc command reloads the Bash configuration, making the variable available in your current session.

## Permanent Environment Variable (For All Users):
If you want to set a global environment variable that affects all users on the system, you can typically add the variable to a system-wide configuration file. However, this usually requires administrative privileges (root access). The location of the file depends on the distribution and shell being used.
For example, you might add the export command to /etc/profile or /etc/environment.

Remember that after you've added or modified environment variables in a configuration file, you'll need to either start a new shell session or use the source command to apply the changes to your current session.

To check if an environment variable has been set, you can use the echo command followed by the variable name:

```
echo $MY_VARIABLE
```

This will print the value of the MY_VARIABLE environment variable if it has been set.
