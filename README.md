# 🎓 FPT GPA Calculator

**Author:** cattillallnight
**Language:** English
**Purpose:** To calculate the cumulative GPA for FPT University students accurately and easily.

---

## 💡 Features

* **Two calculation modes:**

  1. **Manual Input Mode:**
     Enter each course manually with course name, credits, and 10-scale grade.
     Optionally list *conditional courses* (e.g., MAS291, LAB211) that will be excluded from GPA.
  2. **Paste Transcript Mode:**
     Paste your transcript lines in this format:

     ```
     Semester:Course:Credit:Grade:Status
     ```

     Example:

     ```
     Fall2025:IOT102:3:9.1:Passed
     Summer2025:CSD201:3:8.6:Passed
     Summer2025:MAS291:3:Studying
     ```

     The calculator automatically:

     * Counts only courses with `Passed` status
     * Excludes `ENT`, `VOV`, `GDQP`, and `OJT` courses
     * Excludes any *conditional courses* listed by the user

* Calculates both:

  * **10-point GPA (official FPT scale)**
  * **4-point GPA (international conversion)**
  * Provides classification: *Excellent, Very Good, Good, Fair, Average, Fail*

* **Dynamic interface:** Switch freely between Manual Input and Paste Transcript modes.

* **Responsive design:** Works on both desktop and mobile browsers.

---

## 🧮 How GPA is Calculated

**Formula:**

```
GPA = (Σ (course_grade × course_credit)) / (Σ course_credits)
```

**Exclusions:**

* English foundation (ENT), Physical Education (VOV), Military Training (GDQP), Internship (OJT)
* Conditional or graduation-required courses defined by the user

---

## 🧾 GPA Conversion Table (FPT Official)

| 10-Scale | 4-Scale | Classification   |
| -------- | ------- | ---------------- |
| 9.0–10.0 | 4.0     | Excellent (A+)   |
| 8.5–8.9  | 3.75    | Very Good (A)    |
| 8.0–8.4  | 3.5     | Good (A-)        |
| 7.5–7.9  | 3.25    | Fairly Good (B+) |
| 7.0–7.4  | 3.0     | Fair (B)         |
| 6.5–6.9  | 2.75    | Average+ (B-)    |
| 6.0–6.4  | 2.5     | Average (C+)     |
| 5.5–5.9  | 2.25    | Average- (C)     |
| 5.0–5.4  | 2.0     | Pass (C-)        |
| < 5.0    | 0.0     | Fail (F)         |

---

## 🧑‍💻 How to Use

1. Open `index.html` in any modern browser.
2. Choose a calculation mode:

   * **Manual Input:** Add courses one by one.
   * **Paste Transcript:** Paste transcript data following the format.
3. Enter conditional courses (if any) separated by commas.
4. Click **📊 Calculate GPA**.
5. View your GPA (10-scale, 4-scale) and classificatio
