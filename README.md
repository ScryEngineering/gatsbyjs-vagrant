# gatsbyjs-vagrant
Vagrant setup for Gatsby.js development

Note that since this uses Apline linux as the box you may need to install
a plugin for Vagrant to get some commands such as `vagrant halt` to work.

```
vagrant plugin install vagrant-alpine
```


## Usage
When developing with the Gatsby development server you may need to specify the port to serve on as follows:

```
gatsby develop -H 0.0.0.0
```

Note you may need to use `sudo` to start the development server.
