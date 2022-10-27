# CFEngine policy example - SSH management

This is an example project for showing how you could get started with managing SSH keys with CFEngine, to grant and revoke SSH access.

The main policy file is in [./ssh_management/ssh_management.cf](./ssh_management/ssh_management.cf).

This is a CFEngine Build project and if you would like to run / test it, we strongly recommend that you do this in a virtual machine (VM).
If you haven't done this before, [see our getting started tutorials](https://docs.cfengine.com/docs/master/getting-started.html).

You can clone it and run `cfbs` / `cf-remote` commands inside the repo, just like in the getting started tutorials:

```
git clone https://github.com/olehermanse/cfengine-example-ssh-management.git
cd cfengine-example-ssh-management
cfbs build
```

and so on...

**Warning:** If you start experimenting with SSH config and access like this, do it in a VM which is easy for you to throw away / recreate.
If you are not careful, it is easy to lock yourself out.
When moving on to doing this in production, ensure you have another way to fix issues if you accidentally lock yourself out.
This can be achieved by deploying policy with git, for example [using CFEngine Build in Mission Portal](https://cfengine.com/videos/?videoID=kkmBdJW8HcM).
