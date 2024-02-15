---
title: Setting Up Personal Blog Website for Flipped Classroom Journals
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
   
   <img src="https://raw.githubusercontent.com/palden518/DBS101.github.io/master/assets/images/repo_1.png" alt="template repository">

2. Use the template and create a new repository.
   
   <img src="https://raw.githubusercontent.com/palden518/DBS101.github.io/master/assets/images/repo-2.png" alt="create new repository">

3. Name the repository as 'yourgithubusername.github.io'.
   
   <img src="https://raw.githubusercontent.com/palden518/DBS101.github.io/master/assets/images/repo_3.png" alt="change repository name" width= 500 height = 400 >

4. Clone your repository.
   
   <img src="https://raw.githubusercontent.com/palden518/DBS101.github.io/master/assets/images/repo_4.png" alt="clone repository" width= 500 height = 400>

### Next Steps
#### Open terminal to enter the following commands:

```javascript
$ git clone //Your repo cloning link
```

#### After cloning
```javascript
$ cd repo_path
```
Go to config.yml file in the root of the directory and the following details.

<img src="https://raw.githubusercontent.com/palden518/DBS101.github.io/master/assets/images/repo-5.png" alt="use the template">


#### Push Changes to Github

```javascript
$ git add .
```
```javascript
$ git commit -m "first-commit"
```
```javascript
$ git push
```

### Opitional: To run website locally

- #### Install Ruby(Mac)

```javascript
$ brew install ruby
```
- #### Install Ruby(Linux)

```javascript
$ sudo apt-get install ruby-full
```
- #### Install ruby(Windows)

[Download installer](https://rubyinstaller.org/)

- #### Check if ruby is installed
```javascript
$ ruby -v
```
- #### build website locally(Execute this command only once to install dependencies!)
```javascript
$ bundle
```

- #### run website on local server
```javascript
$ bundle exec jekyll s
```

  - #### go to http://localhost:4000 or  http://127.0.0.1:4000 to view your website on local server

### Adding posts to your website

- #### You can also refer [chirpy docs](https://chirpy.cotes.page/posts/write-a-new-post/) to learn how to add posts on your website

#### Add a file with file name YYYY-MM-DD-TITLE.md under _posts folder

Your file should have the .md extension for you to use markdown.

In your case the date should be the date of your flipped class.

Title should be the your  module class and flipped class title, Example; DBS101_FlippedClass1

##### Example file name: 2024-02-12-DBS101_FlippedClass1.md


<img src="https://raw.githubusercontent.com/palden518/DBS101.github.io/master/assets/images/repo-post1.png" alt="add file with name">


#### Inside your file, your title, categories and tags should be defined

Your title should be DBS101 Flipped Class [Number]

Example:

Note: Do not omit the horizontal lines, they are important!!!

```javascript
---
Title: DBS101 Flipped Class 1
categories: [DBS101, Flipped_Class1]
tags: [DBS101]
---
```

#### Example file

<img src="https://raw.githubusercontent.com/palden518/DBS101.github.io/master/assets/images/repo-post2.png" alt="examplefile">


#### How your entry will look like on your website

##### Homepage
<img src="https://raw.githubusercontent.com/palden518/DBS101.github.io/master/assets/images/repo-post3.png" alt="examplefile">

##### Post page
<img src="https://raw.githubusercontent.com/palden518/DBS101.github.io/master/assets/images/repo-post4.png" alt="examplefile">

##### Categories Page

<img src="https://raw.githubusercontent.com/palden518/DBS101.github.io/master/assets/images/repo-post5.png" alt="examplefile">


### Tips!

- #### Change your profile name to your name! It should not show up as chirpy

- #### Use correct file naming conventions, your post should not say MyfirstPost like my demo, it should be your modulecode_FlippedClass{no.}

- #### Try customizing your website, read the instructions on chirpy website:
[chirpy website guide](https://chirpy.cotes.page/)

- #### Do not forget to push your changes on github else it will not be reflected on your website

### Journal Format

- #### Your journal should be in blog format; should follow a structure whereby you have a blog topic and paragraphs detailing what you did during your flipped class and what you have learned.
- #### You can refer vides on writing a blog.



### Add website link to VLE

After deploying the website, add the website link to the database setup for the module on VLE.

Add your website link as an entry to the database on VLE.

