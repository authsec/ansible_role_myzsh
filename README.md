Role Name
=========

Installs a basic shell environment (zsh with tmux). Configuration  works with the pragmata pro font.

Requirements
------------

The role will install tmux, zsh and zplug at least. It will then pull other plug-ins as specified with zplug.

Role Variables
--------------

Most important

```
  riv_myzsh_username: Your username in the shell
```

These parameters can be set, but will be derived.

```
  riv_myzsh_groupname: "{{ riv_myzsh_username }}"
  riv_myzsh_userhome: "/home/{{ riv_myzsh_username }}"
```

Dependencies
------------

-

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

  - hosts: servers
    become: true
    roles:
      - authsec.myzsh

License
-------

MIT

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
