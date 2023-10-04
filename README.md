# AskMe - Question and Answer Platform

AskMe is a simple question and answer platform where users can ask questions, answer questions, and engage in discussions within threads. This README provides an overview of the project, its features, and a guide on how to set it up and use it.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Design](#design)
- [Usage](#usage)

## Introduction

AskMe is a file-based system that allows users to interact with a question and answer platform. Every time a user runs AskMe, they will see the previous state of the platform, including users, questions, and answers. Multiple users can use the platform in parallel, allowing for real-time interactions.

### User Authentication

- Users can sign up with their name, email, password, and username.
- Users can also choose whether to allow anonymous questions.

### User Operations

- **Print Questions**: Users can view questions asked by them, questions asked to them, and feed questions from all users.
- **Ask and Answer Questions**: Users can ask questions and answer questions from others. The system supports threads, allowing multiple questions to be asked within the same thread.
- **Delete Questions**: Users can delete questions they have asked, which may also remove the entire question thread if it was initiated by them.

## Features

### File-Based System

- AskMe stores user data, questions, and answers in files.
- The system preserves the state of the platform across sessions.

### Threaded Questions

- Questions can be organized into threads, where new questions are related to an original question.
- Deleting an original question also removes the entire thread.

### Correctness

- Users can only perform actions related to their own questions.
- Users cannot remove questions asked to someone else.

## Design

- Each user is assigned a system-generated ID, which is used consistently for their questions.
- While system-generated IDs are used internally, user-friendly usernames are displayed on the site.
- Thread questions are organized hierarchically, with the original question serving as the parent for all subsequent questions within the thread.


## Screenshots

![App Screenshot](https://snipboard.io/wGcZN2.jpg)
