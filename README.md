# Event Recognition using PageRank

## What is this project
This project is an experiment to see if smart devices can automatically figure out what kind of event is happening in a group of photos. I used an algorithm called PageRank to find the most important photos in a group. If the computer can identify the most important photos, it can guess the event much faster.

## The Problem
We take thousands of photos on our phones but it is hard to organize them. The goal is to automatically label a group of photos without looking at every single one.

## How it works
1. Input: I fed the computer images using the CIFAR-10 dataset.
2. Comparison: The computer looked at colors and patterns to see which photos looked similar.
3. Ranking: The photos voted for each other. If a photo looked like many others, it got a high score using PageRank.
4. Selection: The computer picked the highest scoring photos to represent the whole group.
5. Guessing: It used those key photos to guess the object or event (like "Airplane").

## The Results
I compared my method against a random guess.
Random Guessing: 10% Accuracy
My PageRank Method: 20% Accuracy
My method is twice as good as random guessing. It worked best on things with clear shapes like Trucks and Airplanes but struggled with animals like Cats and Dogs because they move around a lot.

## Tools I Used
Python
PageRank Algorithm
CIFAR-10 Dataset
Scikit Learn

## How to Run
1. Open the Notebooks folder.
2. Run task2_dataset_analysis.ipynb to see the data visualizations.
3. Run task3_proof_of_concept.ipynb to see the PageRank algorithm in action.

Created by: Fariha Tanha (Student ID: 22101296)
Course: CSE449
