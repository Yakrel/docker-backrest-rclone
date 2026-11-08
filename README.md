# Docker Backrest + Rclone

A specialized utility container designed for automated backups. It combines the `backrest` backup tool with `rclone` for cloud storage synchronization.

## 🛠 Included Tools
- **Backrest:** For efficient backup orchestration.
- **Rclone:** For syncing backups to cloud providers (Google Drive, S3, etc.).
- **Cron:** For scheduling periodic tasks.

## 🐳 Docker Hub
The image is published to: **[ghcr.io/yakrel/docker-backrest-rclone](https://github.com/Yakrel/docker-backrest-rclone/pkgs/container/docker-backrest-rclone)**

## 🔄 Build Policy
- **Schedule:** Builds run weekly (Sunday at 02:00 UTC), on pushes to `main`, and on manual dispatch. A keepalive job re-enables the scheduled workflow on each scheduled run so GitHub does not disable it after 60 days of repository inactivity.
- **Retention:** Keeps the 2 most recent image versions (each carries `latest`/dated tags as applicable); older tagged and untagged versions are deleted after every build.
