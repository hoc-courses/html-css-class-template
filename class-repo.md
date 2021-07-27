# Curriculum Management Overview

The goal is to create a management system for the ongoing delivery of curriculum across a range of courses. For this discussion I'm going to limit it to a single sample course, HTML/CSS, and what the setup would be for the delivery of this course.

## Master Repositories
We need a series of repositories for storing the master copy of various resources we need for teaching. 

#### Course Reading Material
Currently I am using Gitbook to store this material. It only contains the core curriculum for the course. For example, software installation, Git/GitHub introduction, etc. should not be included here. They are included in the shared resources repo.

[HTML/CSS Gitbook](https://chnn-anne.gitbook.io/html-css/)

#### Shared Resources
These are a collection of Markdown files covering various topics that are common across course. For example:
* software installation
* Git/GitHub topics
* Terminal/CLI Intro
* VS Code Intro/Config
* GitHub Classroom Intro

[Share Resources Repo](https://github.com/hoc-courses/shared-resources)

#### Labs
Labs are what are assigned to students through GitHub Classroom. The teacher gives the students a link provided by GitHub Classroom, and when they enter it in browser a repo for the lab assignment will be created for them. The student assignment repos are all stored in the GitHub Classroom organization, not the students' GitHub account. That way, the distribution/collection is simplified and the instructor can see and give feedback on them easily.

Each lab has two repositories: starter and solution. The starter lab is what is assigned to the students. It contains a README file with the instructions for the lab, as well as any starter files needed.

The solution lab is for the instructor to review the lab before class, and possibly start the lab during class with the students. 

[Labs Repo](https://github.com/hoc-labs)

#### Demos
Demos are available for instructors to use during class to introduce new topics. Each demo has a README file overviewing the demo and any files needed.

[Demos Repo](https://github.com/hoc-demos)

#### Instructor Course Guide
A set of Markdown files overviewing the modules for the course and the labs,demos available.

[Instructors' Guide Repo](https://github.com/hoc-courses/html-css-instructor-guide#readme)

**TODO:** Ideally, we would eventually create a class-by-class guide for what should be covered, referencing the course material, demos, and labs. This requires agreeing on what content should be covered, the pace, etc.

#### Class Instance Repo
At the beginning of each class run the instructor would create a class repo. The repo is read-only to students, but writable by the instructor.

It consists of a few Markdown pages for class mechanics:
* [course info page](https://github.com/hoc-courses/html-css-class-template): instructor info, schedule, contact info, etc.
* link to course reading material (Gitbook)

It also is used for the sharing of class lecture material with the students. For each class, the instructor would create a new folder in the repo and that folder would be populated with the following:
* [overview of class](https://github.com/hoc-courses/html-css-class-template/tree/main/class-01#readme)
* class notes, links to lab assignments
* demo code copied from master repo and modified during class
* lab code copied from master repo and started during class

At the end of the class, the instructor would push the changes to the class repo (the demo and lab code, class notes) and students would then be able to pull the latest changes.




