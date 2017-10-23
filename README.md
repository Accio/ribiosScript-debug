The following commands works well:

```{bash correct}
## first optional, last required arguments
./myRscript.Rscript -infile test.file -opt1 A -opt2 B
```

```{bash correct}
## or first required, last optional arguments
./myRscript.Rscript  -opt1 A -opt2 B -infile test.file
```

In case the required arguments are given first, and unrecognised optional parameters are given, the program quits without printing any message

```{bash reqFirstError}
./myRscript.Rscript -infile test.file -opt1 A -opt3 B
```

In case the optional arguments are given first, errors are raised but the messages seem to make little sense now.

```{bash optFirstError}
./myRscript.Rscript -infile test.file -opt1 A -opt3 B
```
