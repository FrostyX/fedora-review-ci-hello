# Running fedora-review on every commit

This is a fake Fedora DistGit repository for the `light` package.

https://src.fedoraproject.org/rpms/light

Of course, I wanted to use the `hello` package for this example but the GNU
website is having a prolonged outage causing:

```
| WARNING: Cannot download url: https://ftp.gnu.org/gnu/hello/hello-2.12.2.tar.gz
| WARNING: Cannot download url: https://ftp.gnu.org/gnu/hello/hello-2.12.2.tar.gz.sig
| WARNING: Cannot download url: https://ftp.gnu.org/gnu/gnu-keyring.gpg
```

So we are temporarily using `light` for the example.


## Run workflows locally

You can easily run the workflow locally with:

```
sudo dnf install act-cli
act -W .github/workflows/
```

Or just push the code and trigger the CI on GitHub
