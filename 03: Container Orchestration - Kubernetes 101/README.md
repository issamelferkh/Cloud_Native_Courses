# Container Orchestration - Kubernetes 101

## Why Container Orchestration
- diff between test (local machine) and prod (cloud)
- run containers with default ports
  - containers created with random ports
- Issue:
  - In Cloud we can't pre-config security group or load balancer before
  - need run containers -> list open ports ->  re-conf sec group + load balancer
  - In case restart containers -> they take other random ports
- Solution:
  - Need and external tool -> that can listen and understand: the platform + open ports + running containers ...
  - Container Orchestration Platform










## Kubernetes Concepts
 