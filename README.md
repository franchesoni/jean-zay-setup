# jean-zay-setup

## setup steps:
- ensure $WORK, $SCRATCH, $HOME, and $STORE are clean (except for .ssh and git configs)
- from $HOME run `ln -s "$WORK" work`
- now `cd work`, `ln -s "$STORE" store`, `ln -s "$SCRATCH" scratch`, `ln -s "$DSDIR" dsdir`, `mkdir repos`
- from $WORK, `mkdir .local`, `ln -s .local $HOME` (this will avoid blowing up the space in $HOME, $WORK has a little bit more)
- add to .bashrc `alias pinstall='pip install --user --no-cache-dir'` 

## rules:
- never work in $HOME, only in $WORK (which is $HOME/work )
- if possible work in $HOME/work/scratch , which is temporary but SSD
- load your module (usually the last pytorch), for instance `module load arch/h100` `module load pytorch-gpu/py3/2.6.0` and `pinstall` other packages if needed

## utils:
- use a machine interactively
- consult quota: `idr_quota_user`

