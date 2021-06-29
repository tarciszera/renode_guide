# Renode startup guide

Renode is a tool for hardware(HW) simulation. HW can be described on .repl files,
such as peripheral properties, mem space and pins linkage.

## Dependencies for Ubuntu 20.04 LTS

```sh
sudo apt install mono-complete

sudo apt-get install policykit-1 libgtk2.0-0 screen uml-utilities gtk-sharp2 libc6-dev gcc python3 python3-pip
```

## Instalation

The instalation of renode could be done by
 [git rep.](https://github.com/renode/renode/releases/tag/v1.12.0), compilation
 and instalation:

 ```sh
 git clone https://github.com/renode/renode

 cd renode
 ./build.sh -v
 ```

Or by precompiled .deb package download from [here](https://renode.io/#downloads), then installing by apt:

 ```sh
 # Easiest way!
 sudo apt install /path/to/package.deb
 ```

## Plataforms

In renode environment there's those .repl files used to describe hardware architecture, such as special properties, memory allocation and linkage with other parts of hardware. Generaly it's described as peripherals, [here](https://renode.readthedocs.io/en/latest/advanced/platform_description_format.html) there is an explanation on the systax.

Renode have some chips and boards implemented already, though it's possible to describe your own hardware, [here](https://renode.readthedocs.io/en/latest/advanced/writing-peripherals.html) there's a guide to describe custom peripherals.

## Usage

When you run:
```sh
# Must be on PATH
renode
```
A terminal like GUI is open, and it seems like this:

![](./img/renode_gui.png)

There machines could be created, runned and dellete. For more information please reffere to [this](https://renode.readthedocs.io/en/latest/introduction/using.html). You also can run your first `demo`, what is decribed [here](https://renode.readthedocs.io/en/latest/introduction/demo.html).
