---
description: Before diving in to create Data Products complete the
---

# Prerequisites

### Install CLI

The `dataos-ctl` CLI is your gateway to DataOS. You’ll use it to:

* Log in to the platform
* Initialize the environment
* Deploy or inspect your Data Product

Install `dataos-ctl` by following the installation guide for your operating system:

* [Install on Linux](https://dataos.info/interfaces/cli/installation/#installation-on-linux)
* [Install on macOS](https://dataos.info/interfaces/cli/installation/#installation-on-macos)
* [Install on Windows](https://dataos.info/interfaces/cli/installation/#installation-on-windows)

### Initialize CLI

After installation, open a terminal and run:

```
dataos-ctl init
```

Follow the prompts and provide inputs depending on your user role:

<details>

<summary>Prompts!</summary>

```bash
INFO[0000] The DataOS® is already initialized, do you want to add a new context? (Y,n)  
-> Y   # input the answer: Y or n

INFO[0255] 🚀 initialization...

INFO[0255] The DataOS® is not initialized, do you want to proceed with initialization? (Y,n)  
-> Y

INFO[0269] Please enter a name for the current DataOS® Context?  
-> {{name of the DataOS context}}
# Example: marmot (or any name you prefer).
# Your enterprise may offer multiple contexts — pick one to start.
# You can switch context anytime using a CLI command after login.

INFO[0383] Please enter the fully qualified domain name of the DataOS® instance?  
-> {{domain name}} 
# Example: apparent-marmot.dataos.app

INFO[0408] Entered DataOS®: marmot : apparent-marmot.dataos.app 

INFO[0429] Are you operating the DataOS®? (Y,n)         
-> n  
# If you are the operator (admin) for your enterprise, type Y.
# If you type Y, the installation steps will change.

INFO[0452] 🚀 initialization...complete
```

</details>

### Log in to [DataOS CLI](#user-content-fn-1)[^1]

Now, log in:

```bash
dataos-ctl login
```

Check if the setup is successful:

```
dataos-ctl version
dataos-ctl health
```

:tada:Now, you can use the CLI in your terminal to run different commands in DataOS.

### Set up IDE[^2]

[Set up an IDE, preferably VS Code. ](#user-content-fn-3)[^3]

* **Linux**: [Install VS Code on Linux](https://code.visualstudio.com/docs/setup/linux)
* **Windows**: [Install VS Code on Windows](https://code.visualstudio.com/docs/setup/windows)
* **macOS**: [Install VS Code on macOS](https://code.visualstudio.com/docs/setup/mac)

### Have the right access!

The Data Product creation requires the user to have the following tags or use cases:

`roles:id:data-dev`

`roles:id:sys-dev`

Check your tags by running the following command in your terminal:

```
dataos-ctl user get
```

Expected output:

```bash
            NAME      │       ID       │  TYPE  │          EMAIL          │              TAGS               
    ──────────────────┼────────────────┼────────┼─────────────────────────┼─────────────────────────────────
      Iamgroot        │ iamgroot       │ person │ iamgroot@tmdc.io        │ `roles:id:data-dev`,              
                      │                │        │                         │ `roles:id:system-dev`,            
                      │                │        │                         │ `roles:id:user`,                  
                      │                │        │                         │ `users:id:iamgroot`
```

To get the right tags, contact your DataOS Admin.

### Set up Workspace



###







[^1]: or DataOS CLI



[^2]: Can we not use other IDE, also why do we need to give the link even (if we want to make it more short)



[^3]: To create a data product, you must define it through a YAML file.
