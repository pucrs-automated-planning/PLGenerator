# PLGenerator

PLGenerator.jar - (Plan Library Generator) is program to automatically generate arbitrarily complex plan libraries. 

## Running PLGenerator

```bash
java -jar PLGenerator.jar [OPTION]... 
```

### Command-line Parameters
- -h 	 display this help and exit  
- -g 	 number of top plans (goals), (default: 3)  
- -d 	 depth of the plan tree, (default: 4)  
- -b 	 minimum number of branches that all nodes must have, (default: 1)  
- -B 	 maximum number of branches that all nodes may have, (default: 3), this value must be greater than or equal to the minimum number of branches (-b) 
- -f 	 number of features associated with each plan node, (default: 1) 
- -c 	 number of values that may be associated with the features, (default: 2) 
- -F 	 number of features available to be associated with plan nodes, (default: 10) 
- -s 	 probability [0,1] of create a sequential branch, (default: 0.8) 
- -D  percentage [0,1] of duplicated top-plans (goals) in order to generate ambiguous paths, (default: 0) 
- -t 	 minimum number of times that an observation of a plan step must be repeated (default: 1) 
- -T 	 maximum number of times that an observation of a plan step must be repeated (default: 1) 
- -A 	 receives ALL parameters in the following order: g, d, b, B, f, c, F, s, D, t, T, p (e.g., java -jar PLGenerator.jar -A 3 4 1 3 1 2 10 0.8 0 1 1 plan_library.xml) 
- -p 	 output file path to save the plan library, (default: plan_library.xml)  

A more thorough manual is available in [PDF form at this repository](README.pdf).

## Authors

This software was written by Giovani P. Farias. (giovanifarias@gmail.com), under supervision of [Felipe Meneguzzi](https://github.com/meneguzzi) and [Rafael Bordini](https://github.com/rbordini), with the [Lab on Autonomous Systems](https://github.com/lsa-pucrs). 
The plan library format was originally developed by [Felipe Meneguzzi](https://github.com/meneguzzi), so this project uses a substantial code-base from @meneguzzi. 

