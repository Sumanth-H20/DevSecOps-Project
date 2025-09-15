# DevSecOps-Project
🧮 Spring Boot Calculator with Modern UI
Prerequisites
Java 17 or higher
Maven 3.6+
Docker (optional)
Kubernetes cluster (optional)
Option 1: Run with Maven
# Clone the repository
git clone <repository-url>
cd calculator-app

# Run the application
./mvnw spring-boot:run

# Or build and run the JAR
./mvnw clean package
java -jar target/calculator-app-0.0.1-SNAPSHOT.jar
Option 2: Run with Docker
# Build and run with Docker
docker build -t calculator-app .
docker run -p 8081:8081 calculator-app

# Or use Docker Compose
docker-compose up
Option 3: Deploy to Kubernetes
# Apply Kubernetes manifests
kubectl apply -f Deployment.yaml

# Check deployment status
kubectl get pods -l app=calculator-app

# Access via port-forward
kubectl port-forward service/calculator-app-service 8081:80
