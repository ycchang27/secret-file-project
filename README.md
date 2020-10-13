# git-secret guide for windows 10

# Prereqs
- git (must have bash)  
- MinGW

# Installing git
- https://git-scm.com/downloads

# MinGW (required to build git-secret)
- Get the latest installation manager here: https://osdn.net/projects/mingw/releases/
- Download the exe and execute the installation.

# Installing git-secret (MinGW required)
- In the installation location:
```
git clone https://github.com/sobolevn/git-secret.git git-secret
cd git-secret && make build
PREFIX="/usr/local" make install
```

# Installing gpg (required to use git-secret)
Follow the instructions mentioned here: http://www.ibiblio.org/shadow/pgp/install-gpg.pdf

# Validating the installation
- git-secret: `git-secret --version`
- gpg: `gpg --version`
