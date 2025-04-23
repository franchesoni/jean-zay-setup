# jean-zay-setup

## setup steps:
- ensure $WORK, $SCRATCH, $HOME, and $STORE are clean
- from $HOME run `ln -s "$WORK" work`
- now `cd work`, `ln -s "$STORE" store`, `ln -s "$SCRATCH" scratch`, `ln -s "$DSDIR" dsdir`, `mkdir repos`

## rules:
- never work in $HOME, only in $WORK (which is $HOME/work )


