# From official apt!
apt-get download curl

dpkg -x curl* dir

# Binaries
Precompiled binaries

# Compress to highest quality
```bash
hc (){
  tar cv $1 | xz -9 > $2.tar.xz
 }
 ```

hc folder file

or,

tar cv path/to/data | xz -9 > file.tar.xz

# Decompress
tar -xf file.tar.xz

# Copy
Now, copy the bin in $HOME/.local/bin and 

copy the libs in $HOME/.local/lib (if exists or needs)

# .bash_profile
export PATH=$HOME/.local/bin:$PATH

export LD_LIBRARY_PATH=$HOME/.local/lib:$LD_LIBRARY_PATH
