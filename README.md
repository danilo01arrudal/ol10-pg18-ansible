# oracle linux 10 + postgres + bash + ansible

```
.
├── ansible.cfg
├── group_vars
│   ├── all
│   │   └── vars.yml
│   ├── pg_classe_grande
│   │   └── vars.yml
│   ├── pg_classe_media
│   │   └── vars.yml
│   └── pg_classe_pequena
│       └── vars.yml
├── inventory
│   └── production
├── playbooks
│   ├── site.yml
│   └── uninstall.yml
├── README.md
└── roles
    └── postgresql
        ├── handlers
        │   └── main.yml
        ├── tasks
        │   ├── configure.yml
        │   ├── init.yml
        │   ├── install.yml
        │   ├── main.yml
        │   └── uninstall.yml
        ├── templates
        │   ├── pg_hba.conf.j2
        │   └── postgresql.conf.j2
        └── vars
            └── main.yml
```

1. Pré‑requisitos

 - Máquina de controle com Ansible instalado (pode ser sua estação ou outra VM).
 - Acesso SSH da máquina de controle para a VM Oracle Linux 10 (com chave pública ou senha).
 - Python 3 instalado na VM alvo (geralmente já vem no Oracle Linux).
 - Repositório GitHub para armazenar o projeto.

