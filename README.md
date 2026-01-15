🚀 Cloud Deployment Project — CI/CD on Google Cloud
Developer → GitHub → GitHub Actions → SSH → Google Cloud VM → Docker → Nginx → Web App

🛠️ Technologies Used
Area	Stack
Cloud Provider	Google Cloud Platform
Compute	Compute Engine VM (Linux)
Containers	Docker
Web Server	Nginx
CI/CD	GitHub Actions
Security	SSH, Firewall Rules
Automation	GitHub Workflows
⚙️ How It Works

Code is pushed to the main branch on GitHub.

GitHub Actions triggers a deployment workflow.

The pipeline connects securely to the VM via SSH.

The application is rebuilt as a Docker image.

The running container is replaced with the new version.

The updated website is instantly available.

This ensures zero-downtime updates and full automation.

🧪 CI/CD Workflow

The deployment process is fully automated using this workflow:

.github/workflows/deploy.yml


It performs:

Git clone / pull

Docker image build

Container replacement

Service validation

🧩 Project Structure
.
├── Dockerfile
├── index.html
├── README.md
└── .github
    └── workflows
        └── deploy.yml

🔐 Security & Reliability

SSH authentication with private keys

Firewall rules exposing only required ports

Immutable Docker deployments

Automated recovery on redeploy

👨‍💻 Author

Roberto Slawinski
Cloud & DevOps Engineering Student
Portugal · 2026
