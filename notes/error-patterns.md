# Error Patterns

> Operational taxonomy for tagging IELTS practice material and session reviews.
> Add a tag only when the error is observed in a learner draft or deliberately targeted by an exercise.

---

## Provenance rule

Do not describe a newly generated prompt as recovered from a previous session.

| Value | Meaning |
|---|---|
| `historical-session-derived` | Exact or substantially recoverable material from a documented session |
| `personal-session-result` | Learner-authored response, score or reflection |
| `repo-existing` | Material already present in the repository |
| `newly-generated` | New original practice content |
| `attested-session-topic` | The topic occurred previously, but the current wording is newly generated |

---

## High-priority structural patterns

### `indirect-question-word-order`

**Problem**

Using interrogative word order inside an indirect question.

```text
Incorrect: Could you tell me where is the hotel located?
Correct:   Could you tell me where the hotel is located?
```

**Detection rule**

After introductory forms such as `Could you tell me`, `I would like to know`,
`Do you know whether`, use statement word order.

**Drill target**

Formal information requests and Task 1 letters.

---

### `causal-clarity`

**Problem**

The explanation contains facts, but the causal relationship between them is implicit or ambiguous.

```text
Weak:     I cannot attend because I have work and the meeting was changed.
Stronger: I cannot attend because my employer moved a mandatory client meeting
          to the same afternoon.
```

**Detection rule**

The reader should be able to identify cause, consequence and requested action without inference.

---

### `gerund-chaining`

**Problem**

Several `-ing` clauses are chained together, producing weak attachment or unclear sequencing.

```text
Weak:     Travelling abroad, meeting new people and learning cultures,
          improving a person's mind.
Stronger: Travelling abroad exposes people to unfamiliar perspectives,
          which can broaden their understanding of other cultures.
```

**Detection rule**

When two or more gerund phrases appear consecutively, check whether each has a clear subject and logical role.

---

### `verb-complement-pattern`

**Problem**

Italian complement structures are transferred directly into English.

```text
Incorrect: The government required companies to reducing emissions.
Incorrect: They demanded the company to solve the problem.
Correct:   The government required companies to reduce emissions.
Correct:   They demanded that the company solve the problem.
```

---

## Lexical patterns

### `weak-intensifier`

**Problem**

Overuse of `very + basic adjective`.

| Weak | Prefer when accurate |
|---|---|
| very important | critical, fundamental, pivotal |
| very expensive | costly, financially burdensome |
| very bad | harmful, detrimental, adverse |
| very common | widespread, prevalent |
| very large | substantial, considerable |

**Constraint**

Do not replace words mechanically. Precision is more important than apparent sophistication.

---

### `false-cognate`

Frequent Italian interference:

| Intended meaning | Avoid | Use |
|---|---|---|
| attualmente | actually | currently, at present |
| eventualmente | eventually | possibly, if necessary |
| sensibile, emotivamente reattivo | sensible | sensitive |
| argomento, tema | argument when no disagreement exists | topic, issue, subject |

---

### `verb-deflation`

Prefer a precise verb over an unnecessary noun phrase.

| Weak | Stronger |
|---|---|
| make a decision | decide |
| make a proposal | propose |
| have a discussion | discuss |
| give a recommendation | recommend |

---

### `prompt-repetition`

**Problem**

Copying the wording of the Task 2 prompt into the introduction or conclusion.

**Correction process**

1. Identify the core noun phrase.
2. Identify the central action or relationship.
3. Replace both while preserving the scope and logical claim.
4. Check that the paraphrase has not altered the question.

---

## Task-response patterns

### `missing-bullet`

One or more mandatory Task 1 bullet points are absent or insufficiently developed.

### `unclear-position`

The Task 2 position cannot be stated in one sentence after reading the introduction.

### `two-part-coverage`

A two-part question receives uneven treatment or one part is answered only implicitly.

### `explicit-weighing`

An advantages/disadvantages essay lists both sides but never states the criterion used to decide which side outweighs the other.

### `matched-solution`

A proposed solution does not directly address a cause previously identified.

### `example-development`

An example is named but not connected back to the paragraph claim.

---

## Register patterns

### `formal-register`

Check for:

- neutral, precise wording;
- appropriate salutation and closing;
- controlled use of contractions;
- clear requests rather than commands;
- no slang, threats or exaggerated emotional language.

### `hedged-request`

Use proportionate request forms:

```text
I would be grateful if you could...
Could you please confirm whether...
I would appreciate your assistance in...
```

Avoid excessive deference that obscures the requested action.

---

## Tagging example

```yaml
error_tags:
  - indirect-question-word-order
  - causal-clarity
  - weak-intensifier
observed_in_draft: true
review_status: human-reviewed
```

*Last updated: July 2026*
