# binaries
Precompiled binaries
# compress to highest quality 
tar cv path/to/data | xz -9 > file.tar.xz

# decompress
tar -xf file.tar.xz

# .bash_profile
export PATH=$HOME/.local/bin:$PATH
