# git-secret guide for windows 10

# Prereqs
- git (must have bash)  
- MinGW

# Installing git
- https://git-scm.com/downloads

# MinGW (required to build git-secret)
- Get the latest installation manager here: https://osdn.net/projects/mingw/releases/
- Download the exe and execute the installation.

# Installing gpg (required to use git-secret)
- Reference: http://www.ibiblio.org/shadow/pgp/install-gpg.pdf
- Go to https://www.gnupg.org/(en)/download/index.html and download Tarball from `GnuPG` at `Source code releases` section.
- To extract tar file, go to that location and execute (via git bash) `tar -xvf <tar file name>
- Move that extracted folder to installation location. Then set that PATH as environment variable
```
For example, if your PATH variable reads as c:\windows;c:\utils
then change it to c:\windows;c:\utils;c:\gnupg
 ```

# Installing git-secret (MinGW required)
- In the installation location, execute the following commands (https://git-secret.io/installation):
```
git clone https://github.com/sobolevn/git-secret.git git-secret
cd git-secret && make build
PREFIX="/usr/local" make install
```

# Validating the installation
- git-secret: `git-secret --version`
- gpg: `gpg --version`

# Troubleshooting
- Installation is successful, but bash or shell doesn't pick up `[program]`
  - Make sure that the installation path are saved to PATH environment variable

# How to use git-secret
- Follow instructions given by git-secret: https://git-secret.io/
- Or youtube: https://www.youtube.com/watch?v=zyev7RPqi5o
