# DaskIt

A repo of dockerfiles to create a container with a dask scheduler and a dask worker.

## Instructions
- _run docker build . -t dask-scheduler_ in scheduler directory.
- start scheduler with _docker run -p 8787:8787 dask-scheduler_
- in a new terminal, run _docker build . -t worker_ in the worker directory
- Run the worker container with _docker run --name=worker worker_
