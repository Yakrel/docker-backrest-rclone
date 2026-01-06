# Docker Backrest + Rclone

A specialized utility container designed for automated backups. It combines the `backrest` backup tool with `rclone` for cloud storage synchronization.

## 🛠 Included Tools
- **Backrest:** For efficient backup orchestration.
- **Rclone:** For syncing backups to cloud providers (Google Drive, S3, etc.).
- **Cron:** For scheduling periodic tasks.

## 🐳 Docker Hub
The image is published to: **[yakrel93/backrest-rclone](https://hub.docker.com/r/yakrel93/backrest-rclone)**

## 🔄 Build Policy
- **Schedule:** Builds run twice a week (Sunday & Wednesday at 02:00 UTC).
- **Retention:** Retains `latest` and the last **5** dated tags.
