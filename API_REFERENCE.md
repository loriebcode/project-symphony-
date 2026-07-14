# 📝 Part 2: Technical API Reference Guide

This document maps out the backend data structure for the candidate match engine. As a technical writer, my job is to clearly explain how data must look when moving through the system so software engineers know exactly what to build.

---

## 2.1 Endpoint: Evaluate Candidate Profiles

Processes a resume text block and checks it against a specific list of required skills.

*   **Method:** `POST`
*   **URL Route:** `/api/v2/talent/evaluate`
*   **Format:** `application/json`

---

## 2.2 Data Fields & Rules

| Field Name | Data Type | Required? | Default Value | Technical Rules & Constraints |
| :--- | :--- | :--- | :--- | :--- |
| `candidate_id` | String | **Yes** | *None* | Must be a unique, secure user ID string. |
| `raw_resume_text` | String | **Yes** | *None* | Plain text from the resume. Max 10,000 characters. |
| `skills_filter` | Array | No | `[]` | A list of specific skills you want to check for. |

---

## 2.3 Data Integration Examples

### Sample Data Request (Going In)
```json
{
  "candidate_id": "usr_99x_symphony",
  "raw_resume_text": "Experienced talent professional specializing in high-volume sourcing and Python-driven automation frameworks.",
  "skills_filter": ["Python", "Sourcing Strategy", "Technical Writing"]
}
