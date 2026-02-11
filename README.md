# API Testing Framework - Postman & Newman

A comprehensive API testing framework using Postman collections, Newman for CLI execution, HTML reporting, and Jenkins CI/CD integration.

## 📋 Features

- **Postman**: Developing detailed collections and thorough test cases
- **Newman**: Streamlining the execution of these collections
- **HTML Reports**: Creating in-depth reports for better insights
- **Jenkins**: Implementing Continuous Integration and Continuous Deployment (CI/CD) workflows

## 🚀 Setup

1. **Install dependencies:**
   ```bash
   npm install
   ```

2. **Install Newman globally (optional):**
   ```bash
   npm install -g newman
   ```

## 📁 Project Structure

```
api-testing-postman/
├── collections/              # Postman collections
│   └── Trello.postman_collection.json
├── environments/             # Postman environments
│   └── Trello.postman_environment.json
├── reports/                  # Test reports (generated)
├── jenkins/                  # Jenkins pipeline files
│   └── Jenkinsfile
├── package.json
└── README.md
```

## 🧪 Running Tests

### Run tests with Newman:
```bash
npm test
```

### Run tests with HTML report:
```bash
npm run test:html
```

### Run tests with CLI reporter:
```bash
npm run test:cli
```

### Run tests with JSON report:
```bash
npm run test:json
```

### Run all report types:
```bash
npm run test:all
```

## 📊 Reports

After running tests, HTML reports will be generated in the `reports/` directory:
- `newman-report.html` - Interactive HTML report
- `newman-report.json` - JSON report for programmatic access

## 🔧 Jenkins Integration

The project includes a Jenkinsfile for CI/CD integration. To use it:

1. Create a new Jenkins pipeline job
2. Point it to your repository
3. The pipeline will automatically:
   - Install dependencies
   - Run API tests
   - Generate HTML reports
   - Archive test results

### Jenkins Pipeline Features:
- Automated test execution
- HTML report generation
- Test result archiving
- Email notifications on failure

## 📝 Postman Collections

### Trello API Collection
- **Collection**: `collections/Trello.postman_collection.json`
- **Environment**: `environments/Trello.postman_environment.json`

The collection includes:
- Authentication tests
- Board management
- List operations
- Card operations
- Comprehensive test assertions

## 🎯 Best Practices

1. **Environment Variables**: Use environment files for different test environments (dev, staging, prod)
2. **Test Data**: Keep test data separate from collections
3. **Assertions**: Include comprehensive assertions for all API responses
4. **Documentation**: Document each request and test case
5. **Version Control**: Keep collections and environments in version control

## 📦 Dependencies

- **newman** 6.0.0 - CLI companion for Postman

## 🔗 Resources

- [Postman Documentation](https://learning.postman.com/docs/)
- [Newman Documentation](https://github.com/postmanlabs/newman)
- [Jenkins Documentation](https://www.jenkins.io/doc/)

## 📄 License

ISC

## 👤 Author

Mina Nagy QA Engineer
