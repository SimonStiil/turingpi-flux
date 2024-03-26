# Repository for flux configuration used on kubernetes cluster based on turingpi

Base directory is flux-base containing:
* flux-system responsible for flux, flux-base kustomization and helmrepositories
* kustomizations which are all kustomizations used.

## Order of application
Kustomizations are loaded in a dependency chain, this is due to the need to load CRDs before components 