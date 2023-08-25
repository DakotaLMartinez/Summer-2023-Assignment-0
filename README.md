# Assignment 0

## Preface

In order to get up and running and to set up the environment (both local and remote) for Assignment-0, a lot of credentials have to be filled out and a lot of software has to be installed. We will briefly introduce some of this software for this assignment but we will have more time to concentrate on it throughout the course​.

This README is not designed to be a comprehensive introduction into all of the topics covered​ but will provide just enough information to move forward to the next slide/step, and, by doing this in this​ piecemeal manner, we reach the primary objective of being in a position to finally work on Assignment-0 in a carefully expedited fashion​

In addition, if any resources are shared via hyperlinks to official documentation and professional​ resources, it is important to step through them for further reference.

## Agenda

- [Overview of Assignment 0](#overview-of-assignment-0)
- [GitHub](#github)
- [Git](#git)
- [NodeJS and Node Package Manager (NPM)](#nodejs-and-node-package-manager-npm)
- [Testing](#testing)
- [Walkthrough and Logistics of Assignment 0](#walkthrough-and-logistics-of-assignment-0)
- [Submitting Your Assignment](#submitting-your-assignment)
- [Assignment 0 Problems](#assignment-0-problems)
- [Complete Environment Setup](#complete-environment-setup)

## Overview of Assignment 0

- One of the core parts of the prework, this assignment provides opportunities to become more familiar with JavaScript commands, JavaScript syntax, and unit testing with JavaScript while also improving problem-solving skills​

- This assignment is composed of twenty prompts (Problems 00 to 19) that will put your understanding of fundamental string interpolation, string manipulation, mathematical operations, loops, objects, arrays, recursion, rest parameters, sets, classes into practice​

- This assignment will also serve as an introduction to reading and running unit​ tests​

- Prior to reading any prompts and writing out any solution code, this assignment provides a timely opportunity to coordinate and set up GitHub and Git, which will be critical in practicing fundamental git commands on the terminal, independently developing a git workflow, and getting more exposure to distributed version control systems​

- This assignment also affords us the opportunity to download and install NodeJS, Node Package Manager (NPM), and Unit Testing Libraries (Mocha, Chai, Sinon) so that everyone follows along throughout the course with the same materials as soon as possible

## GitHub

- GitHub, Inc. is a United States-based global company that provides hosting​ for software development version control using Git​

- GitHub, Inc is a subsidiary of Microsoft, which acquired the company in 2018​ for US $7.5 billion​

- More than 2.9 million businesses and organizations use GitHub

- Touted as the world's leading software development platform, GitHub brings together the world's largest community of developers to discover, share, and build better software​

- You need to, if you haven’t already, register for an account with GitHub so that you can:​
  - have a portfolio site to host and showcase our projects​
  - access a platform that allows you to host and review code​ use project management tools​
  - be exposed to repositories of open-source software from as many as 50 million fellow developers​
  - access Assignment 0 from the original repository​
  - Fork the Assignment 0 repository to your own personal GitHub account​

### Signing up to GitHub

1. Navigate to <https://github.com/>​

2. Click on "Sign Up"​

    a)  Provide a username​

    b)  Provide an email address​

    c)  Provide a password​

    d)  Verify the account (if prompted)​

    e)  Click on "Create Account"​
3. Fill out preferences and interests​

4. Verify email address​

5. ​Visit the repository for Assignment 0

    a) Click the Fork Repository button​

    b) Select your account as the owner​

    c) Click the Create Fork button​

    d) once forking is complete, the URL will look like this: https://github.com/yourGitHubUsername/Summer-2023-​Assignment-0​

    e) This is the URL you will use when you submit your assignment in Blackboard.

Now that you have successfully registered with GitHub, a web- based service and platform, it’s time to put that part on hold for now, and transition into: git

## Git

- Git is a free and open source distributed version control system designed to​ handle everything from small to very large projects with speed and efficiency​

- Its goals include speed, data integrity, and support for distributed, non-linear​ workflows​

- It is designed for coordinating work among programmers, but it can be used to track changes in any set of files​

- Every git directory on every computer is a full-fledged repository with complete history and full version-tracking abilities, independent of network access or a central server

- For our purposes, we need to, if we haven't already, download,​ install and configure git on our local machines so that we can:

    -   copy, or clone, git repositories (such as the git repository that houses the original Assignment-0)​

    - save, or commit, modifications we perform on our local copy of a project

    -   upload, or push, the changes made on our local copy of a project to the remote version of the project

    - perform other declarative actions and operations that we will cover later on in the course

### Installing Git

If you run the following command in your terminal and you don't get an error, you can skip this step:

```
git --version
```

### Installation Methods

Navigate to any of the links below, which serve as reliable, official, and general sources of truth when it comes to installing git in a variety of ways for different operating systems

- [https://www.atlassian.com/git/tutorials/install-git](https://www.atlassian.com/git/tutorials/install-git)

-  [https://git-scm.com/book/en/v2/Getting-Started-Installing-Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

- Note: Please record the method of installation you decided on for future reference

    - Note: You may need to close your terminal sessions and then re-open them for git to be in effect post-installation​

    -   Note: You may encounter situations where file restrictions and/or hidden files might need to be accessed \--\- troubleshoot accordingly and please ask for assistance if necessary!

There are multiple scenarios that could be encountered, but in the following content, we will step through one of the scenarios involving installing git on a machine running on macOS​

### Scenario and Instructions

#### Installing and Configuring Git on MacOS

1) You have a machine running macOS​

2) You have never installed git before on this machine​

3) If you type in the terminal `git --version`​
, you are met with a prompt that suggests you download Xcode in order to download the command line developer tools (if this is not the case, then you may already have git installed)​

4) After successfully downloading Xcode, you then type in the terminal `git --version` and you are met with something like this:​

    `git version 2.17.2 (Apple Git-113)​`

5) You are now able to set some credentials which will be associated with any git- related activity and interaction you perform on your terminal​

      a) git config --global user.name "John Carl" ​

      b) git config --global user.email "emailAddressUsedWithGitHubToBeConsistent@gmail.com”​

      c) If you come across something like: “John Carl” committed 23 minutes ago, that is that user's config setting for `user.name` that is​ used to identify and associate the user with that particular commit​.

6) If you want to see the configuration settings, you can type in: `git config --list`​

7) Now would be an opportune moment to​ [create an ssh key pair and add it to your GitHub account](./ENVIRONMENT_SETUP.md#configuring-ssh-keys-for-github). This will allow you to interact with GitHub via your terminal without having to enter your email address and password each time.​

#### Cloning a Repository

1. Navigate to:​
https://github.com/CSI-Tech-Talent-Pipeline/Summer-2023- Assignment-0​

2. Click on the link to your fork of the repository​

3. Click on the green button with the text "Code"​

4. Copy the generated link (select SSH if configured, HTTPS if not)​

5. Go to your terminal, ensuring you are in the directory where you want to store your code, and run `git clone pasteURLHere`​

6. Change into that directory with the command​

    ```
    cd Summer-2023-Assignment-0
    ```

7. Afterwards, you can stage and save changes, executing `git add` and `git commit`​

    a) If you are not familiar with these commands, please consult this link:​ [https://www.atlassian.com/git/tutorials/saving-changes](https://www.atlassian.com/git/tutorials/saving-changes)

8. Once you have completed the assignment, run `git push` to share your solutions to your GitHub account​

9. You will paste the link to your fork of the repository on GitHub as your submission for Assignment 0 within Blackboard (detailed instructions to follow)

Now that you have successfully downloaded, installed, and configured git on your local machine, in addition to cloning the assignment, establishing a link to the remote repository, and pushing up the local copy, it’s time to transition into: NodeJS and Node Package Manager (NPM)​

## NodeJS and Node Package Manager (NPM)

- NodeJS provides support for the JavaScript programming language​

- NodeJS is open source and actively maintained by contributors all over the​ world​

- NodeJS runs the V8 JavaScript engine, the core of Google Chrome, outside of the browser, allowing NodeJS to be very performant​

- Brief Summary (for now): NodeJS is a free, open-sourced, cross-platform JavaScript run-time environment that lets developers write command line tools and server-side scripts outside of a browser​

### Node Package Manager (NPM)

- NPM, which is typically packaged with a NodeJS installation, is a package​ (module) manager for NodeJS​

  - If you are familiar with Python’s `pip` or Ruby’s `RubyGems`, then this is a similar construct​

- The main three components of NPM are: the website, the registry, the CLI​

- With NPM, a developer can:​
    - install packages locally and globally​
    - install, uninstall, and update dependencies​
    - publish and revise their own modules for other developers to incorporate in other codebases​
​
- The website www.npmjs.com hosts thousands of free packages to download​

- NPM is an ideal and ever-growing ecosystem and it’s free to use​

When working with Node.js on our local machine, we'll sometimes want to work with different projects we find on the internet that require different versions of Node.JS. In order to facilitate this, we can install a Node Version Manager package (NVM). This will allow us to manage multiple node installations on our computer to make switching between projects with different dependencies a breeze.
### Installing NVM

1. **macOS/Linux**:
    ```bash
    curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
    ```

   After installation, restart the terminal or run the following command to access `nvm`:

    ```bash
    export NVM_DIR="$HOME/.nvm"
    [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
    ```

2. **Windows**:
    - Download the installer from [here](https://github.com/coreybutler/nvm-windows/releases).
    - Follow the installation instructions.

3. Verify the installation:

    ```bash
    nvm --version
    ```

### Node

1. With `NVM` installed, you can install the latest stable version of node:

    ```bash
    nvm install node
    ```

2. Set the newly installed version as the default:

    ```bash
    nvm alias default node
    ```

3. Verify the Node and npm versions:

    ```bash
    node -v
    npm -v
    ```

Traditionally, JavaScript was only run in the browser, but now you have a way to execute JavaScript within the confines of your local machine!​

NodeJS will effectively allow you to execute `.js` files such as Assignment-0​ and NPM will allow you to incorporate external modules of code into your​ project so that you do not need to reinvent the wheel.

Now that you have successfully downloaded, installed, and configured both NodeJS and NPM in order to be able to execute JavaScript on your local machine and in order to streamline the installation of helpful packages, libraries, and modules of code, it’s time to transition into: testing​

## Testing

- Testing, a world of its own, is a key stage of the Software Development​ Lifecycle (SDLC)​

- ​There are many kinds of tests such as: acceptance tests, functional tests, A/B​ testing, automated testing, manual testing, TDD, BDD, and unit tests, etc​

- For now, we will concentrate solely on unit tests​

- ​Unit testing helps developers decide that individual units of the program are working as per requirements and are error-free​

- ​The libraries we will use for this assignment, courtesy of NPM, are Mocha, Chai, and Sinon

### Mocha 

- Mocha is a JavaScript test framework for NodeJS programs, featuring browser support, asynchronous testing, test coverage reports, and use of any assertion library (https://mochajs.org/)​

- Mocha is a feature-rich JavaScript test framework running on NodeJS and in the browser, making asynchronous testing simple and fun.​

- Mocha tests run serially, allowing for flexible and accurate reporting, while mapping uncaught exceptions to the correct test cases​.

- In Assignment-0, whenever you see a script involve `mocha` or some code​ that involves a `describe()` block or an `it()` block, then you are seeing Mocha code.

### Chai

- Chai is a Behavior-Driven-Development (BDD) and Test-Driven-Development (TDD) assertion library for NodeJS and the browser that can be delightfully paired with any JavaScript testing framework (https://www.chaijs.com/)​

- Chai has several interfaces that allow the developer to choose the most comfortable​

     - The chain-capable BDD styles provide an expressive language and readable style, while the​ TDD assert style provides a more classical feel​


- In Assignment-0, whenever you see code that looks like this:​

    ```js
    expect(functionToTest, customErrorMsgHere).to.equal(expectedOutput)​
    ```

    then you are seeing the Chai assertion library (its `expect()` function) in​ practice​

### Sinon

- Sinon is self-described as a collection of standalone test spies, stubs and​ mocks for JavaScript (https://sinonjs.org/)​

- Works with any unit testing framework​

- In Assignment-0, whenever you see code that involves what’s known as a spy (which can be used to test how many times a function was called, what kind of arguments were passed to that function, etc) such as: `sinon.spy(object, methodName)`, then Sinon is being utilized​.

Now that you have successfully been briefly introduced to Mocha, Chai, and Sinon from a bird’s eye view, it’s time to transition to the walkthrough and the logistics of this assignment​

## Walkthrough and Logistics of Assignment 0

- The purpose of Assignment-0 is to become more familiar with JavaScript syntax, JavaScript commands, problem-solving skills, and reading unit tests both as a file and in the terminal​

- The project consists of 20 directories, numbered from 00 to 19​

- Each directory is composed of three main files​

    - A `.js` file, where you will write out your possible solution to test against the test suite/test​ specs​ (This is the ONLY file in each directory that requires modification)

    - An `.md` file, where you will be able to view questions, prompts, and examples in natural​ language​

    - A `test.js` file, where you will be able to view specific test cases that form the bulk of the test coverage via unit testing and what the Mocha runner will evaluate​

- When you run `npm install` in your terminal, all necessary dependencies will be installed in a folder called node_modules​

As there are many ways to approach this assignment, the following are simply​

### Suggestions and Recommendations​

- When jumping into any directory, please read through the markdown (.md) file​ first, and then re-read it if need be​

- Here, you will understand the expected function signature, the business logic requirements of each function you write, and brief examples​

- It is also important to, then, review the test spec file and try to follow along with one `it()` block at a time, understanding everything in piecemeal but also as a system​

- Then, when you are ready, it is important to try to run the tests while you write your code so that you can ensure that the changes you make are having the intended effect​

- While reading through a markdown file (.md) and writing solution code in a JavaScript file (.js) are intuitive based on past experiences, reading the test specs file (test.js) and understanding how to execute the built-in scripts (in the package.json file) might be a new experience​

- To understand that last part, it might best to step through the flow of data:​

    - The code you write in the (.js) file will be the default export from that file​

    - In the test spec file (test.js) will access what you submit by importing that default export​

    - All of the tests will then run the function you wrote, and it will pass or fail​ based on the business logic contained within the body of your function​

    - All tests were previously tested with a working solution beforehand​

### Notes about the package.json file and node_modules

In addition to all of those considerations, it is important to be aware of how to execute the tests (which, due to the --watch flag, will “watch” for real-time changes until the process is killed and re-execute/reload the watched files)​

You can navigate to the “scripts” key within the `package.json` file, a file that allows us to add custom-made scripts, provide metadata of our project, and install libraries via NPM based on the dependencies listed here.​

On that note, you will have to run the command `npm install` to populate the node_modules directory after you `cd` into the project directory. None of the test scripts (or any other scripts for that matter) will run properly until you have completed `npm install` command​

This is necessary because the `node_modules` directory is typically not tracked by git (it is `.gitignore`d) because it is a memory-intensive resource to both upload and download. The `package.json` file specifies which libraries (and which versions of those libraries) your project depends upon​. Those dependencies are installed within the `node_modules` directory when you run `npm install`.

PLEASE NOTE: Now that you’ve seen that, you will now know where the script commands originate from when you type them into the terminal such as: `npm run test` to run all of the tests or `npm run test-17` to run just the tests for problem 17​

- This was done in case running all of the tests becomes unreadable or difficult to read​

- Since these are unit tests, each problem is isolated and anthological --- no module whatsoever​ depends on another from another directory in order to succeed or fail in and of itself​

## Submitting Your Assignment

- Here is how you will submit not just Assignment-0 but all Assignments and Projects (unless otherwise stated) for the entirety of the course​

- Be sure to pass most of, if not all, the test specs as that will be the grade we record for you when the instructional staff clones your repository and runs the code​

To submit Assignment 0:

1.  [Log in to Blackboard](https://ssologin.cuny.edu/cuny.html?resource_url=https%3A%2F%2Fbbhosted.cuny.edu%252F).​

2.  Go to [Tech Talent Pipeline Full Stack](https://bbhosted.cuny.edu/webapps/blackboard/content/listContent.jsp?course_id=_2267876_1&content_id=_75836936_1&mode=reset) [Web Development Bootcamp 2023](https://bbhosted.cuny.edu/webapps/blackboard/content/listContent.jsp?course_id=_2267876_1&content_id=_75836936_1&mode=reset).​

3.  Click on the binder that reads TTP Full Stack Bootcamp at the top of that page​

4.  Click on "Assignment 0", click on the "Write Submission" button, paste the link to your Github repo in the text field and click submit

## Summary

- This entire process encompassed a lot (A LOT) of setup that will make sure we are all on the same page and that our credentials are set for certain tools and services​

- We briefly jumped into the world (just scratching the surface) of Git, GitHub, JavaScript, NodeJS, NPM, Mocha, Chai, Sinon, and much more​

- Thanks to git, we can both track (this history will be helpful to us down the road if we ever want to rollback by a `revert` or `reset` command) and make modifications to Assignment-0​

    - Thanks to git, we were able to clone down Assignment-0 from the original repository (TTP) and then upload it to our own personal repositories​

    - As an aside, we could have used `fork` and then cloned that down, but there’s time for that later​

    - More on git later on in the course...and for the rest of your career in tech!​

- Thanks to GitHub, we (TTP) were able to host Assignment-0 and you were​ able to then host it on your own personal GitHub accounts​

    - Thanks to GitHub, we also virtually have a graphical user interface to better visualize our repositories as well as the histories of those repositories​

    - As an aside, it is important to distinguish that you can use git without GitHub and vice-versa​

- Thanks to NodeJS, we were able to execute all of the JavaScript involved in Assignment-0​

    - This is just the beginning as NodeJS will allow us to build out full-fledged servers that​ cooperate systematically with a database management system among other things​

- Thanks to NPM, we were able to import so much code and also execute helpful scripts to automate processes​

- Thanks to Mocha, Chai, and Sinon, we were able to have some semblance of​ robust and thorough test coverage within this contrived scenario​

## Taking Stock

- There is a lot of material that was mentioned and introduced, but here is a list​ to check off some potential takeaways to align expectations​

​- If you are in a place where you are aware that JavaScript on the browser (console/frontend) is different (due to environment) from JavaScript on a local machine (server-side/backend), even though it is the same language, then you are in a good place at the moment (we will cover this in more detail throughout the course) (all thanks to NodeJS!)​

​- If you are in a place where you are aware that NPM exists and it helps us bring in entire directories of files (see: node_modules) so that we can import production-level code into our own personal projects, then you are in a good place.

- If you are in a place where you feel a bit more comfortable with reading and executing test specs, and using those test specs to shape your solution code, then you are in a good place​

    - Testing frameworks (Mocha), assertion libraries (Chai), and libraries like Sinon are not the only​ libraries out there to help with testing​

        - These are specific implementations of an overarching concept, and so while it might be overwhelming to encounter hundreds of different libraries, understanding a few will yield transferable knowledge and transferable skills, a recurring theme of the entire course​

- While all of that will be crucial by the end of the course, this (Assignment-0) is primarily designed to improve familiarity with JavaScript syntax, JavaScript conventions, JavaScript commands, and problem-solving skills --- so if you feel that you are getting the hang of it, and all of your accounts/credentials are set, then you have likely made significant progress at this point (more practice is encouraged)​

## Assignment 0 Problems

* 00-greetFriend
* 01-titleCaseEdit
* 02-subtractFive
* 03-cutInHalfAndFloor

* 04-countOfAllBooleans
* 05-countOfAllBooleansAndStrings
* 06-countOfAllNumbersSmallerThanTarget
* 07-countOfAllIndexMatchingNumbers

* 08-sumOfAllEvenNumbers
* 09-sumOfAllOddNumbers
* 10-sumOfNumsWithinARange
* 11-sumOfMinimumAndMaximum

* 12-fizzBuzz
* 13-isPalindrome
* 14-frequencyCounter
* 15-countDownSum

* 16-productOfAnyAmountOfNumbers
* 17-setUnionOfAnyAmountOfSets
* 18-pairSum
* 19-binarySearch

## Complete Environment Setup

You have installed some of the necessary dependencies that you will use throughout the course, but you have not installed all of the essentials yet! In order to make the most use of our class time together, please take the time to go through the [full Environment Setup guide](./ENVIRONMENT_SETUP.md) and make note of any installations that failed. We will go through any of those issues you had and fix them on Day 1, so be sure to go through the entire guide before then.