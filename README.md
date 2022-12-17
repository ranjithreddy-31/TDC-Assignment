# Counting Primes using Message Passing Interface
<h3>Description</h3> In this assignment, I will try to establish inter process communication between them using Message Passing Interface(MPI). The expectation is to set up a running code which uses MPI to compute the primes in a range of numbers.
<h3>Header File</h3>mpi.h
<h3>Example Code</h3>:
    int main(int argc, char** argv){
        int process_Rank, size_Of_Cluster;

        MPI_Init(&argc, &argv);
        MPI_Comm_size(MPI_COMM_WORLD, &size_Of_Cluster);
        MPI_Comm_rank(MPI_COMM_WORLD, &process_Rank);

        printf("Hello World from process %d of %d\n", process_rank, size_Of_Cluster);

        MPI_Finalize();
        return 0;
    }
<h3>Required Commands</h3>:
To load MPI: apt install libopenmpi-dev
To open the file: nano file_name.c 
To compile the file: mpicc file_name.c -o <argument_to_intialize_mpi> (Ex: mpicc hello.c -o hellompi)
TO run the file: mpirun <argument_to_intialize_mpi> (Ex: mpirun hellompi)

<h3>Output</h3>:
 ![Alt text](/relative/path/to/img.jpg?raw=true "Optional Title")

