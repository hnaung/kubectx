# kubectx(1)

kubectx is an utility to manage and switch between kubectl(1) contexts.

```
USAGE:
  kubectx                   : list the contexts
  kubectx <NAME>            : switch to context
  kubectx -                 : switch to the previous context
  kubectx <NEW_NAME>=<NAME> : create alias for context
  kubectx -h,--help         : show this message
```

Purpose of this project is to provide an utility and facilitate discussion
about how `kubectl` can manage contexts better.

## Example

```sh
$ kubectx minikube
Switched to context "minikube".

$ kubectx -
Switched to context "oregon".

$ kubectx -
Switched to context "minikube".

$ kubectx dublin=gke_ahmetb_europe-west1-b_dublin
Context "dublin" set.
Aliased "gke_ahmetb_europe-west1-b_dublin" as "dublin".
```

[Set up `bash` and `zsh` completion &rarr;](completion/README.md)

### Help wanted

- [ ] homebrew formula/tap that installs the script and completions

-----

Disclaimer: This is not an official Google product.
