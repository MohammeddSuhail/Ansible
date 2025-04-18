.
├── ReadMe.md
├── Server_Clean_Up/
    ├── ansible.cfg
    ├── inventory/
    │   ├── config
    │   ├── group_vars/
    │   │   └── all/
    │   │       └── vars.yml
    │   └── hosts
    ├── playbook/
    │   ├── home_directory_usage_alerter.yml
    │   └── region_junk_remover.yml
    └── roles/
        ├── home_directory_usage_alerter/
        │   ├── files/
        │   │   ├── email_alerts.py
        │   │   ├── email_extractor.py
        │   │   ├── home_disk_usage_report.py
        │   │   └── jira_email_fetcher.py
        │   └── tasks/
        │       ├── email_address_gathering.yml
        │       ├── home_disk_usage.yml
        │       └── send_email_alerts.yml
        └── region_junk_remover/
            ├── tasks/
            │   └── junk_find_and_delete.yml
            └── templates/
                ├── junk_deleter.py.j2
                ├── junk_finder.py.j2
                └── report_formatter.py.j2







.
├── ansible/
│   ├── ansible.cfg
│   ├── config
│   ├── inventory/
│   │   ├── group_vars/
│   │   │   ├── all/
│   │   │   │   └── vars.yml
│   │   │   ├── app_srv/
│   │   │   │   └── vars.yml
│   │   │   ├── db_srv/
│   │   │   │   └── vars.yml
│   │   │   ├── om_srv/
│   │   │   │   └── vars.yml
│   │   │   └── webui_srv/
│   │   │       └── vars.yml
│   │   ├── host_vars/
│   │   │   ├── host1/
│   │   │   │   └── vars.yml
│   │   │   ├── host2/
│   │   │   │   └── vars.yml
│   │   │   └── host3/
│   │   │       └── vars.yml
│   │   └── hosts
│   ├── playbook/
│   │   ├── region_create.yml
│   │   ├── region_delete.yml
│   └── roles/
│       ├── region/
│       │   ├── tasks/
│       │   │   ├── backup_app.yml
│       │   │   ├── restore_app.yml
│       │   │   ├── post_install_icg.yml
│       │   │   ├── delete_region.yml
│       │   │   ├── deploy_region.yml
│       │   │   ├── install_region.yml
│       │   └── templates/
│       │       └── create_region.ini.j2
│       ├── database/
│       │   ├── tasks/
│       │   │   ├── backup_db.yml
│       │   │   ├── create_cert_postgres.yml
│       │   │   ├── dump_pg_parallel.yml
│       │   │   ├── restore_pg_parallel.yml
│       │   │   ├── restore_db.yml
│       │   │   ├── create_schema.yml
│       │   │   ├── create_schema_oracle.yml
│       │   │   ├── create_schema_postgres.yml
│       │   │   ├── delete_schema.yml
│       │   └── templates/
│       │       ├── schema_definition_oracle.sql.j2
│       │       └── schema_definition_postgres.sql.j2
└── ReadMe.md




