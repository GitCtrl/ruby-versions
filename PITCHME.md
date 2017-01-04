#HSLIDE
### R
### OpenCPU Spark Executor

<span style="color:gray">An Apache Spark Package</span>

#HSLIDE

### ROSE Apache Spark Package
   
   - Offers the full scientific computing of the R programming language
   - Within Spark and streaming apps on the JVM

#VSLIDE

### OCPUTask

<span style="color:gray">An executable object that represents an R function call.</span>

'''scala

// Define executable for R starts#rnorm function call.
OCPUTask task = OCPU.R().pkg("stats").function("rnorom").input(params.asJava).library()