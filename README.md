# code-server

Run VS Code on a remote server.

## Overview

- Repository: [alzkdpf/code-server](https://github.com/alzkdpf/code-server)
- Visibility: Public
- Last updated: 2021-12-16
- Main stack: TypeScript, Node.js, Docker

## Project Structure

```text
.dockerignore
.github/CODEOWNERS
.github/ISSUE_TEMPLATE/bug_report.md
.github/ISSUE_TEMPLATE/extension_bug.md
.github/ISSUE_TEMPLATE/feature_request.md
.github/ISSUE_TEMPLATE/question.md
.github/pull_request_template.md
.gitignore
.node-version
.travis.yml
Dockerfile
LICENSE
README.md
deployment/chart/Chart.yaml
deployment/chart/README.md
deployment/chart/values.yaml
deployment/manifests/deployment.yaml
doc/assets/aws_ubuntu.png
doc/assets/chrome_warning.png
doc/assets/cli.png
doc/assets/cros.png
doc/assets/do-new-droplet-btn.svg
doc/assets/ide.png
doc/assets/logo-horizontal.png
doc/assets/release.gif
doc/assets/server-password-modal.png
doc/security/code-server.fail2ban.conf
doc/security/fail2ban.md
doc/security/ssl.md
doc/self-hosted/cros-install.md
doc/self-hosted/index.md
package.json
packages/disposable/package.json
packages/disposable/yarn.lock
packages/dns/.gcloudignore
packages/dns/Dockerfile
packages/dns/app.yaml
packages/dns/package.json
packages/dns/webpack.config.js
packages/dns/yarn.lock
packages/events/package.json
packages/events/yarn.lock
packages/ide/package.json
packages/ide/yarn.lock
packages/ide-api/README.md
```

## Getting Started

Install dependencies or prepare the project:

```bash
npm install
```

Run the common development command:

```bash
npm run dev
```

## Available Scripts

- `build:rules`: `cd ./rules && tsc -p .`
- `packages:install`: `cd ./packages && yarn`
- `postinstall`: `npm-run-all --parallel packages:install build:rules`
- `start`: `cd ./packages/server && yarn start`
- `task`: `ts-node -r tsconfig-paths/register build/tasks.ts`
- `test`: `cd ./packages && yarn test`

## Notes

- This README was generated from the repository metadata and file structure.
- Update this document when setup steps, deployment targets, or project ownership changes.
