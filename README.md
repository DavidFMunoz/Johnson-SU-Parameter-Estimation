# Johnson-SU-Parameter-Estimation
This project is asssociated to the article "Comparison of Five Estimation Methods for the Parameters of the Johnson Unbounded Distribution using Simulated and Real-Data Samples"
that has been submitted for possible publication to the journal Computational Statistics.

The main produces a random sample of size N1 from a Johnson-SU distribution with four parameters: MuN, StDevN, Shift, Mult 
that has the form of 
                    
                    X = Shift + Mult * sinh(Y)
where Y denotes a random variable that has a normal distribution with mean MuN and standard deviation StDevN.

The four parameters of the Johnson-SU distribution are estimated using the Minimum Cramér-von Mises Distance method and then reported along with statistics of goodness-of-fit such as 
the Kolgomorov-Smirnov statistics, the Cramér-von Mises distance and the logarithm of the likelihood funtion.

Input Data for the main program is in the file SimData1.txt that has the followig values:

N0

N1

MuN

StDevN

Shift 

Mult 

where N0 and N1 are integers with N0 >= 0 and N1 > 2.  MuN, StDevN, Shift, Mult are real numbers with  StDevN > 0.

The value of N0 is the number of samples of size N1 that are generated (and discarded) before producing the random sample that will be used to estimate the parameters of the Johnson-SU distribution.

In file Main.cpp there is also a (commented) main to estimate the four parameters using the method of Maximum Likelihood. 
The code in this Main can be easily modified to estimate the parameteres of a Johnson Unbounded Distribution from an arbitrary sample of n > 2 observations.
