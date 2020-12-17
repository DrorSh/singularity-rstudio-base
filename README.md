Based on https://github.com/granek/singularity-rstudio-base

Changed CRAN repository to timestamped version (2020-12-15)


# Build

```
singularity build --fakeroot rstudio.sif Singularity.4.0.3
```

# Run

```
mkdir mytmp myrun
singularity run --home /home/drorsh/dev/RStudio:/home/drorsh --bind mytmp:/tmp --bind myrun:/run --bind /home/drorsh/Projects:/home/drorsh/Projects rstudio.sif 
```
