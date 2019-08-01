# BigData-AzureTest

The R script generates 1000 random numbers from 0 to 100 and computes the standard deviation and variance.

The R script was executed using a free trial of Microsoft Azure.
First I created a databrick and its associated resource group. Inside that databrick, I created and started a cluster. Then I created a new notebook and wrote the R code in the cells. The first cell defines the function that generates the random numbers and computes the standard deviation and variance. The second cell calls that function. I then attached the notebook to the cluster I made and ran all the cells. When I ran the code, I got a standard deviation of 29.342 and a variance of 860.953.

One of the issues I encountered while getting the R script to run was that my cluster kept terminating because it exceeded the quota for the number of cores I could use. At first, I thought I was getting the error due to a bug in the R code, but when I tried running the cluster without the notebook, it still failed to start. I looked into the cluster configurations more closely and eventually figured out how to reduce the number of cores it required to run.

The repository contains screenshots of the cluster's configuration and the results of executing the R script.
