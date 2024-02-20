# From official apt!

```bash
apt download curl
dpkg -x curl** dir
```

# Nix package manager!!
They have done a very good work on precompiled binaries with even bleding edge packages! Let's download those binaries and use those. :-)
1. Install nix package manager
```bash
curl -L https://nixos.org/nix/install | sh
```
3. Install desired packages
```bash
nix-shell -p neofetch
```
5. Copy the installed packages to your desired location
```bash
cp /nix/store/3c6idwsrx95wbqfgha94b45cyr81ac1f-neofetch-unstable-2021-12-10/bin/neofetch ~/bin/
```
# Binaries
Precompiled binaries

# Compress to highest quality
```bash
hc(){
  tar cv $1 | xz -9 > $2.tar.xz
}
```

```bash
hc folder file
```

or,

```bash
tar cv path/to/data | xz -9 > file.tar.xz
```

# Decompress
```bash
tar -xf file.tar.xz
```

# Copy
Now, copy the bin in $HOME/.local/bin and 

copy the libs in $HOME/.local/lib (if exists or needs)

# .bash_profile
```bash
export PATH=$HOME/.local/bin:$PATH
export LD_LIBRARY_PATH=$HOME/.local/lib:$LD_LIBRARY_PATH
```
