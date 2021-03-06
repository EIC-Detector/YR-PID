# Yellow Report PID Performance Evaluation

The codes presented here are not officially sanctioned code.

Nonetheless, for PID, there will be a requirement that all detector technologies
shall present performance plots via code so that an apples-to-apples comparison
is possible.

This example will allow groups to get started immediately with code that would require
minimal future updates when an official formulation becomes available.  The code here is how you 
REPORT the fundings of your simulations...not how you acquire them.

Here is how to run this simple example:

```
[me@computer] root -l
root [0] .x RUNME.C
```

If you want to develop your own detector, it is basically like this:

1.  `Copy tofBarrel.h <yourThing>.h`
2.  `Copy tofBarrel.C <yourthing>.C`
3.  Edit these files to make them correct:
    - search and replace tofBarrel with <yourThing>  
    - change every routine until to gives answers for your detector technology.
4.  A few requests to help your colleagues:
    - use variable names that are meaningful (particularly in the constructor).  
    - put reasonable default values for all arguments in the constructor.
    - If there is some critical value (tof res, index of refraction) put this in the name string.
    - comments in the code can include:
      - comments to help understand how it is coded.
      - comments to summarize assumptions in the present version.
      - comments to reference source of information
