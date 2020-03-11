# azhpc

Devito MPI strong scaling POC using azhpc 

# Install Devito
```python
git clone https://github.com/devitocodes/devito.git
cd devito
python setup.py install
```

# Run benchmark
```python
DEVITO_ARCH=gcc DEVITO_MPI="full" DEVITO_OPENMP=1 DEVITO_LOGGING=DEBUG mpirun -n 1 python3 benchmarks/user/benchmark.py run -P viscoelastic -d 600 600 600 -t 100
```
