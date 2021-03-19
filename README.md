# Jupyter on OzSTAR

A bash script to run Jupyter in a singularity container on OzSTAR, and tunnel in to connect.

If you don't have an account on the OzSTAR supercomputer, this isn't for you.

Usage:

- Clone this repo
- Make the script executable
- Run the script with relevant parameters and command, particularly `-n` or `--node` if you want to run the notebook on a dedicated job node, useful if you need lots of cycles or guaranteed GPU memory.
- Take a look at the help with `ozjup -h`

```git clone https://github.com/coljac/ozjup
chmod +x ozjup
./ozjup -h
```

Quickstart:

```
ozjup start
ozjup check
ozjup kill
```

**Note**: You'll need your ssh keys set up so you can ssh into ozstar without typing a password, and ssh from ozstar to ozstar as well.
