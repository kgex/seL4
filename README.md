Hello World Setup with seL4 Tutorials
1.1 Setup with seL4-Tutorials-Manifest and Environment
Create a directory for the tutorials:
bash
mkdir sel4-tutorials-manifest
cd sel4-tutorials-manifest

Initialize the repository:
bash
repo init -u https://github.com/seL4/sel4-tutorials-manifest
repo sync

Create a virtual Python environment:
bash
python3 -m venv venv

Activate the virtual environment:
bash
source venv/bin/activate

Install required packages:
bash
pip3 install setuptools
pip3 install sel4-deps
pip3 install camkes-deps

If only required, install additional packages:
bash
pip install aenum 
pip install sh

To deactivate the environment:
bash
deactivate

Initialize the Hello World tutorial:
bash
./init --tut hello-world
cd hello-world_build

1.2 Building Your First Program
Build the program using Ninja:
bash
ninja

Clean the build if necessary:
bash
ninja clean

Run the simulation:
bash
./simulate

Output:
text
Booting all finished, dropped to user space
Hello, World!

Terminate QEMU: Press Ctrl-A, then X.
