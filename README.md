## INFO 550 Project 

It is a very basic R program for my project
I used library of 'tidyr','tidyverse' and 'data.table'. The required packages can be installed using R commands.


```{r}
installed_pkgs <- row.names(installed.packages())
pkgs <- c("tidyr", "tidyverse","data.table")
for(p in pkgs){
	if(!(p %in% install_pkgs)){
		install.packages(p)
	}
}

```

My project is about linking some birth records with air pollution quality data. I also calculate their trimester averages and present them in table and plot format.

The birth record is the file 'simulated_final' and 'NH4' is my air pollution data.

## Execute the analysis

To execute the analysis, from the project folder you can run 

```{r}
Rscript -e "rmarkdown::render('HW4_YX.Rmd')"

```
This will create a file called HW4_YX.html output in your directory that contains the results.