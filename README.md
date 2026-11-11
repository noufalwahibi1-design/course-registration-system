# University Course Registration System

Java program that decides whether a student can register for a course, based on a discrete-math model (CS285 – Discrete Mathematics for Computing, Prince Sultan University, Term 261).

## Eligibility rule
A student is ELIGIBLE if all three hold:
1. All prerequisites completed — Prereq(c) ⊆ Completed(s)
2. At least one section has a free seat — ∃x ∈ Sec(c), enr(x) < cap(x)
3. Course not already completed — c ∉ Completed(s)

If not eligible, the program shows which condition failed and the missing prerequisites.

## Files
- `Student`, `Course`, `Section` – data classes
- `Registrar` – sample data and one method per model function (missing, prereqOk, available, eligible)
- `Main` – reads student ID and course code, prints the result (Q to quit)
- `TestCases` – 14 tests that print PASS/FAIL

## Run
javac *.java
java Main

## Team
Ghaida Aldali, Nouf Alwahibi, Rahaf Alhumaidi, Lamia Bin Jrais