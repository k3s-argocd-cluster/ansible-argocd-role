Inject centrally controlled ansible variables into ArgoCD GitOps repository and ansible tasks to install ArgoCD and Bootstrap repository.

|Variable|Description|
|---|---|
|{{ argocd_password }}|The password for the admin account to be used|
|{{ dns_names.argocd }}|DNS name to be used for ArgoCD|
|{{ dns_names.duplicati }}|DNS name to be used for duplicati|
|{{ dns_names.gitea }}|DNS name to be used for gitea|
|{{ dns_names.haproxy }}|DNS name to be used for haproxy|
|{{ dns_names.iobroker }}|DNS name to be used for iobroker|
|{{ dns_names.longhorn }}|DNS name to be used for longhorn|
|{{ dns_names.minio }}|DNS name to be used for minio UI|
|{{ dns_names.netdata }}|DNS name to be used for netdata|
|{{ dns_names.pihole }}|DNS name to be used for pihole|
|{{ dns_names.postgresql }}|DNS name to be used for PostgreSQL|
|{{ dns_names.s3 }}|DNS name to be used for minio S3 API|
|{{ dns_names.samba }}|DNS name to be used for Samba|
|{{ dns_names.tekton }}|DNS name to be used for tekton dashboard|
|{{ dns_names.traefik }}|DNS name to be used for traefik|
|{{ fritzbox.dns }}|DNS name of your fritzbox, if exists|
|{{ fritzbox.ip }}|IP of your fritzbox, if exists|
|{{ gitea_settings.admin.email }}|The gitea admin user email address|
|{{ images.argocd_sidecar }}|Sidecar image for custom build stages using cmp plugin|
|{{ images.busybox }}|Image for busybox|
|{{ images.duplicati }}|Image for duplicati|
|{{ images.iobroker }}|Image for iobroker|
|{{ images.kaniko_executor }}|Image for kaniko executor|
|{{ images.manifest_tool }}|Image for manifest-tool|
|{{ images.minio }}|Image for minio|
|{{ images.postgresql }}|Image for postgresql|
|{{ images.recover_volume }}|Image for recover-volume-presync hook|
|{{ kubernetes.argocd.version }}|ArgoCD to be used|
|{{ kubernetes.gitea.version }}|Gitea version to be used|
|{{ kubernetes.longhorn.repository_organisation }}|Organisation to retrieve the longhorn repository from, useful for forks|
|{{ kubernetes.longhorn.version }}|Longhorn version (i.e. git tag) to be used|
|{{ kubernetes.metallb.version }}|metallb version to be used|
|{{ kubernetes.netdata.room }}|The netdata room to join|
|{{ kubernetes.netdata.version }}|netdata version to be used|
|{{ kubernetes.pihole.version }}|pihole version to be used|
|{{ kubernetes.sealedsecrets.version }}|sealed-secrets (Bitnami) to be used|
|{{ kubernetes.tekton.dashboard.version }}|tekton dashboard version to be used|
|{{ kubernetes.tekton.pipeline.version }}|tekton pipeline version to be used|
|{{ kubernetes.tekton.tasks.git_clone.version }}|git-clone task version from tekton hub|
|{{ kubernetes.tekton.tasks.kaniko.version }}|kaniko task version from tekton hub|
|{{ kubernetes.tekton.triggers.version }}|tekton triggers version to be used|
|{{ kubernetes.traefik.version }}|traefik version to be used|
|{{ metallb.ips.pihole }}|IP for your pihole to be assigned and managed from metallb|
|{{ metallb.ips.postgresql }}|IP for PostgreSQL to be assigned and managed from metallb|
|{{ metallb.ips.traefik }}|IP for traefik to be assigned and managed from metallb|
|{{ metallb.range }}|Range of IPs available to metallb|
|{{ postgresql_settings.additional_databases }}|Additional databases to be created when starting PostgreSQL|
|{{ postgresql_settings.database }}|Main PostgreSQL database|
|{{ postgresql_users }}|List of additional users (and their credentials) to be created when starting PostgreSQL|
