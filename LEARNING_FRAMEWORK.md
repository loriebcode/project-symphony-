# 📘 Part 1: Instructional Design & User Learning Framework

A strategy is only helpful if your team knows how to use it. This framework ensures that any recruiter can set up their workspace and run their first candidate batch in less than 3 minutes.

---

## 1.1 User Learning Matrix

We designed this tool to serve two very different types of users:

| User Type | Tech Skill Level | Main Goal | Biggest Hurdle |
| :--- | :--- | :--- | :--- |
| **Recruiting Team** | Low to Medium | Quickly check candidate resumes against core skills. | Fear of the command line; setting up software tools. |
| **System Engineers** | High | Keep the automated data pipeline running smoothly. | Dealing with messy resume text and unusual job titles. |

---

## 1.2 The 3-Minute Quick Start Guide

Follow these three quick steps to get your local screening tool up and running.

### Step 1: Set Up Your Workspace
Open your terminal application and paste these commands to download the project and create a safe, isolated workspace:
```bash
git clone [https://github.com/loriebcode/project-symphony-.git](https://github.com/loriebcode/project-symphony-.git)
cd project-symphony-
python -m venv venv
source venv/bin/activate
