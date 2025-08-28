
### Helm pack

```
helm package <chart_path>

eg.
helm package .
```


### Github registey
```s
//assign value
$ export HELM_PAT=<token>

//authen
$ echo $HELM_PAT | docker login ghcr.io -u <github_account_name> --password-stdin

eg.
echo $HELM_CHART_PAT | docker login ghcr.io -u supanut741355 --password-stdin
```

### Helm push

```
$ helm push <chart_zip_file> oci//ghcr.io/<github_account_name>/<github_repo_name>

eg.
$ helm push omegared-0.1.0.tgz oci://ghcr.io/supanut741355/dev_space
```