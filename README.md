# Hello World Tutorial Setup with seL4-tutorials-manifest

## 1.1 Setup with seL4-tutorials-manifest and Virtual Environment

### Setup:

- Create a new directory for the tutorial manifest:

  ```bash
  mkdir sel4-tutorials-manifest
  cd sel4-tutorials-manifest
  ```

- Initialize and sync the repository:

```bash
repo init -u https://github.com/seL4/sel4-tutorials-manifest
repo sync
```

### you should see something like this 👀 👀 👀 
=======
- Create a virtual Python environment and activate the environment 

```bash
python3 -m venv venv
source venv/bin/activate

```

### Dependencies:

- Install setuptools

```bash
pip3 install setuptools
```

- Install seL4 dependencies

```bash
pip3 install sel4-deps
```

- Install CAmkES dependencies

```bash
pip3 install camkes-deps
```

- If only required, install additional packages:

```bash
pip install aenum
pip install sh
```

## 1.2 Building Your First Program

- Build the project using ninja:

```bash
./init --tut hello-world
```

- Navigate to the build directory:

```bash
cd hello-world_build
```

- Build the project using ninja:

```bash
ninja
```

- Clean the build using ninja:

```bash
ninja clean
```

- Simulate the program:

```bash
ninja clean
```
<img width="821" alt="Screenshot 2024-09-25 at 16 18 55" src="https://github.com/user-attachments/assets/04d420b4-217e-46e9-bc73-d04dc3a0f39f">
