**Helm Basics:**
- `helm create <chart-name>`: Create a new Helm chart.
- `helm install <release-name> <chart-name>`: Install a chart and create a release.
- `helm upgrade <release-name> <chart-name>`: Upgrade a release to a new version of a chart.
- `helm uninstall <release-name>`: Uninstall a release and remove the associated resources.
- `helm list`: List all installed releases.
- `helm status <release-name>`: Show the status of a release.
- `helm rollback <release-name> <revision-number>`: Rollback a release to a specific revision.
- `helm history <release-name>`: Show the revision history of a release.
- `helm dependency update`: Update the dependencies of a chart.
- `helm dependency build`: Build the dependencies of a chart.
- `helm template <chart-name>`: Render the templates of a chart without installing it.
- `helm lint <chart-name>`: Lint a chart for best practices and errors.
- `helm package <chart-directory>`: Package a chart into a compressed tarball.
- `helm install <tarball>`: Install a chart directly from a tarball.
- `helm get <resource> <release-name>`: Get information about a specific resource in a release.
- `helm repo add <repository-name> <repository-url>`: Add a new Helm repository.
- `helm repo update`: Update the local cache of Helm repositories.

**Chart Configuration:**
- `helm show chart <chart-name>`: Show the chart details and metadata.
- `helm show values <chart-name>`: Show the default values of a chart.
- `helm get values <release-name>`: Get the overridden values of a release.
- `helm install --set <key=value>`: Override values during installation.
- `helm upgrade --set <key=value>`: Override values during upgrade.
- `helm upgrade --reuse-values`: Reuse the previous release's values during upgrade.
- `helm install --values <values-file>`: Specify custom values file during installation.
- `helm upgrade --values <values-file>`: Specify custom values file during upgrade.
- `helm install --set-file <key=file>`: Specify values from a file during installation.
- `helm upgrade --set-file <key=file>`: Specify values from a file during upgrade.
- `helm install --set-string <key=value>`: Override string values during installation.
- `helm upgrade --set-string <key=value>`: Override string values during upgrade.
- `helm install --set-file <key=file>`: Override values from a YAML file during installation.
- `helm upgrade --set-file <key=file>`: Override values from a YAML file during upgrade.
- `helm install --set-json <key=value>`: Override values using JSON syntax during installation.
- `helm upgrade --set-json <key=value>`: Override values using JSON syntax during upgrade.

**Working with Repositories:**
- `helm repo list`: List all added Helm repositories.
- `helm repo update`: Update the local cache of Helm repositories.
- `helm repo remove <repository-name>`: Remove a Helm repository from the local configuration.
- `helm search <chart-name>`: Search for charts in the added repositories.
- `helm search repo <keyword>`: Search for charts in the added repositories based on a keyword.
- `helm pull <repository-name>/<chart-name>`: Download a chart from a repository without installing it.
- `helm repo index <chart-directory>`: Generate an index file for a local chart repository.

**Hooks and Lifecycle Management:**
- `helm test <release-name>`: Run tests defined in a chart.
- `helm plugin install <plugin-name>`: Install a Helm plugin.
- `helm plugin uninstall <plugin-name>`: Uninstall a Helm plugin.

**Helm Security:**
- `helm repo add <repository-name> <repository-url> --username <username> --password <password>`: Add a Helm repository with authentication credentials.
- `helm repo update --username <username> --password <password>`: Update the local cache of Helm repositories with authentication credentials.
