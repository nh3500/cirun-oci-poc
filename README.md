# cirun-oci-poc

Throwaway proof of concept: ephemeral GitHub Actions runners on Oracle Cloud (E5.Flex, ap-tokyo-1) through Cirun.

- `p1-shape`: one job per `.cirun.yml` variant; reports the shape, OCPU and memory the VM actually got.
- `p2-burst`: N parallel jobs on one variant plus a GitHub-hosted reference job; reports boot latency, GitHub egress and CPU.

Workflows run only on `workflow_dispatch`, so forks cannot start a runner. This repository will be deleted after the test.
