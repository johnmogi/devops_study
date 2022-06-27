## CI/CD

[What is Continuous Integration]
{{Continuous Integration (CI) is a development practice where developers integrate code into a shared repository frequently, preferably several times a day.}}
make sure not to mix ci with c delivery

- CI is a method of chaining deployment to the staging or the dev environment.
meaning we allways obtain an updated code base for review purposes and testing / QA.
the code all the time gets pushed to stage and we can trouble shoot issues in advance.

[Why do we need Continuous Integration]
{{ Continuous Integration enables better transparency and farsightedness in the process of software development and delivery. It not only benefits the developers but all the segments of that company. These benefits make sure that the organization can make better plans and execute them following the market strategy.}}

to avoid merge hell, to reduce deploy times, to avoid downtime, to avoid unnecessary work.
from team work perspective and also testing perspective this cut into stages workflow is a must.


[What is Continuous Deployment/Delivery]
{{ Continuous integration serves the purpose of automating your builds. It’s the practice of merging code changes back into the main branch as quickly and as often as possible.}}

{{ In continuous delivery(CD), all code changes are automatically deployed to either a testing or production environment right from the build stage, which practically makes this process a direct extension of continuous integration.}}

{{ Continuous deployment (CD) takes the entire process of continuous delivery a step further by releasing every change that passes through the production pipeline directly to your clients. If an automated test fails, then the change will not be sent, but if everything checks out in testing, the changes are deployed automatically.}}

- continuous delivery is a process of deploying a software application to a production environment with a controlled "buffer" for the deployment.
-CONTINUOUS DEPLOYMENT is a process of deploying a software application to a production environment - at the end of the testing cycle with manual approvement. 

[Why do we need Continuous Deployment/Delivery]
{{ There's no human intervention, and only a failed test will prevent a new change to be deployed to production. Continuous deployment is an excellent way to accelerate the feedback loop with your customers and take pressure off the team as there isn't a "release day" anymore.}}

to reduce build times, to achieve an "organic" enviroment that can quickliy revcieve new updates, from bug fixes and new features.

[Difference between Continuous Deployment and Continuous Delivery]
{{ Continuous Delivery is the automation of steps to safely get changes into production. Where Continuous Deployment focuses on the actual deployment, Continuous Delivery focuses on the release and release strategy. An elusive goal would be a “push of a button” to get changes into production.}}

continues delivery sends out our code instantly to the staging environment.
while continous deployment makes us stop and test and manually approve changes after testing for the production environment.

[Main Tools for CI/CD]
{{Tools to Consider · 1. Jenkins · 2. TeamCity · 3. CircleCI · 4. Travis CI · 5. Bamboo · 6. GoCD · 7. CodeShip · 8. GitLab CI. }}
git actions, azure devops, jenkins and others as well

## Azure DevOps Pipelines

[Azure DevOps Overview]
{{ Azure DevOps provides developer services for allowing teams to plan work, collaborate on code development, and build and deploy applications. Azure DevOps supports a collaborative culture and set of processes that bring together developers, project managers, and contributors to develop software.}}

- Azure DevOps is a cloud-based software development platform that provides a unified view of the development lifecycle.

[Build Pipelines]
{{ Azure Pipelines automatically builds and tests code projects to make them available to others. It works with just about any language or project type. Azure Pipelines combines continuous integration (CI) and continuous delivery (CD) to test and build your code and ship it to any target.}}

- Azure DevOps provides a set of build and release pipelines that can be used to build, test, and deploy your software.

[Azure Artifacts]
{{ Azure Artifacts enables developers to share their code efficiently and manage all their packages from one place. With Azure Artifacts, developers can publish packages to their feeds and share it within the same team, across organizations, and even publicly.}}

- Azure DevOps provides a set of artifacts that can be used to track the progress of your build and release pipelines.

[Release Pipelines]
{{ Azure Pipelines releases can deploy artifacts produced by a wide range of artifact sources. such as Azure Pipelines build, Jenkins, or Team City. Define the release pipeline using stages and restrict deployments into or out of a stage using approvals. Define the automation in each stage using jobs and tasks.}}
release pipelines are a set of build and release pipelines that can be used to build, test, and deploy your software.

[Build Agents]
{{ To build your code or deploy your software using Azure Pipelines, you need at least one agent. As you add more code and people, you'll eventually need more. When your pipeline runs, the system begins one or more jobs. An agent is computing infrastructure with installed agent software that runs one job at a time.}}
- Azure DevOps provides a set of build agents that can be used to build your software.

[Task Groups]
{{ A task group allows you to encapsulate a sequence of tasks, already defined in a build or a release pipeline, into a single reusable task that can be added to a build or release pipeline, just like any other task.}}
 - Azure DevOps provides a set of task groups that can be used to build your software.

[Libraries]
{{ A library is a collection of build and release assets for an Azure DevOps project. Assets defined in a library can be used in multiple build and release pipelines of the project. The Library tab can be accessed directly in Azure Pipelines. The library contains two types of assets: variable groups and secure files.}}
- Azure DevOps provides a set of libraries that can be used to build your software.

[Yaml Pipelines]
{{ Overview. Many teams prefer to define their build and release pipelines using YAML (YAML Ain't Markup Language). This allows them to access the same pipeline features as those using the visual designer, but with a markup file that can be managed like any other source file. }}
- Azure DevOps provides a set of yaml pipelines that can be used to build your software.
