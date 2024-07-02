
# Enable CentOS 7 Repos after it went EOL

> ⚠️ WARNING: Don't use it in production

CentOS 7 went EOL on 30th June 2024.

This means that all CentOS 7 repositories will be shut down and moved to vault.centos.org.

Some people (not businesses) still want to use the old repositories (which are present in vault) to install packages using yum.

> ⚠️ WARNING: packages being present in vault doesn't mean that they are secure. It is just an archive of the last state(s) of the packages. Don't use it in production

If you want to enable the repositories all you have to do is to run this command:

```bash
sudo curl https://raw.githubusercontent.com/sdhmh/enable-centos-7-repo/main/CentOS-Base.repo --output /etc/yum.repos.d/CentOS-Base.repo
```

