# Installation instructions:

1. You can get the latest version from [the Releases page](https://t.me/turkernelwsl2releases).

2. Place the downloaded kernel in the folder named 'Linux' under the user directory. (e.g., `C:\Users\onurb\Linux\bzImage`)(To find your username, you can find your username by opening the cmd or PowerShell application and typing 'query user'.).

3. Create a configuration file under the user folder with any editor, name '.wslconfig' and prepare your configuration as written below:

It should look something like:

```
[wsl2]
kernel = C:\\Users\\'Your Username'\\Linux\\bzImage
```

4. Save this file as `.wslconfig` in the current user's home directory (e.g. `C:\Users\'Your Username'\.wslconfig`).

5. Restart WSL with `wsl.exe --shutdown` and check that the new image has been booted with `uname -r`.

Note: I don't have an instant updater right now. I will add if I can do it in the future.

Note 2: I'll keep the kernel up to date as soon as I can.

Warning: This Kernel is not for ARM base. I'm doing it for x86. Since I don't have an ARM-based device, I don't get a compilation.