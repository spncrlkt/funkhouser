# Install step notes

           _____
           |_ _|
      n    (O O)    n
      H   _|\_/|_   H
     nHnn/ \___/ \nnHn
    <V VV /     \ VV V>
     \__\/|     |\/__/

	     EAT SHIT


install vagrant and virtualbox
https://docs.vagrantup.com/v2/getting-started/project_setup.html
run hashicorp/precise32 box

	brew install ansible

update vagrantfile to use ansible provisioner
http://docs.ansible.com/ansible/guide_vagrant.html

built a small playbook to test ansible provisioning which installs
nodejs and npm

If so inclined, at this point, you could dig into containerizing the
different subcomponents (front-end, API, db/persistence layer) using
something like Docker. But I don't want to do that, yet.


Next steps:
write ansible playbook to install the following on the guest system:

1. front-end toolchain
2. API toolchain
3. DB


## Front-end toolchain
https://github.com/omniscientjs/omniscient-starter-pack
basically set up a package.json, and some hot-loader shit from the
starter pack, webserver 2

## TMUXer MFer
install tmux, so the webserver (and api, and db, eventually) can be 
run in a persistent tmux session... still working on this
also working on moving .bash_profile into ~/.bash_profile
moved tmuxinator.bash into ~/.bin for completion
make 'mux start dev' run on login
