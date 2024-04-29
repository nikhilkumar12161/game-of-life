pipeline {
  agent any  // Defines where the pipeline will run (any available agent)

   stages {  // Defines different stages in the pipeline
      stage('Checkout') {
          // Get the source code from a version control system (e.g., Git)
          steps {
              git branch: 'master',  // Replace 'main' with your branch name
                 url: 'https://github.com/nikhilkumar12161/game-of-life.git'
          }
      }
      stage('Build') {
          // Perform actions to build your application (e.g., compile code)
          steps {
              sh 'mvn compile' // Replace 'mvn compile' with your specific build command
          }
      }
      stage('Test') {
          // Run automated tests to ensure code functionality
          steps {
              sh 'mvn test'  // Replace 'mvn test' with your specific test command
          }
      }
  }
}
 
