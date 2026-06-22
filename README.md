# pg18-ansible
postgres + ansible

```mermaid
ansible-postgresql/
├── ansible.cfg
├── inventory/
│   └── production
├── group_vars/
│   └── all/
│       └── vars.yml
│   └── pg_classe_pequena/
│       └── vars.yml
│   └── pg_classe_media/
│       └── vars.yml
│   └── pg_classe_grande/
│       └── vars.yml
├── roles/
│   └── postgresql/
│       ├── tasks/
│       │   ├── main.yml
│       │   ├── install.yml
│       │   ├── configure.yml
│       │   └── init.yml
│       ├── templates/
│       │   ├── postgresql.conf.j2
│       │   └── pg_hba.conf.j2
│       ├── vars/
│       │   └── main.yml
│       └── handlers/
│           └── main.yml
├── playbooks/
│   └── site.yml
├── .gitignore
└── README.md
```
