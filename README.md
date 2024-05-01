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
