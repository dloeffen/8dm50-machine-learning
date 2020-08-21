
# Machine Learning in Medical Imaging and Biology (8DM50)
The course covers a number of machine learning methods and concepts, including state-of-the-art deep learning methods, with example applications in the medical imaging and computational biology domains.

This GitHub page contains all the general information about the course and the study materials. The **Canvas** page of the course will be used only for sharing of course information that cannot be made public (e.g. Microsoft Teams links), submission of the practical work and posting questions to the instructors and teaching assistants (in the Discussion section).

## Hybrid schedule due to the coronavirus pandemic
The 2020 edition of the course will be given in a hybrid manner combining on-campus and on-line education. We have a limited capacity for around 30-35 students to attend the lectures on-campus. The lectures will also be streamed on-line via Microsoft Teams for the students that want to attend remotely.

Because the room capacity is less than the number of students that registered for the course, you will have to subscribe to attend a lecture on-campus. The details about how to do this will be posted on Canvas.

The schedule is as follows:
* **Lectures**, *time*: Mondays 13.30 - 15.30, *location*: Atlas - 1.210 and on-line via Microsoft Teams (the link will be shared on Canvas)
* **Practical work**, *time*: Mondays 15.30 - 17.30, *location*: on-line via Microsoft Teams (the link will be shared on Canvas)

Since the practical sessions are immediately after the lectures, if you attend the lectures on-line you might not have sufficient time to travel home for the practical session. The University is working on ensuring that there are sufficient number of safe workspaces on-campus so that you can log in from there.

## Practical work on-line

The practical work, a.k.a. guided self-study (*begeleide zelfstudie*), will be done in groups. The groups will be formed in Canvas and you will also submit all your work there (check the Assignments section for the deadlines). Your are expected to do this work independently with the help of the teaching assistants. Each group will be assigned a teaching assistant that you can contact via Microsoft Teams during the practical sessions (the details and links will be posted in Canvas). You can also post your questions in the Discussion section in Canvas at any time (i.e. not just during the practical sessions).

# Materials

## Books
The lectures are mainly based on the selected chapters from following two books that are freely available online:

* [Deep Learning](https://www.deeplearningbook.org/), Ian Goodfellow and Yoshua Bengio and Aaron Courville
* [Elements of Statistical Learning](https://web.stanford.edu/~hastie/ElemStatLearn/), Trevor Hastie, Robert Tibshirani, Jerome Friedman

Additional reading materials such as journal articles are listed within the lecture slides.

## Software

The practical assignments for this course will be done in Python. To get started with setting up a Python environment, follow the instructions in the [Essential Skills](https://github.com/tueimage/essential-skills/python-essentials) module.

In addition, you have to install the packages `matplotlib`, `jupyter`, `scikit-learn`, `scipy`, `pandas` and `tensorflow-cpu`. It is recommended to install these packages in a separate Conda environment. A Conda environment is a directory in which you can install files and packages such that their dependencies will not interact with other environments, which is very useful if you develop code for different courses or research projects. If you want to know more about how to use Conda, read the [docs](https://docs.conda.io/projects/conda/en/latest/user-guide/getting-started.html).

To create a new Conda environment and install the required packages, run the following commands from the Anaconda Prompt application.

````bash
conda create --name 8dm50 python=3.6				# create a new environment called `myenv`
conda activate 8dm50						# activate this environment
conda install matplotlib jupyter scikit-learn scipy pandas tensorflow	spyder # install the required packages
````
Note that you have to activate the `8dm50` environment every time you start working on the assignments. In order to start Jupyter Notebook type `jupyter notebook` in Anadonda Prompt (after activating the `8dm50` environment with `conda activate 8dm50`). It is best if you change directory to the directory containing the code before starting Jupyter Notebook. Similarly, you can start the Spyder integrated development environment by typing `spyder` in the Anaconda Prompt.

For the practicals, you have to work as a group on the same code. Things are further complicated this year because you will likely not be able to meet in person and have to work remotely. While it is not essential, using `git` can make thing easier. The [Essential Skills](https://github.com/tueimage/essential-skills/blob/master/version-control-with-git.md) module also contains a section on `git` basics.

````bash
# first, you have to go to https://github.com/tueimage/8dm40-machine-learning and fork
# the 'official' course repository by clicking 'fork' in the top right corner
# of the page

# then, make a local copy of your fork (note that you will have to replace the username mitkovetta with your own)
git clone https://github.com/mitkovetta/8dm40-machine-learning.git

# change the working directory to the repository
cd 8dm40-machine-learning

# add the 'official' course repository as upstream
git remote add upstream https://github.com/tueimage/8dm40-machine-learning.git

# to pull from the forked student version (e.g. to get updates pushed by other group members):
git pull

# to pull from the 'official' course repository (e.g. in case some assignments have been updated):
git pull upstream master
````

## Assignments and Lectures

**IMPORTANT**: All materials tagged with (*tentative*)  are not updated from the previous edition of the course and might change for this edition. However, any changes made will not be substantial and you can still use the materials to get an early peek at the content.

* (*tentative*) [Introduction slides](lectures/intro.pdf)

### Reading assignment
* (*coming soon*) Instructions

### Machine learning fundamentals I
* (*tentative*) [Lecture slides](lectures/week_1.pdf)
* (*tentative*) [Practical work](practicals/week_1.ipynb)

### Machine learning fundamentals II
* (*tentative*) [Lecture slides](lectures/week_2.pdf)
* (*tentative*) [Practical work](practicals/week_2.ipynb)

### Linear models
* (*tentative*) [Lecture slides](lectures/week_3.pdf)
* (*tentative*) [Practical work](practicals/week_3.ipynb)

### Deep learning I
* (*tentative*) [Lecture slides](lectures/week_4.pdf)
* (*tentative*) [Practical work](practicals/week_4.ipynb)

### Deep learning II
* (*tentative*) Lecture slides [part 1](lectures/week_5_1.pdf) and [part 2](lectures/week_5_2.pdf)
* (*tentative*) [Practical work](https://colab.research.google.com/drive/1zLIAaGX8Z53YD8iR2FLNl8D-CXaQBTX-) @ Google Colab

### Support vector machines, random forests
* (*tentative*) [Lecture slides](lectures/week_6.pdf)
* (*tentative*) [Practical work](practicals/week_6.ipynb)

### Unsupervised machine learning
* (*coming soon*) Lecture slides
* (*coming soon*) Practical work

# Course information

## Learning objectives

After completing the course, the student will be able to:
* Recognise how machine learning methods can be used to solve problems in medical imaging and computational biology.
* Comprehend the basic principles of machine learning.
* Implement and use machine learning methods.
* Design experimental setups for training and evaluation of machine learning models.
* Analyze and critically evaluate the results of experiments with machine learning models.

## Assessment

The assessment will be performed in the following way:

* Work on the practical assignments: 25% of the final grade (each assignment has equal contribution);
* Reading assignment: 10% of the final grade;
* Final exam: 65% of the final grade.

Intermediate feedback will be provided as grades to the submitted assignments.

The grading of the assignments will be done per groups, however, it is possible that individual students get separate grade from the rest of the group (e.g. if they did not sufficiently participate in the work of the group).

## Instruction

The students will receive instruction in the following ways:

* Lectures;
* Guided practical sessions;
* Contact hours with the project instructors for questions, assistance and advice;
* Online discussion (in Canvas, see below).

Course instructors:
* Mitko Veta
* Federica Eduati

Teaching assistants:
* Suzanne Wetstein
* Oscar Lapuente Santana
* Yasmina Al Khalil


## Recommended preliminary knowledge

8DB00 Image acquisition and Processing, and 8DC00 Medical Image Analysis.

## Canvas

The [course page in Canvas] will be used for submission of the assignments, scheduling of the lectures and contact hours and announcements. The students are highly encouraged to use the Discussion section in Canvas. All general questions (e.g. issues with setting up the programming environment, error messages etc., general methodology questions) should be posted in the Discussion section in Canvas and not asked during the contact hours.



*This page is carefully filled with all necessary information about the course. When unexpected differences occur between this page and Osiris, the information provided in Osiris is leading.*
