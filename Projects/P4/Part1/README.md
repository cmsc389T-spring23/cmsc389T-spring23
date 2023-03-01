# Project 4: PacMan CI

Part 1: Actions and Sabotage

Due: 03/15, 11:59pm

## Before You Start

Make sure you have completed the PacMan project before you start this project.

**This project will require collaborating among at least 8 people**. Some key initial steps to take are,

- Create cards for Sections 1 and 2 and assign deadlines. 
  - Add these deadlines on your cards on your Kanban Board to make them visible to the entire team 
- Create a Slack channel to communicate with your partner team(s).

## Team Pairings

- Teams 1 and 3
- Teams 2 and 4
- Teams 5 and 7
- Teams 6, 8, and 10
  - Team 6 will fork Team 8
  - Team 8 will fork Team 10
  - Team 10 will fork Team 6
- Teams 9 and 11
 
## Introduction

**READ THE BEFORE YOU START SECTION BEFORE CONTINUING** 

In this project, you will adding Continous Integration pipelines to your PacMan project. This project has three sections:

- GitHub Actions - FTR-actions
- Sabotage - FTR-sabotage
- Notify Your Partner Team - Slack 

## Section 1: GitHub Actions

**Only one person** from each team needs to take the following steps:

1. Create 2 Feature branches: FTR-actions, FTR-sabotage 
2. Create a feature-item actions-setup for the main.yaml file 
3. Add a main.yml file to your feature-item that uses the openjdk image and compiles all of your files
4. Create a pull request, add a reviewer, and have the reviewer merge the feature-item to FTR-actions

Once the steps above have been completed, you should be able to see a workflow show up on the Actions tab on GitHub. Now that the project is configured to work with GitHub Actions, each team member should

6. Create a feature-item branch actions-name_of_member
7. Modify the main.yml file to include a job for each test that you wrote
8. Create a pull request, add a reviewer, and have the reviewer merge your feature-item to FTR-actions

Once all feature-items have been completed

9. Submit a pull request to merge FTR-actions with the main branch
10. Add all group members as reviewers
11. Once the merge is complete, you should be able to see all of your jobs passing on the Actions tab

**Note** Your tests must run be able to run headless (i.e. without a Java Display). Make sure to include the ```-Djava.awt.headless=true``` flag when running tests both locally and on Actions. You should also use the **NoFrame** class instead of the MainFrame class to avoid a ```java.awt.HeadlessException```. It has the same functionality as MainFrame but it doesn't create a JFrame for the display.

**Once you have completed this FTR as a team, there should be 13 jobs (1 compile job and 12 test jobs) in the main.yml file.**

## Section 2: Sabotage

<p align="center">
<img src="https://i.redd.it/n0cz029px3q51.jpg"/>
</p>

1. Checkout a new branch from the FTR-sabotage feature branch that is titled with sabotage-your_name
2. Change your function so that it will fail the test you wrote previously. **Do not change the test.**
3. Create a pull request, add a reviewer, and have the reviewer merge your feature-item to FTR-sabotage
 
**Any 'mistakes' that you have intentionally made MUST be reversible**

Once the steps above have been completed, your team should

4. Submit a pull request to merge FTR-sabotage with the main branch
5. Add all group members as reviewers
6. Once the merge is complete, check that all of your jobs for tests are now failing on the Actions tab and that your compilation job still passes

## Section 3: Notify Your Partner Team

Once you have completed the Actions and Sabotage FTRs, notify your partner team or the team that is forking your repository.
They can now move on to the next part of the project.
Once your team has been notified, please move on to the next part of the project.

## Academic Integrity

Please **carefully read** the academic honesty section of the course syllabus. **Any evidence** of impermissible cooperation on projects, use of disallowed materials or resources, or unauthorized use of computer accounts, **will be** submitted to the Student Honor Council, which could result in an XF for the course, or suspension or expulsion from the University. Be sure you understand what you are and what you are not permitted to do in regards to academic integrity when it comes to project assignments. These policies apply to all students, and the Student Honor Council does not consider lack of knowledge of the policies to be a defense for violating them. Full information is found in the course syllabus, which you should review before starting.

