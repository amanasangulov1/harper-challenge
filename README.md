# HarperDB test

This repository contains a Docker Compose setup and a GitHub Actions pipeline that:
- Deploys a HarperDB container
- Inserts, updates, and verifies data using the HarperDB Operations API
- Collects performance metrics from the container

## 📦 Contents

- `docker-compose.yml` – HarperDB container setup
- `.env` – Environment variables (ignored in Git)
- `.github/workflows/main.yml` – GitHub Actions workflow
- `container_stats.txt` – Placeholder for performance metrics
- `README.md` – Instructions and documentation

## ✅ Setup Instructions

1. Clone this repository
2. Create a `.env` file with your admin password:
   ```
   HDB_ADMIN_PASSWORD=YourSecurePassword
   ```

3. Run the container locally (optional):
   ```bash
   docker-compose up
   ```

4. Push the code to a **public GitHub repository**
5. Add the `HDB_ADMIN_PASSWORD` as a GitHub Secret
6. GitHub Actions will handle the CI/CD pipeline automatically

## 🧪 HarperDB API Example Used

Operations follow examples from the [HarperDB API Quickstart](https://docs.harperdb.io/docs/developers/operations-api/quickstart-examples).
