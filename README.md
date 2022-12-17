# Counting Primes using Message Passing Interface
<h3>Description</h3> 
    In this assignment, I will try to establish inter process communication between them using Message Passing Interface(MPI). The expectation is to set up a running       code which uses MPI to compute the primes in a range of numbers.
<h3>Header File</h3>mpi.h
<h3>Example Code</h3>

    # include <mpi.h>
    # include <stdio.h>
    int main(int argc, char** argv){
        int process_Rank, size_Of_Cluster;

        MPI_Init(&argc, &argv);
        MPI_Comm_size(MPI_COMM_WORLD, &size_Of_Cluster);
        MPI_Comm_rank(MPI_COMM_WORLD, &process_Rank);

        printf("Hello World from process %d of %d\n", process_rank, size_Of_Cluster);

        MPI_Finalize();
        return 0;
    }
<h3>Required Commands</h3>
    <li>To load MPI</li> apt install libopenmpi-dev
    <li>To open the file</li> nano file_name.c 
    <li>To compile the file</li> mpicc file_name.c -o <argument_to_intialize_mpi> (Ex: mpicc hello.c -o hellompi)
    <li>TO run the file</li> mpirun <argument_to_intialize_mpi> (Ex: mpirun hellompi)

<h3>Output</h3>

 ![mpi](/images/mpi.jpg)


