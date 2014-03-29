
#PBS -l walltime=120:00:00,nodes=4:ppn=8

cd ~/Projects/drop2/

mpirun -np 32 -machinefile $PBS_NODEFILE interFoam -parallel | tee -a log