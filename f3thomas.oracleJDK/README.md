# Role Name

I needed a role that did install the oracle JDK 8 on Ubuntu Xenial
NOTE: This is just for Ubuntu 

To install,

    sudo ansible-galaxy install f3thomas.oracleJDK

## Role Variables

Variables and defaults follow.

java_version  ... must be one of [6,7,8,9] 


## Dependencies

No dependencies on other roles.

IMPORTANT: Using this role implies that you have accepted the Oracle license agreement to download the Oracle JDK and JCE. If you don't agree, don't use this role please.

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      become: yes
      become_user: root
      vars:
        -java_version: 8
      
      roles:
        - role: f3thomas.oracleJDK


## License

MIT

