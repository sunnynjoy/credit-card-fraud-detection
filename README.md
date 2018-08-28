## Find similarity between between 2 rows

Sample (S) 100 transactions from whole data (D), for every transaction in S, print 10 transactions from D which have least values of 'similarity'
the similarity between any two vectors is defined as
## similarity(vi,vj) = cosine^-1(dot product (vi, vj) / (length(vi) * length(vj)) )

1. vi represents a vector i.e. a row in our data.
2. similarity(i,j) is just a function we can think it like f(x,y)
3. length(vi): length of the vector vi
4. dot product(i,j) is the dot product between the vectors vi, vj

Note: the sample contains at least two transactions of minority class 

## ex: 
Sample S = {1, 34, 989, 1000}

given transaction id = 1 , class = 1
-------------------
similar transactions
-------------------
class = 1 # similarity = 0.00 # transaction id = 1
class = 1 # similarity = 0.0023 # transaction id = 0
class = 1 # similarity = 0.02312 # transaction id = 89
class = 1 # similarity = 0.02498 # transaction id = 2034
...
--------------------------------------------------------
given transaction id = 34, class = 0
-------------------
similar transactions
-------------------
class = 0 # similarity = 0.00 # transaction id = 34
class = 0 # similarity = 1.005 # transaction id = 523212
class = 1 # similarity = 1. 2673 # transaction id = 500001
class = 1 # similarity = 1. 3459 # transaction id = 24
