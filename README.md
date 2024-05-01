# helm-chart-basics

## helm-chart structure

          nextjs-express-mysql/
          │
          ├── charts/
          │   ├── nextjs/         # Next.js frontend sub-chart
          │   ├── express/        # Express backend sub-chart
          │   └── mysql/          # MySQL database sub-chart
          │
          ├── templates/          # Helm templates for the main chart
          │   ├── deployment.yaml     # Deployment configuration
          │   ├── service.yaml        # Service configuration
          │   └── ingress.yaml        # Ingress configuration
          │
          ├── values.yaml         # Helm values file
          └── Chart.yaml          # Chart metadata

## Explanation
- Chart Metadata (Chart.yaml): Contains metadata about the Helm chart, such as its name, description, and version.

- Values File (values.yaml): Contains configurable values for the Helm chart. It includes settings for each component (Next.js, Express, MySQL).
  
- Main Helm Templates:

- - Deployment Template (templates/deployment.yaml): Defines a Kubernetes Deployment with containers for Next.js, Express, and MySQL. It specifies the replica count and container images.

  - Service Template (templates/service.yaml): Defines Kubernetes Services to expose the Next.js and Express applications internally within the cluster.
 
  - Ingress Template (templates/ingress.yaml): Defines a Kubernetes Ingress resource to expose the application externally with an optional host.
