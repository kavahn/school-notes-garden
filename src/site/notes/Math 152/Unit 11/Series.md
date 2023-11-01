---
{"dg-publish":true,"permalink":"/math-152/unit-11/series/"}
---


# Unit X.x of [[Math 152/Math 152\|Math 152]]

# Series
- #### Suppose ${a_{n}}$ is a sequence of numbers. An expression of the form
	- $a_{1}+a_{2}+a_{3}\dots+a_{n}+\dots$
		- ###### is called an infinite series and it is denoted by 
			- $\sum^\infty$
- ### Definition
	- #### Given the series 
		- $\sum^\infty_{i=1}a_{i}=a_{1}+a_{2}+\dots$ let s_n denote its $n^{th}$ partial sum
			- if the sequence {sn} is convergent and $\lim_{ n \to \infty }s_{n}=s$ exists as a 0real number, then the series is convergent
				- ###### s is the sum of the series
- ### Infinite series and geometric
	- #### infinite $1+\frac{1}{2}+\frac{1}{4}+\dots$ has the partial sums $s_{1}=1,s_{2}=1.5,s_{3}=1.75\dots$
		- and in general it turns out that $s_{n}=2-\frac{1}{2^{n-1}}$
	- #### Geometric. show that the geometric series $\sum^\infty_{i=1}ar^{i-1}=a+ar+ar^2+\dots$is convergent if $|r|<1$and its sum is 
		- $\sum^{\infty_{i=1}ar^{i-1}}=\frac{a}{1-r},|r|<1$
			- if |r| is $\geq$ the series is divergent *a=1*
				- $\sum^{n}_{i=1}r^{i-1}=r\sum^n_{i=1}r^{i-1}+1-r^n$
					- $(1-r)s_{n}=1-r^n$ (assuming that r=/=1)
						- => $s_{n}=\frac{{1-r^{n}}}{1-r}$ $\lim_{ n \to \infty }s_{n}=\frac{1}{1-r}$
			- if a is a coefficient we can rewrite it as 
				- $a\sum$
- ### Examples. 
	- #### Ex 1. Determine whether that the given series converges or diverges
		- ###### a. $\sum^\infty_{n=1}(\frac{e}{10})^n$ 
			- => $\sum^\infty_{n=1}{\frac{e}{10}\left( \frac{e}{10} \right)^{n-1}}$ => 
	- #### Ex 2. write 0.55555555... as a rational number
		- 0.55555...= $\frac{5}{10}+\frac{5}{100}+\frac{5}{1000}+\dots$
			- => $\sum^\infty_{1=1}5\left( \frac{1}{10} \right)^i\implies \sum^\infty_{i=1}{\frac{5}{10}\left( \frac{1}{10} \right)^{i-1}}$ 
				- $r=\frac{1}{10},a=\frac{5}{10}$
					- => $\frac{5}{9}$
	- #### Ex 3. show that the series $\sum^\infty_{n=1}{\frac{1}{(n+1))(n+2)}}$
		- => $\frac{1}{6}+\frac{1}{12}+\frac{1}{20}+\dots$
			- ###### This is ugly and doesnt have any nice patterns so we can do partial fraction decomposition
				- => $\frac{1}{(n+1)(n+2)}=\frac{1}{n+1}-\frac{1}{n+2}$
					- $S_{k}=\sum^k_{n=1}{\frac{1}{(n+1)(n+2)}}=\sum^k_{n=1}{\frac{1}{n+1}}-{\frac{1}{n+2}}=\frac{1}{2}-\frac{1}{3}+\frac{1}{3}-\frac{1}{4}+\frac{1}{4}-\dots{-\frac{1}{k+2}}$
						- = $\frac{1}{2}-\frac{1}{k+2}$
							- => $\lim_{ k \to \infty }S_{k}=\frac{1}{2}$
	- #### Ex 4. Show that the harmonic series is divergent
		- $\sum^\infty_{n=1}{\frac{1}{n}}=1+\frac{1}{2}+\frac{1}{3}+\dots$
			- $1+\frac{1}{2}+\frac{1}{3}+\frac{1}{4}+\frac{1}{5}+\frac{1}{6}$
			- we can group it so that 
				- $a_{2^{n}+1}+\dots a_{2^{n+1}}\geq \frac{1}{2^{n+1}}2^{n}=\frac{1}{2}$
					- $S_{2^{n+1}}\geq \frac{1}{2}(n+1)\implies diverges$