# Mathematics Session 6 — Permutations and Combinations
> **Admission-test focus:** NUST NET + FAST/NUCES  
> **Session type:** Concept repair + fast revision  
> **Main goal:** Decide correctly whether a problem needs an arrangement or a selection, then count it without missing restrictions.

**Video reference:** [YouTube video supplied for this session](https://www.youtube.com/watch?v=Y1X_zLptX_E&t=31s)  
**Important source note:** The video page and captions were not accessible during preparation of this file. These notes therefore consolidate the permutations-and-combinations lesson and the revision gaps from our recent chat; they do not claim to be a verified transcript or a complete summary of the video's spoken content.

---

## 1. The 20-second idea

There are two different questions:

- **Permutation:** In how many ways can we arrange or order things?
- **Combination:** In how many ways can we select or choose things?

The only question you should ask first is:

**Does changing the order create a different result?**

- If **yes**, use permutation.
- If **no**, use combination.

### One simple example

Suppose there are 5 students: A, B, C, D, E. We need 2 students.

- Choosing A and B for a committee is the same as choosing B and A. This is a **combination**.
- Giving A first position and B second position is different from giving B first and A second. This is a **permutation**.

So:

\[
{}^5C_2 = \frac{5!}{2!3!}=10
\]

\[
{}^5P_2 = \frac{5!}{3!}=20
\]

There are 10 pairs, but 20 ordered arrangements.

**Memory line:** Selection = combination. Arrangement = permutation.

---

## 2. Factorial — the building block

Factorial means multiplying a positive integer by every positive integer below it.

\[
5! = 5\times4\times3\times2\times1=120
\]

Important values:

| n | n! |
|---:|---:|
| 0 | 1 |
| 1 | 1 |
| 2 | 2 |
| 3 | 6 |
| 4 | 24 |
| 5 | 120 |
| 6 | 720 |
| 7 | 5040 |
| 8 | 40320 |

Remember:

\[
0!=1
\]

Why? It makes the counting formulas work consistently. Do not treat \(0!\) as zero.

### Fast cancellation

Do not expand every factorial if terms can cancel.

\[
\frac{8!}{6!}=\frac{8\times7\times6!}{6!}=56
\]

\[
\frac{9!}{7!2!}=\frac{9\times8}{2}=36
\]

In NET questions, cancellation saves time and reduces arithmetic mistakes.

---

## 3. The two main formulas

### A. Permutation: order matters

Number of ways to arrange r objects selected from n different objects:

\[
\boxed{{}^nP_r=\frac{n!}{(n-r)!}}
\]

Use it when positions, ranks, seats, codes, or order are important.

**Example:** Arrange 3 students in 3 positions from 7 students.

\[
{}^7P_3=7\times6\times5=210
\]

Why? There are 7 choices for the first position, 6 remaining choices for the second, and 5 for the third.

### B. Combination: order does not matter

Number of ways to select r objects from n different objects:

\[
\boxed{{}^nC_r=\frac{n!}{r!(n-r)!}}
\]

Use it for teams, committees, groups, selections, and choosing questions when order does not matter.

**Example:** Select 3 students from 7 for a committee.

\[
{}^7C_3=\frac{7!}{3!4!}=35
\]

### C. The connection between them

\[
\boxed{{}^nP_r={}^nC_r\times r!}
\]

First select the r objects, then arrange those r selected objects in \(r!\) ways.

This is a very useful NET shortcut:

- Select a group: \(C\)
- Select and then arrange that group: \(C\times r!\), which is \(P\)

---

## 4. How to identify the correct method in an MCQ

| Words or situation | Usually use |
|---|---|
| Arrange, order, rank, first/second/third | Permutation |
| Seat people in numbered seats | Permutation |
| Make a number using digits | Permutation / place-by-place counting |
| Create a code or password | Permutation if positions differ |
| Select, choose, committee, team | Combination |
| Choose a group of questions | Combination, if order is irrelevant |
| Choose a team and appoint its captain | Combination, then choose the captain |

**Important:** Do not decide from one keyword alone. Ask whether swapping two selected items changes the result.

### Quick test

- AB and BA are the same committee → combination.
- AB and BA are different two-letter codes → permutation.

---

## 5. Fundamental counting principle

When a task has steps, multiply the number of choices at each step.

**Example:** A student has 3 shirts and 4 trousers. How many shirt-trouser outfits are possible?

\[
3\times4=12
\]

This is the same idea behind permutations.

### Addition rule

When a task can happen in separate, non-overlapping cases, add the cases.

**Example:** A digit may be selected from either a set of 3 red cards or a separate set of 4 blue cards. If the cases cannot overlap, total choices are \(3+4=7\).

### Remember the difference

- Different steps that all happen: multiply.
- Separate possible cases: add.

Many digit questions are solved by **splitting the final digit into cases**, then adding the valid counts.

---

## 6. Repetition: allowed or not allowed?

This is one of the most important details in counting questions.

### A. Repetition is not allowed

For r ordered positions filled from n different choices:

\[
\boxed{{}^nP_r=n(n-1)(n-2)\cdots(n-r+1)}
\]

Each used object is removed from the next position.

Example: 3-digit codes using digits 1–6 without repetition:

\[
6\times5\times4=120
\]

### B. Repetition is allowed

If every one of r positions can use any of n choices:

\[
\boxed{n^r}
\]

Example: 3-digit codes using digits 1–6 when repetition is allowed:

\[
6\times6\times6=6^3=216
\]

**Do not use \(n^r\) when repetition is forbidden. Do not use \(nP r\) when repetition is allowed.**

---

## 7. Number formation — the restriction checklist

Number-formation questions are arrangements with extra rules. Check restrictions in this order:

1. **How many places?** For example, a 4-digit number has thousands, hundreds, tens, and units places.
2. **Can zero be first?** No. A number cannot begin with zero.
3. **Is repetition allowed?** Read the question carefully.
4. **Must the number be even or odd?** Check the units digit first.
5. **Must it be divisible by 5 or 10?** Check the units digit.
6. **Are any digits fixed or forbidden?** Apply that restriction before counting the remaining places.

### Even and odd numbers

- An even number ends in 0, 2, 4, 6, or 8.
- An odd number ends in 1, 3, 5, 7, or 9.

For an even-number question, choose the last digit first. Then count the remaining positions.

### Example 1 — Four-digit even numbers from 0 to 9, no repetition

Digits available: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9.

Split into two cases.

**Case 1: Last digit is 0**

- Units place: 1 choice (0).
- First digit: 9 choices (1–9).
- Hundreds place: 8 choices remain.
- Tens place: 7 choices remain.

\[
1\times9\times8\times7=504
\]

**Case 2: Last digit is 2, 4, 6, or 8**

- Units place: 4 choices.
- First digit: 8 choices (non-zero and different from the last digit).
- Hundreds place: 8 choices remain.
- Tens place: 7 choices remain.

\[
4\times8\times8\times7=1792
\]

Add the two cases:

\[
504+1792=\boxed{2296}
\]

**Why do we split the cases?** When the last digit is zero, zero is no longer available for the first place anyway, so the number of first-place choices is different. Treating all even last digits as one identical case causes mistakes.

### Example 2 — Four-digit even numbers when repetition is allowed

Using digits 0–9:

- First digit: 9 choices (1–9).
- Middle two digits: 10 choices each.
- Last digit: 5 even choices (0, 2, 4, 6, 8).

\[
9\times10\times10\times5=\boxed{4500}
\]

### Example 3 — Four different even digits, all selected from {0, 2, 4, 6, 8}

There are two different possible questions:

**Question A: Select 4 even digits.** Order does not matter.

\[
{}^5C_4=\boxed{5}
\]

**Question B: Form 4-digit numbers from 4 different even digits.** Order matters, and the first digit cannot be zero.

Count all arrangements, then subtract those that start with zero:

\[
{}^5P_4-{}^4P_3
\]

\[
=120-24=\boxed{96}
\]

This distinction is essential: selecting four even digits is not the same as arranging them into four-digit numbers.

---

## 8. Arrangements when some objects are identical

If all objects are different, arrange n objects in \(n!\) ways.

If some objects are repeated and look identical, divide by the factorials of their repeated counts.

\[
\boxed{\frac{n!}{p!q!r!\cdots}}
\]

Here p, q, r are the numbers of identical copies.

### Example — BANANA

BANANA has 6 letters:

- A appears 3 times.
- N appears 2 times.
- B appears 1 time.

\[
\frac{6!}{3!2!}=\boxed{60}
\]

Why divide? Swapping identical A's or identical N's does not create a new visible arrangement.

---

## 9. Arrangements in a circle

For n different people sitting around a round table, rotations are treated as the same arrangement.

\[
\boxed{(n-1)!}
\]

Example: 5 different people around a circular table:

\[
(5-1)!=4!=\boxed{24}
\]

**Why not \(5!\)?** In a circle there is no fixed first seat. Fix one person in one position, then arrange the remaining people.

Use this formula for a circular arrangement when rotations are considered identical. A question about a row or numbered seats is not circular.

---

## 10. Restrictions: together, not together, and no two adjacent

### A. Two people must sit together

Treat the two people as one block.

Example: Arrange A, B, C, D in a row with A and B together.

- Treat AB as one block: [AB], C, D.
- Arrange the 3 units: \(3!\).
- Inside the block, A and B can be AB or BA: \(2!\).

\[
3!\times2!=\boxed{12}
\]

### B. Two people must not sit together

Use the complement method:

\[
\boxed{\text{Not together}=\text{Total arrangements}-\text{Together arrangements}}
\]

For A, B, C, D:

\[
4!-12=24-12=\boxed{12}
\]

This is often easier than counting every separated arrangement directly.

### C. No two selected people of one group can be adjacent

Use the **gap method**.

Simple example: Arrange 3 different boys first:

\[
B\quad B\quad B
\]

There are 4 available gaps:

\[
\_\,B\,\_\,B\,\_\,B\,\_
\]

To place 2 girls without putting them together, choose 2 of these 4 gaps and arrange the girls:

\[
3!\times{}^4C_2\times2!
\]

\[
=6\times6\times2=\boxed{72}
\]

The gap method is useful when a question says no two girls, boys, letters, or selected objects should be adjacent.

---

## 11. Combination patterns that appear in admission tests

### A. Selecting a committee

Select r people from n:

\[
{}^nC_r
\]

Example: Select 4 students from 9:

\[
{}^9C_4=126
\]

### B. A particular person must be included

Fix that person in the group, then select the remaining members.

Example: A 4-person committee from 9 students must include Ali:

\[
{}^8C_3=56
\]

### C. A particular person must be excluded

Remove that person from the available set.

\[
{}^8C_4=70
\]

### D. At least one

At least one means 1, 2, 3, and so on. Adding every possible case can be long.

Use:

\[
\boxed{\text{At least one}=\text{Total}-\text{None}}
\]

Example: Select at least one girl from a group of 5 boys and 4 girls for a 3-person team.

- Total teams: \({}^9C_3\).
- Teams with no girls (all boys): \({}^5C_3\).

\[
{}^9C_3-{}^5C_3=84-10=\boxed{74}
\]

### E. Exact number from two groups

If a team must contain exactly r people from Group A and s people from Group B:

\[
\boxed{{}^aC_r\times{}^bC_s}
\]

Example: Choose 2 boys from 5 and 2 girls from 4:

\[
{}^5C_2\times{}^4C_2=10\times6=\boxed{60}
\]

### F. Two particular people must both be included

Fix both people, then choose the remaining members.

For a 5-person team from 10 people, with A and B both included:

\[
{}^8C_3=56
\]

### G. Two particular people cannot both be included

Use the complement:

\[
\text{Total groups}-\text{Groups containing both}
\]

For a 3-person team from 8 people, A and B cannot both be included:

\[
{}^8C_3-{}^6C_1=56-6=\boxed{50}
\]

---

## 12. Combination identities and shortcuts

These identities can save time in MCQs.

### Symmetry

\[
\boxed{{}^nC_r={}^nC_{n-r}}
\]

Example:

\[
{}^{10}C_8={} ^{10}C_2=45
\]

Choose 8 to include, or choose the 2 to leave out. Both describe the same group.

### Pascal identity

\[
\boxed{{}^nC_r+{}^nC_{r-1}={}^{n+1}C_r}
\]

### Sum of all combinations

\[
\boxed{{}^nC_0+{}^nC_1+\cdots+{}^nC_n=2^n}
\]

This is the number of all possible subsets of n different objects, including the empty set.

### Useful values

\[
{}^nC_0={}^nC_n=1
\]

\[
{}^nC_1={}^nC_{n-1}=n
\]

\[
{}^nC_2=\frac{n(n-1)}{2}
\]

\[
{}^nP_2=n(n-1)
\]

### Very useful relationship

\[
{}^nP_r=r!\,{}^nC_r
\]

If you know the combination and need the number of arrangements of the selected group, multiply by \(r!\).

---

## 13. Common NET mistakes to avoid

| Common mistake | Correct repair |
|---|---|
| Using permutation for a committee | A committee is a selection: use combination. |
| Using combination for seats or ranks | Different positions matter: use permutation. |
| Forgetting that order matters in a number | Digits occupy different places: count arrangements. |
| Allowing zero in the first place | The first digit of a multi-digit number cannot be zero. |
| Choosing an even last digit after arranging the other digits | Fix the units digit first, then count the remaining positions. |
| Using one case when zero and non-zero endings give different choices | Split the cases and add them. |
| Using \(n^r\) when repetition is forbidden | Use \(nP r\), or multiply decreasing choices. |
| Using \(nP r\) when repetition is allowed | Use \(n^r\) if each position has n independent choices. |
| Forgetting repeated letters | Divide by factorials of identical-letter counts. |
| Using \(n!\) for a circular table | Use \((n-1)!\) when rotations are equivalent. |
| Counting “at least one” directly | Use total minus none when that is simpler. |
| Counting “not together” directly | Use total minus together. |

### My special revision focus

Before solving a restricted counting question, write down:

- Does order matter?
- Is repetition allowed?
- Is zero available?
- Can zero be first?
- Is there a required last digit?
- Are objects identical?
- Is it a line or a circle?
- Does the question say together, apart, at least one, or exactly?

These eight checks prevent most avoidable errors.

---

## 14. A quick decision flow

1. **Are you choosing a group?** Use combination.
2. **Are you arranging items into positions?** Use permutation or position-by-position multiplication.
3. **Can an item repeat?** If yes, consider \(n^r\); if no, choices decrease.
4. **Is there a special final digit?** Fix that digit first.
5. **Is zero among the digits?** The first digit cannot be zero.
6. **Are some objects identical?** Divide by repeated factorials.
7. **Is it circular?** Consider \((n-1)!\).
8. **Does it say at least one or not together?** Try the complement method.

---

## 15. Ten-minute formula sheet

| Situation | Formula |
|---|---|
| Arrange r from n, no repetition | \({}^nP_r=\frac{n!}{(n-r)!}\) |
| Select r from n | \({}^nC_r=\frac{n!}{r!(n-r)!}\) |
| Arrange r positions, repetition allowed | \(n^r\) |
| Relation between P and C | \({}^nP_r=r!\,{}^nC_r\) |
| Arrange n different objects in a row | \(n!\) |
| Arrange with identical objects | \(\frac{n!}{p!q!\cdots}\) |
| Arrange n different people in a circle | \((n-1)!\) |
| At least one | Total − None |
| Not together | Total − Together |
| Together | Treat the required objects as one block |
| Exact selection from separate groups | \({}^aC_r\times{}^bC_s\) |
| Select 2 from n | \(\frac{n(n-1)}{2}\) |

---

## 16. Active-recall check — answer without looking above

Try to explain each answer in one or two sentences. Do not only memorize the formula.

1. Why are choosing a committee and arranging students in seats different?
2. What is the value of \(0!\)?
3. What is the difference between \({}^nP_r\) and \({}^nC_r\)?
4. How many 3-digit codes can be made from 1–5 without repetition?
5. How many 3-digit codes can be made from 1–5 when repetition is allowed?
6. Why must the last digit be selected first for a 4-digit even-number problem?
7. Why do 4-digit numbers from digits 0–9 need separate cases when the last digit is zero or non-zero?
8. How many ways can 4 even digits be selected from {0, 2, 4, 6, 8}?
9. What changes when those same four even digits must be arranged into a 4-digit number?
10. Why do we divide by \(3!2!\) when arranging BANANA?
11. Why is a circular arrangement \((n-1)!\), not \(n!\)?
12. Explain “at least one” using the complement method.

### Answers for checking

1. A committee has no order; seats have different positions.
2. \(0!=1\).
3. Permutation counts order; combination does not.
4. \(5\times4\times3=60\).
5. \(5^3=125\).
6. Evenness is decided by the units digit.
7. If zero is last, it cannot also be first, and the first-place choices differ from the non-zero-last case.
8. \({}^5C_4=5\).
9. Order now matters and zero cannot be first: \({}^5P_4-{}^4P_3=96\).
10. Swapping identical A's or N's does not produce a new visible word.
11. Rotations describe the same circular seating; fix one person to remove duplicate rotations.
12. Count every possible outcome, then subtract the outcomes with none.

---

## 17. Revision schedule — keep the topic in memory

Use active recall before re-reading. First try to write the formulas and explain the decision rule from memory.

| When | What to do | Time |
|---|---|---:|
| Same day | Read Sections 1, 3, 7, 11 and the formula sheet; solve the active-recall check | 20 min |
| Next day | Rebuild the formulas from memory; redo even-number and committee examples | 15 min |
| After 3 days | Solve 10 mixed questions without notes; mark every error by type | 20 min |
| After 7 days | Attempt a timed mixed P&C set; revisit only weak patterns | 25 min |
| Before a mock | Read the decision flow and common-mistakes table | 5 min |

### Error-analysis template

After a practice set, record:

- **Question number:**
- **My answer:**
- **Correct answer:**
- **Mistake type:** wrong method / missed restriction / arithmetic / case split / formula recall / careless reading
- **Why my method failed:**
- **Correct idea in one sentence:**
- **One similar question to redo:**

Do not write only “silly mistake.” Name the exact reason, such as “I allowed zero in the first position” or “I treated an unordered selection as an arrangement.”

---

## Final memory lines

- **Order matters → permutation.**
- **Order does not matter → combination.**
- **Repeated choices → often \(n^r\).**
- **No repetition → decreasing choices.**
- **Even number → last digit even.**
- **Zero cannot be the first digit.**
- **Together → block method.**
- **Not together → total minus together.**
- **At least one → total minus none.**
- **Identical objects → divide by repeated factorials.**
- **Circle → fix one person, then arrange the rest.**

The target is not to memorize every question. Learn to identify the counting structure, apply the restrictions in the correct order, and then calculate.
