# CI/CD
## Setup CI
### 1. What is CI



### 2. Planifiez votre dev

### 3. Intégrez votre code en continu
- Create GitLab Repo
  - Create gitlab repo

- Clone the gitlab repo 
https://gitlab.com/issamelferkh/ci-cd.git

- In GitLab repo Pull the App Code source from github repo
  - Add remote from github
    - Check remotes
      e1r9p7% git remote -v
      origin  https://gitlab.com/issamelferkh/ci-cd.git (fetch)
      origin  https://gitlab.com/issamelferkh/ci-cd.git (push)

    - Add and Check new remotes
      e1r9p7% git remote add issam https://github.com/spring-petclinic/spring-petclinic-microservices.git
      e1r9p7% git remote -v                                                                              
      issam   https://github.com/spring-petclinic/spring-petclinic-microservices.git (fetch)
      issam   https://github.com/spring-petclinic/spring-petclinic-microservices.git (push)
      origin  https://gitlab.com/issamelferkh/ci-cd.git (fetch)
      origin  https://gitlab.com/issamelferkh/ci-cd.git (push)

    - Pull App code source from remote (github repo) using srcs shortname
      - git pull issam master --allow-unrelated-histories

    - Push App code source to gitlab repo
      - git push origin main

- Setup CI
  - Install your own runner: https://docs.gitlab.com/runner/install/
  - Create a new .gitlab-ci.yml file at the root of the repository to get started.
  - .gitlab-ci.yml
    - Add config: Stages (Build (build_job) + Test (test_job))
    - Run it: from CI/CD -> Piplines -> 


```yaml
stages:          # List of stages for jobs, and their order of execution
  - build
  - test
  - Deploy

build-job:       # This job runs in the build stage, which runs first.
  stage: build
  script:
    - echo "Compiling the code..."
    - echo "Compile complete."

unit-test-job:   # This job runs in the test stage.
  stage: test    # It only starts when the job in the build stage completes successfully.
  script:
    - echo "Running unit tests... This will take about 60 seconds."
    - sleep 60
    - echo "Code coverage is 90%"

lint-test-job:   # This job also runs in the test stage.
  stage: test    # It can run at the same time as unit-test-job (in parallel).
  script:
    - echo "Linting code... This will take about 10 seconds."
    - sleep 10
    - echo "No lint issues found."

deploy-job:      # This job runs in the deploy stage.
  stage: deploy  # It only runs when *both* jobs in the test stage complete successfully.
  script:
    - echo "Deploying application..."
    - echo "Application successfully deployed."

```


















## CD