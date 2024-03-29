## Give your Application Auto-Deploy Superpowers

In this project, you will prove your mastery of the following learning objectives:

- Explain the fundamentals and benefits of CI/CD to achieve, build, and deploy automation for cloud-based software products.
- Utilize Deployment Strategies to design and build CI/CD pipelines that support Continuous Delivery processes.
- Utilize a configuration management tool Ansible to accomplish deployment to cloud-based servers.
- Surface critical server errors for diagnosis using centralized structured logging.

![Diagram of CI/CD Pipeline we will be building.](udapeople.png)

### Instructions

* [Selling CI/CD](instructions/0-selling-cicd.md)
* [Getting Started](instructions/1-getting-started.md)
* [Deploying Working, Trustworthy Software](instructions/2-deploying-trustworthy-code.md)
* [Configuration Management](instructions/3-configuration-management.md)
* [Turn Errors into Sirens](instructions/4-turn-errors-into-sirens.md)

### Project Submission

For your submission, please submit the following:

- A text file named `urls.txt` including:
  1. Public Url to GitHub repository (not private) [URL01]
  1. Public URL for your S3 Bucket (aka, your green candidate front-end) [URL02]
  1. Public URL for your CloudFront distribution (aka, your blue production front-end) [URL03]
  1. Public URLs to deployed application back-end in EC2 [URL04]
  1. Public URL to your Prometheus Server [URL05]
- Your screenshots in JPG or PNG format, named using the screenshot number listed in the instructions. These screenshots should be included in your code repository in the root folder.
  1. Job failed because of compile errors. [SCREENSHOT01]
  1. Job failed because of unit tests. [SCREENSHOT02]
  1. Job that failed because of vulnerable packages. [SCREENSHOT03]
  1. An alert from one of your failed builds. [SCREENSHOT04]
  1. Appropriate job failure for infrastructure creation. [SCREENSHOT05]
  1. Appropriate job failure for the smoke test job. [SCREENSHOT06]
  1. Successful rollback after a failed smoke test. [SCREENSHOT07]  
  1. Successful promotion job. [SCREENSHOT08]
  1. Successful cleanup job. [SCREENSHOT09]
  1. Only deploy on pushed to `master` branch. [SCREENSHOT10]
  1. Provide a screenshot of a graph of your EC2 instance including available memory, available disk space, and CPU usage. [SCREENSHOT11]
  1. Provide a screenshot of an alert that was sent by Prometheus. [SCREENSHOT12]

- Your presentation should be in PDF format named "presentation.pdf" and should be included in your code repository root folder. 

Before you submit your project, please check your work against the project rubric. If you haven’t satisfied each criterion in the rubric, then revise your work so that you have met all the requirements. 

### Built With

- [Circle CI](www.circleci.com) - Cloud-based CI/CD service
- [Amazon AWS](https://aws.amazon.com/) - Cloud services
- [AWS CLI](https://aws.amazon.com/cli/) - Command-line tool for AWS
- [CloudFormation](https://aws.amazon.com/cloudformation/) - Infrastrcuture as code
- [Ansible](https://www.ansible.com/) - Configuration management tool
- [Prometheus](https://prometheus.io/) - Monitoring tool

## AUTO-DEPLOY PIPELINE RESULTS
1. Job failed because of compile errors. [SCREENSHOT01]

![Backend-Build](screenshoots/SCREENSHOT01.png)



2. Job failed because of unit tests. [SCREENSHOT02]

![Backend-Test](screenshoots/SCREENSHOT02.png)



3. Job that failed because of vulnerable packages. [SCREENSHOT03]

![Backend-Scan](screenshoots/SCREENSHOT03.png)



4. An alert from one of your failed builds. [SCREENSHOT04]

![Failed Job Alert](screenshoots/SCREENSHOT04.png)



5. Appropriate job failure for infrastructure creation. [SCREENSHOT05]

![Infrastructure-Job Appropriate Failure](screenshoots/SCREENSHOT05.png)


6. Appropriate job failure for the smoke test job. [SCREENSHOT06]

![Failed Job Alert](screenshoots/SCREENSHOT06.png)



7. Successful rollback after a failed smoke test. [SCREENSHOT07] 

![Successful Rollack](screenshoots/SCREENSHOT07.png)


8. Successful promotion job. [SCREENSHOT08]

![Promotion job Succeed](screenshoots/SCREENSHOT08.png)



9. Successful cleanup job (Destroy Old Infra. on New Infra. Deployment Success) [SCREENSHOT09]

![Clean-Up Success](screenshoots/SCREENSHOT09.png)



10. Only deploy on pushed to `master` branch. [SCREENSHOT10]

![Deploy OnlyMaster](screenshoots/SCREENSHOT10.png)



11. Provide a screenshot of a graph of your EC2 instance including available memory, available disk space, and CPU usage. [SCREENSHOT11]

CPU USAGE MONITORING
![CPU usage](screenshoots/SCREENSHOT11_CPU_USAGE.png)

DISK USAGE MONITORING
![Disk usage](screenshoots/SCREENSHOT11_DISK_USAGE.png)

MEMORY USAGE MONITORING
![Memory usage](screenshoots/SCREENSHOT11_MEMORY_USAGE.png)




12. Provide a screenshot of an alert that was sent by Prometheus. [SCREENSHOT12]

![Instance Down](screenshoots/SCREENSHOT12_INSTANCE_DOWN.png)

ALERT SENT BY PROMETHEUS
![Alert](screenshoots/SCREENSHOT12.png)

#### URLS

13. Public URL for your CloudFront distribution (aka, your blue production front-end) [URL03]
![Cloudfront URL](screenshoots/URL03_SCREENSHOT.png)

14. Public URLs to deployed application back-end in EC2 [URL04]
![Backend Status](screenshoots/URL04_SCREENSHOT.png)

15. Public URL to your Prometheus Server, To List Target Instances [URL05]
![Target Instances](screenshoots/URL05_SCREENSHOT.png)

INSTANCE STATUS IS DOWN
![Target Instance Down](screenshoots/URL05_SCREENSHOT_DOWN.png)

### License

[License](LICENSE.md)
