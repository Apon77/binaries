# binaries
Precompiled binaries

# compress to highest quality 
hc () 
{ 
    tar cv $1 | xz -9 > $2.tar.xz
}

hc folder file

or,
tar cv path/to/data | xz -9 > file.tar.xz

# decompress
tar -xf file.tar.xz

# .bash_profile
export PATH=$HOME/.local/bin:$PATH
