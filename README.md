## WHAT
Practice using [kubebuilder](https://book.kubebuilder.io/) to implement k8s operator

## Steps
```bash
## Bootstrap
kubebuilder init --domain extend-k8s.io

kubebuilder create api --group operator --version v1 --kind TimeseriesDB
# Create Resource [y/n]
# y
# Create Controller [y/n]
# y

# Run make command to generate clients and sample files with the updated TimeseriesDB resource
make

# Install the CRD to the cluster and run the controller
make install run
```
