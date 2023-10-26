## Getting started with Jenkins

Mantaining a good order and a naming convention can help in making things easier to find and fix in the future. In this guide we'll learn how to create Jenkins Folders and Jenkins Jobs.<br/>
First we'll create a place to allocate our first Pipeline.
<br/>
<br/>

## Creating a Folder
There are few things as useful as a virtual Folder. In Jenkins likewise many other tools and OS we have the option to create Folders for specific purposes, where our pipelines will happily live.

### My First Folder
Once Jenkins is up and running on your machine click on the "New Item" option on the left hand panel.

![Jenkins New Item](/assets/images/newItem.png)
<br/>

Inside New Item screen we'll need to define a name (don't forget to use a naming convention) and Folder as type. Once those details are ready just click "Ok" button to finish.

![New Jenkins Folder](/assets/images/newFolder.png)
<br/>

As a result you'll find a brand new Folder to start working on it!

![Jenkins Folder Created](/assets/images/newFolderCreated.png)
<br/>

### My First Jenkins Job
For creating a Jenkins Job it's required to go to the desired location, for example inside a folder, and click on the "New Item" option. Inside New Item screen we have many options available but for now we'll focus on entering a descriptive name, select "Pipeline" option and finally click "OK". This will create a Pipeline Jenkins Job.

![New Jenkins Job](/assets/images/newJenkinsJob.png)
<br/>

Once the new Jenkins Job is created, a Configuration screen will automatically open. Inside it, is possible to set a description and make use of multiple options, but for now we'll focus on Pipeline section for the following two scenarios.

#### Pipeline script: 
This kind of pipeline allow us to write a script directly in Jenkins using Groovy Language. This is useful when we want agility during the process of writing this kind of scripts, but a huge disadvantage is that the codebox doesn't offer any help for coding.
</br>
Below it's shown a simple script. It defines a Pipeline with one Stage called `HelloWorld` that prints `First Hello World!` in the Console Output, using any available Jenkins agent for it.
![Pipeline Script](/assets/images/pipelineScript.png)
</br>

#### Pipeline script from SCM:
Jenkins offers another powerful way of pull scripts from Source Code Management (SCM) platforms, for example from GitHub. All we need to do to pull code from a public repository is fill the "Repository URL" input box, specify Branch Name and set the Jenkinsfile path from repository root folder.
</br>
For private repositories it will be required to configure credentials inside Jenkins system for to SCM platform authentication.
</br>
</br>
Configuring Repository URL:
![New Jenkins Job Repo](/assets/images/newJenkinsJobRepo.png)
</br>
</br>
Configuring Repo Branch and Jenkinsfile path:
![New Jenkins Job Branch and Jenkinsfile](/assets/images/newJenkinsJobBranchJenkinsfile.png)
</br></br>
After Jenkins job is configured don't forget to <strong>Apply</strong> and <strong>Save</strong> your changes.
</br>

### Now it's time to Build this first Jenkins Job!