# Jenkins

### Developing an App
1. **Writing Code (Developer → Code Repo - GitHub)**: 
   - A developer writes the code for the app. This code is then stored in a code repository, like **GitHub**. GitHub is like a cloud-based storage for your code, where you can track changes, collaborate with others, and maintain different versions of the code.

2. **Build it and Store in Docker Hub**:
   - After writing the code, the next step is to **build** it. This means converting your code into an executable or a ready-to-deploy version.
   - **Docker** helps in creating containers for your app. A container is like a lightweight, portable package that includes everything your app needs to run (code, libraries, etc.).
   - Once the app is built, it's pushed (stored) to **Docker Hub**, a service where you can store and share Docker images (your app's containers).

3. **Deploy it in Server (e.g., AWS)**:
   - The app needs to be hosted on a server so users can access it. For example, you can use **AWS** (Amazon Web Services) to deploy your app to a cloud server. The server makes the app available to users over the internet.

### Jenkins and CI/CD Pipelines
**Jenkins** is a tool that automates the entire process from coding to deployment. It helps save time and ensures that your code gets tested and deployed automatically whenever there are changes. This is done using **CI/CD pipelines**.

1. **CI/CD Pipeline**:
   - **CI (Continuous Integration)**: Automatically merges new code changes and runs tests to check for errors.
   - **CD (Continuous Delivery or Continuous Deployment)**: Automates the process of preparing the code for production and sometimes even automatically deploys it to production servers.

### Jenkins Types:
Jenkins can help you set up CI/CD pipelines, and it offers two main ways to do this:

1. **Freestyle Project (Using Jenkins GUI)**:
   - A simple way to create a pipeline using Jenkins' graphical user interface (GUI). You don’t need to write any scripts; instead, you can click buttons and configure the pipeline with options in the GUI. This is good for beginners or small projects.

2. **Pipeline (Using Jenkinsfile)**:
   - **Scripting (Declarative/Scripted)**: 
     - **Scripted Pipeline**: This is the older way of writing Jenkins pipelines using **Groovy scripting**. It's more flexible but requires more advanced knowledge of programming.
     - **Declarative Pipeline**: A newer, easier way to define a pipeline. It’s simpler and uses a structured format to define steps like build, test, and deploy. It's the recommended way for most users.

### In Simple Terms:
- **Jenkins** automates the process of testing and deploying code. When you change something in the code, Jenkins runs the tests and then automatically builds and deploys the app to a server like AWS.
- **Freestyle projects** let you use Jenkins through a simple point-and-click interface.
- **Pipelines** let you write automated workflows to manage the entire process, from building to deploying, using either scripts (more flexible) or a declarative structure (easier to read and write).

So, Jenkins automates everything, allowing developers to focus on writing code while Jenkins handles testing, building, and deploying that code automatically whenever changes are made.

---

A **pipeline** in software development is an automated series of steps that are followed to take code from development to production. Each step in the pipeline involves specific tasks, such as building, testing, and deploying the code.

---

CI/CD stands for **Continuous Integration** and **Continuous Deployment** (or **Continuous Delivery**). It's a set of practices used by software developers to automate the process of building, testing, and deploying software. Here's a breakdown:

1. **Continuous Integration (CI)**: Developers frequently integrate (or "merge") their code into a shared repository. Each time code is added, automated tests are run to check for errors or bugs. This helps catch issues early, making it easier to fix them.

2. **Continuous Delivery (CD)**: After code is tested and verified in the CI phase, it is automatically prepared for deployment to production. This means that the code is always in a deployable state and can be released to users at any time.

3. **Continuous Deployment (CD)**: This takes CD a step further. Instead of just preparing the code for deployment, it's automatically deployed to the production environment without manual intervention.

In short, CI/CD helps developers work faster and with more confidence by automating the process of testing and deploying code.

---

**important stages** in a typical CI/CD pipeline :

1. **Code Commit**: 
   - A developer writes code and commits (saves) it to a repository like GitHub. This is the starting point for the pipeline.

2. **Build**: 
   - The code is compiled or packaged into an executable form. This ensures the code is structured and ready to be run.

3. **Test**: 
   - Automated tests are run to check if the code works as expected. These tests help find bugs or issues early before the code is deployed.

4. **Deploy to Staging**:
   - The code is deployed (put onto a test server) where it can be tested in an environment similar to the real production environment.

5. **Acceptance Testing**: 
   - This is the final check to make sure everything works correctly in the staging environment. It often includes user acceptance testing (UAT) where real users test the application.

6. **Deploy to Production**:
   - If everything passes, the code is deployed to the live production server, making it available to real users.

7. **Monitor**:
   - Once the code is live, it is monitored to make sure it’s running smoothly and no new issues arise.

In short, the pipeline ensures that code is built, tested, and deployed automatically, with checks at each stage to make sure everything works correctly before going live.

---

Jenkins requires **Java** because it is built using Java. In simple terms:

- Jenkins is a **Java-based application**, meaning its core components and functionality are written in Java.
- To run Jenkins on your computer or server, you need to have **Java** installed because the Jenkins software depends on it to execute.
- Java provides the necessary tools and environment for Jenkins to work, just like how certain apps require specific programs (like a web browser or database) to run.

So, in short: **Jenkins needs Java to function** because Java is the programming language used to build it. Without Java, Jenkins won't be able to run.

---

![Output](https://i.imgur.com/KU5U3Eu.png)
![Output](https://i.imgur.com/bbSFAzS.png)
