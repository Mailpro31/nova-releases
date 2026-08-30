# Nova Releases

Public, non-secret metadata for Nova release distribution.

`releases.novaspeak.app` serves signed manifests from this project. Large OCI
artifacts are built from their source repositories and referenced immutably by
digest. Customer machines never need Git, GitHub authentication, a registry
login or access to a private repository.

Private signing keys are deliberately absent. Release manifests are generated
and signed by the protected `organization-lab-release` GitHub environment in
`nova-server` and deployed directly to this Vercel project.
