# Install description

## Add repository
helm repo add hoppscotch https://nicklaswallgren.github.io/hoppscotch-helm/

## Install release with custom values
helm repo update
helm install hoppscotch -f values.yaml -n hoppscotch-system --create-namespace hoppscotch/hoppscotch

## Dry run
helm install --dry-run hoppscotch -f values.yaml -n hoppscotch-system --create-namespace hoppscotch/hoppscotch

## Uninstall release
helm uninstall hoppscotch

## Fetch the chart
helm fetch hoppscotch/hoppscotch --untar
