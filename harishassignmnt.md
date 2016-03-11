> source('~/Harish Assignment2.R')
> my_matrix <- makeCacheMatrix(matrix(c(5,8,9,11), 2, 2))
> my_matrix$get()
[,1] [,2]
[1,]    5    9
[2,]    8   11
> my_matrix$getInverse()
NULL
> cacheSolve(my_matrix)
[,1]       [,2]
[1,] -0.6470588  0.5294118
[2,]  0.4705882 -0.2941176
> cacheSolve(my_matrix)
getting cached data
[,1]       [,2]
[1,] -0.6470588  0.5294118
[2,]  0.4705882 -0.2941176
> my_matrix$getInverse()
[,1]       [,2]
[1,] -0.6470588  0.5294118
[2,]  0.4705882 -0.2941176
> my_matrix$set(matrix(c(2,5,8,3), 2, 2))
> my_matrix$get()
[,1] [,2]
[1,]    2    8
[2,]    5    3
> my_matrix$getInverse()
NULL
> NULL
NULL
> cacheSolve(my_matrix)
[,1]        [,2]
[1,] -0.08823529  0.23529412
[2,]  0.14705882 -0.05882353
> cacheSolve(my_matrix)
getting cached data
[,1]        [,2]
[1,] -0.08823529  0.23529412
[2,]  0.14705882 -0.05882353
> my_matrix$getInverse()
[,1]        [,2]
[1,] -0.08823529  0.23529412
[2,]  0.14705882 -0.05882353