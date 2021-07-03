## Execute makeCacheMatrix() e cacheSolve()

source("D:/data_science/R/coursera/r_programming/ProgrammingAssignment2/cachematrix.R")

matFunc <- function(n) { i <- 1:n; 1 / outer(i - 1, i, "+") }
mat <- matFunc(6)
cacFunc <- makeCacheMatrix(mat)
cacheSolve(cacFunc)