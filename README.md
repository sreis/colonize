# colonize

Script to manage Terraform and DC/OS deployments.

*NOTE*: Currently only supports GCP.

## Install

Default config directory is `~/.config/colonize`. To change the defaults edit `colonize` and change `${CONFIGDIR}`.

Add `colonize` to your $PATH.

```bash
chmod +x colonize && cp colonize /usr/local/bin/
```

## Instructions

Edit file `${CONFIGDIR}/config` to setup your GCP credentials.

### Create a Terraform deployment 

``` colonize gcp ```

### List Terraform deployments 

``` colonize list ```

### Destroy Terraform deployment

``` colonize destroy <colony id> ```

### Create SSH to Kubernetes API server running on DC/OS

``` colonize tunnel [<colony id>] ```
