
# Setup a jupiter environment
https://zero-to-jupyterhub.readthedocs.io/en/latest/jupyterhub/installation.html

# Resources assignment MiniKube
minikube delete && minikube start --cpus 4 --memory 8192

# To initialise loadbalancer within MiniKube
minikube tunnel 

# Install a new release of jupiter
helm upgrade --cleanup-on-fail \
  --install solid-peahen . \
  --namespace jupyter \
  --version=1.0.0

