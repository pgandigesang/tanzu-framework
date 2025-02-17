## tanzu package repository update

Update a package repository

```
tanzu package repository update REPOSITORY_NAME --url REPOSITORY_URL [flags]
```

### Examples

```

    # Update repository in default namespace 	
    tanzu package repository update repo --url projects-stg.registry.vmware.com/tkg/standard-repo:v1.0.1 --namespace test-ns
```

### Options

```
      --create                   Creates the package repository if it does not exist, optional
      --create-namespace         Create namespace if the target namespace does not exist, optional
  -h, --help                     help for update
      --poll-interval duration   Time interval between subsequent polls of package repository reconciliation status, optional (default 1s)
      --poll-timeout duration    Timeout value for polls of package repository reconciliation status, optional (default 15m0s)
      --url string               OCI registry url for package repository bundle
      --wait                     Wait for the package repository reconciliation to complete, optional. To disable wait, specify --wait=false (default true)
```

### Options inherited from parent commands

```
      --kubeconfig string   The path to the kubeconfig file, optional
  -n, --namespace string    Namespace for repository command, optional (default "default")
      --verbose int32       Number for the log level verbosity(0-9)
```

### SEE ALSO

* [tanzu package repository](tanzu_package_repository.md)	 - Repository operations

###### Auto generated by spf13/cobra on 14-Sep-2022
