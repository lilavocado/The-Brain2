- Reid, Cade
- V00862222
- STAT 255 R Assignment 2
- Instructor: Dr. Fan Wu

## Part 1


```R
## P(X = 12)
dpois(12, lambda = 14)
```


0.0984184945069073



```R
## P(X <= 15)
ppois(15, lambda = 14)
```


0.66935991756252



```R
## P(10<=X<=14)
ppois(14, lambda = 14) - ppois(10, lambda = 14)
```


0.394755499945287


## Part 2


```R
## Creating vecotor with 9000 observations from X ~ Bin(50, 0.4)
simulation.data <- rbinom(9000,size = 50, prob = 0.4)
```


```R
## Generating histogram
hist(simulation.data)
```


![png](output_7_0.png)


The shape of the distribution is approximately the shape of a normal distribution. By the central limit theorem, as the number of observation approaches inifinity, the approximate pdf will approach to a normal distribtuion function.


```R
mean(simulation.data)
```


19.9731111111111


Population mean: E[x] = n*p = 50*0.4 = 20

Difference between population mean and sample mean = 20 - 19.9731 = 0.0269

## Part 3


```R
## Generating 5 random numbers from [1,200]
sample(c(1:200), size = 5, replace = FALSE)
```


<ol class=list-inline>
	<li>146</li>
	<li>69</li>
	<li>52</li>
	<li>42</li>
	<li>153</li>
</ol>




```R
sample.heights <- c(172.7, 176.5, 165.7, 173.3, 172.5)
```


```R
mean(sample.heights)
```


172.14



```R
var(sample.heights)
```


15.568



```R

```
