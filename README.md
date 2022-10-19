# gsub
This is template that shows how to use gsub to write code with code.


```R
template = 'sbatch scenarioSCENERIONUMBER_runner.sh
'
sink(file = "jiachen_runner.R",append = TRUE)
for (i in seq(1,4860,1)){
  script = gsub(pattern = "SCENERIONUMBER", replacement = i, template)
  cat(script)
}
sink()
```
