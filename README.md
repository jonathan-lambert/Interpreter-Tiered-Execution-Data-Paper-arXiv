# Interpreter-Tiered-Execution-Data-Paper-arXiv
This repository details the dataset that was built from an analysis of the runtime behaviour of the OpenJDK JRE version 9 through to 14 and used within the arXiv preprint paper: Repositioning Tiered Hotspot Execution Performance Relative to the Interpreter.

The file details and lists the observations associated with a number of variables:

jvm: the OpenJDK JRE version - 
    9 through 14
    
gcc: the GNU GCC compiler collection version used in the building of the OpenJDK JRE versions - 
    5 through 8
    
gc: the garbage collector invoked at runtime - 
    SGC serial collector, 
    CGC concurrent mark and sweep collector, 
    CPGC the concurrent mark and sweep collector with parallel collection of the new object heap
    PGC the paralell collector
    G1GC the garbage first collector
    
benchmark: one of the 24 Renaissance Benchmark application workloads
    akka-uct, chi-square, db-shootout, dec-tree,     
    dotty, finagle-chirper, finagle-http, fj-kmeans,     
    future-genetic, gauss-mix, log-regression, mnemonics,       
    movie-lens, naive-bayes, neo4j-analytics, page-rank,      
    par-mnemonics, philosophers, reactors, rx-scrabble,   
    scala-doku, scala-kmeans, scala-stm-bench7, scrabble.

category: a categorisation of the benchmark workloads
    apache, concurrency, database, functional, scala, web.

rtINT: the execution time in interpreter mode

rtHS: the execution time in tiered execution mode

ratio: the ratio of interpretive to teired execution


