<div align="center">

# 🚀 Postman API Testing Project

![Newman Tests](https://github.com/patmcdaniel37/postman/actions/workflows/newman-tests.yml/badge.svg)
![Collections](https://img.shields.io/badge/collections-6-blue)
![Tests](https://img.shields.io/badge/tests-150+-green)
![License](https://img.shields.io/badge/license-MIT-green)

## Quick Stats
6 Collections | 150+ Tests | 3 APIs<br>
100% Pass Rate | Average Response Time: <200ms<br>
CI/CD Integrated | Automated Reporting

### API testing project showcasing <br>CRUD, Authentication, E2E Workflows & Advanced Techniques

</div>

---

## 📋 Overview

This portfolio demonstrates comprehensive API testing skills using Postman and Newman.

## 🎯 Collections

1. **RESTful API Fundamentals** - CRUD operations with JSONPlaceholder running in dev env
2. **Authentication/Authorization** - Token-based auth with Restful-Booker running in dev env
3. **E-commerce API Testing** - Complex workflows with FakeStore API running in stage env
4. **Data Driven Testing** - CSV/JSON parameterization running in stage env
5. **E2E Shopping Workflow** - Complete user journey running in prod env
6. **Advanced Techniques** - Schema validation, performance testing running in prod env

## 🚀 Getting Started

### Prerequisites
- Postman Desktop App
- Node.js v18+
- Newman CLI

### Installation
```bash
# Clone the repository
git clone https://github.com/patmcdaniel37/postman.git
cd postman

# Install dependencies
npm install -g newman newman-reporter-htmlextra
```

### Running Tests
```bash
# Run all collections
bash newman/run-all-tests.sh

# Run specific collection
newman run postman/collections/01-*.json \
  -e postman/environments/API_Testing.postman_environment.json

# Run specific collection
newman run postman/collections/01-*.json \
  -e postman/environments/API_Testing.postman_environment.json
```

### Data Driven Test Files
> ###### CSV Dataset
```
title, price, description, image, category
USB-C Flash Drive 99TB, 99.99, USB-C Flash Drive 99TB, https://fakestoreapi.com/img/123ABC_99TB.png, electronics
Bluetooth Keyboard/Mouse, 79.99, Bluetook Keyboard and Mouse, https://fakestoreapi.com/img/456ABC_BTKM.png, electronics
Screen Cleaner Wipes, 9.99, Anti-Static Screen Cleaner Wipes, https://fakestoreapi.com/img/789ABC_SCW.png, electronics
```
> ###### JSON Dataset
```
[
    {
        "title" : "USB-C Flash Drive 99TB",
        "price" : "99.99",
        "description" : "USB-C Flash Drive 99TB",
        "image" : "https://fakestoreapi.com/img/123ABC_99TB.png",
        "category" : "electronics"
    },
    {
        "title" : "Bluetooth Keyboard/Mouse",
        "price" : "79.99",
        "description" : "Bluetook Keyboard and Mouse",
        "image" : "https://fakestoreapi.com/img/456ABC_BTKM.png",
        "category" : "electronics"
    },
    {
        "title" : "Screen Cleaner Wipes",
        "price" : "9.99",
        "description" : "Anti-Static Screen Cleaner Wipes",
        "image" : "https://fakestoreapi.com/img/789ABC_SCW.png",
        "category" : "electronics"
    }
]
```

## 📊 Test Reports

Sample test report:

<img src="postman/docs/images/test-report-screenshot.png" width="400px">

## Performance Benchmarks
- Average GET response time: < 200ms
- Average POST response time: < 500ms
- All tests complete in: ~45 seconds
  
## 🛠️ Technology Stack

- **Postman** - API development and testing
- **Newman** - CLI collection runner
- **Newman HTML Extra** - Enhanced test reporting
- **GitHub Actions** - CI/CD automation

## 📁 Project Structure
```
postman/
├── collections/        # Postman collections
├── environments/       # Environment configurations
├── data/              # Test data (CSV, JSON)
├── reports/           # Generated HTML reports
└── newman/            # Newman scripts
```

## 🤝 Contributing

Feel free to fork this project and submit pull requests.

## 📄 License

This project is licensed under the MIT License.

## 📧 Contact

Patrick McDaniel - [GitHub](https://github.com/patmcdaniel37)
