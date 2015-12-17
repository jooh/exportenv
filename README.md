Package lists for deploying homebrew and conda to new machines.

# homebrew
Current list of brew packages for use with homebrew-bundle. The idea is to
`brew bundle dump --force` to update the Brewfile and `brew bundle` to
update the current brew environment with any new content from the Brewfile.

# conda
Do something like `conda env create -f environment.yml`. First, make sure
you have the right channels available by checking `conda config --get
channels`. You may have to do `conda config --add channels jcarlin` to get
things to build.

# limitations
Neither solution above has exact version control, For conda this is less of
a problem because the more sensitive packages are installed from my
anaconda repo, where versions will not change unnecessarily.
