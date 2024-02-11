---
title: Setting Up Personal Blog Website for Flipped Classroom Journals
sidebar:
  nav: docs-en
aside:
  toc: true
---

## Introduction
As a part of the module requirements, all students must create a personal blog website to document their flipped classroom experiences and insights.

## Journals
Students are expected to compose reflective blog entries detailing what they have learned during the flipped classroom sessions. 

The evaluation criteria include the quality of content and language proficiency.

For this module, students are tasked with completing 12 journal entries corresponding to 12 flipped class sessions. 

This component contributes 10% towards the overall grade.

## Recommended Blog Site Template
While students have the flexibility to choose any blog site, we recommend utilizing the following blog starter repository for ease of setup:

### Chirpy Blog Starter Repository
- Access the template repository [Chirpy-starter](https://github.com/cotes2020/chirpy-starter).
- Follow these steps to set up your blog:

1. Navigate to the template repository.
   ![Template Repository](/blob/master/assets/images/repo-1.png)

2. Use the template and create a new repository.
   ![Create New Repository](/blob/master/assets/images/repo-2.png)

3. Name the repository as 'yourgithubusername.github.io'.
   ![Change Repository Name](/blob/master/assets/images/repo-3.png)

4. Clone your repository.
   ![Clone Repository](/blob/master/assets/images/repo-4.png)

### Next Steps
```javascript
$ git clone //Your repo link
```

### Install Ruby(Mac)

```javascript
$ brew install ruby
```
### Install Ruby(Linux)

```javascript
$ sudo apt-get install ruby-full
```

### After Installation
```javascript
$ cd repo_path
```
Go to config.yml file in the root of the directory and the following details.

![Use the template](/blob/master/assets/images/repo-5.png)

```javascript
$ bundle
```
### Push Changes to Github

```javascript
$ git add .
```
```javascript
$ git commit -m "first-commit"
```
```javascript
$ git push
```

### Add website link to VLE

After deploying the website, add the website link to the database setup for the module on VLE.

Add your website link as an entry to the database on VLE.
