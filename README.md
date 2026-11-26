# Codex Comic Reader for TOS

Install the package for your NAS architecture on TOS 7 with Docker Engine. Open it from the desktop or visit `http://<NAS IP>:19202` on a trusted network. In the container console, read the generated password with `cat /config/.initial-admin-password`. Sign in as `admin`. Change the password and remove the initial password file after confirming the new password works.

Copy your comics to the TOS application data directory mounted at `/comics`. The corresponding NAS path is listed in the container's bind mounts in Docker Manager. In the Codex Admin Panel, add `/comics` as a library. A library without assigned groups is visible to anyone who can reach the service. Use groups for restricted libraries and a trusted HTTPS reverse proxy for remote access.

The comic archives are stored under `/comics`; the catalogue, users, reading position and settings live under `/config`. Stop Codex before backing them up. Codex runs as UID/GID 1000.

[Upstream guide](https://codex-comic-reader.readthedocs.io/) · [Upstream GPL-3.0 license](https://github.com/ajslater/codex/tree/v2.8.1) · [Privacy policy](PRIVACY.md)

## TOS 使用说明

请在安装了 Docker Engine 的 TOS 7 上选择对应架构的包。从 TOS 桌面打开应用，或在可信网络访问 `http://<NAS IP>:19202`。在容器控制台运行 `cat /config/.initial-admin-password`，用生成的密码登录 `admin`。修改密码并验证后，删除初始密码文件。

将漫画复制到挂载至 `/comics` 的目录，并在管理面板中添加此书库。未配置分组的书库可被能够访问服务的任何人浏览。需要限制访问时请配置分组，远程访问使用可信的 HTTPS 反向代理。

[隐私政策](PRIVACY.md)
