# Jupyter on OzSTAR

A bash script to run Jupyter in a singularity container on OzSTAR, and tunnel in to connect.

If you don't have an account on the OzSTAR supercomputer, this isn't for you.

Usage:

- Clone this repo
- Make the script executable
- Run the script with relevant parameters, most crucial being `-u ozstar_username` and `-n` if you want to run the notebook on a dedicated node, useful if you need lots of cycles or guaranteed GPU memory.
- Take a look at the help with `ozjup -h`

```git clone https://github.com/coljac/ozjup
chmod +x ozjup
./ozjup -h
```

**Note**: You'll need your ssh keys set up so you can ssh into ozstar without typing a password, and ssh from ozstar to ozstar as well.

If you set the environnment variable `OZSTAR_USERNAME` on your local machine, you can skip the `-u` flag.
