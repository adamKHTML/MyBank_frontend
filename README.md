docker run --name mybank_frontend -p 8091:80 mybank_frontend     
docker build . -t mybank_frontend 

Deploy with Jenkins

docker build -t jenkins-agent-frontend-mybank .

docker run --init --name jenkins_agent_frontend_mybank -v /var/run/docker.sock:/var/run/docker.sock jenkins-agent-frontend-mybank -url http://172.17.0.2:8080 99e201efd0b42d7bbef02e85084e7eec483aecc97c18087e441a3a97d50fda81  MBReactAgent
