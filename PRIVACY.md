# Codex Comic Reader on TOS privacy policy

The NAS administrator operates Codex. Codex stores comic archives and metadata, account names and password hashes, reading progress and bookmarks, access settings and logs. It uses these records to catalogue a library, authenticate users and keep reading state. Data is stored on the NAS. Libraries without assigned groups are accessible to all clients that can reach the service.

Local indexing reads the files provided by the NAS administrator. If enabled, online metadata tagging can send title, series or issue information to the configured metadata providers. Optional OIDC or email features communicate with the configured identity or email services. Codex checks for upstream releases. GitHub receives normal network request metadata during the release check and when the NAS pulls the container image.

Data remains until deleted from the library, account, or NAS storage, subject to backup retention. Use Codex to review or correct applicable metadata and reading records, or contact the NAS administrator to remove accounts, archives, logs or backup copies. Packaging support is available in the [package repository](https://github.com/LuYifei-TOS-Apps/tos-codex-comic-reader/issues).

The package generates a unique first-login credential and runs Codex without root privileges. Use library groups and restrict backups, the password file and configuration access. Use HTTPS when accessing Codex remotely.
