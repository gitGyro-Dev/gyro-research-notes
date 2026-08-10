# Information / PULL / ～ing・～ed Study

**Date:** 2026-08-09
**Target Layer:** Gyro Brainstorm / Pre-Theoretical Study
**Status:** Working checkpoint for multi-AI review

---

## 1. Purpose

This note captures the current working state of the discussion around information extraction, PULL, local establishment, continuous flow (`～ing`), locally established states (`～ed`), and retroactive access.

The purpose is not to finalize a theory, but to create a reviewable checkpoint that can be critiqued by multiple AI systems and then refined.

---

## 2. Current Working Premises

### 2.1 Target / event itself is not treated as information

For the current study, the object, event, or process itself is not simply identified with information.

```text
対象・事象 ≠ 情報
```

This is a working premise for analysis, not a metaphysical claim.

---

### 2.2 Operator does not necessarily take in the whole target

The current working image is that an Operator does not necessarily receive the whole ongoing target/process as-is.

Instead, something becomes locally usable and is PULLed or otherwise used in subsequent processing.

Terms such as `purpose`, `direction`, `orientation`, and `relation` remain provisional and should not yet be treated as fixed formal concepts.

---

## 3. Continuous Flow: ～ing

`～ing` is used provisionally to represent an ongoing, connected flow.

This is not meant as a claim about English grammar or physical time.

Example:

```text
人が近づいている
────────────────────────→
        ～ing
```

or

```text
ボールが飛んでいる
────────────────────────→
        ～ing
```

The key point is that the flow itself does not stop merely because an Operator locally handles some part of it.

---

## 4. Provisional Definition of ～ed

For the next stage of examination, the following definition is fixed provisionally:

> **～ed = Operatorが、その時点で後続の処理から扱える形になった局所的成立。**

Important clarifications:

- `～ed` does not mean that the whole ongoing flow has ended.
- `～ed` does not have to be important.
- `～ed` does not have to be actually used later; it only needs to have become locally usable at that time.
- `～ed` does not imply permanent retention.

This is a working definition to be tested for failure cases.

---

## 5. Automatic Door Example

A simplified automatic-door flow:

```text
人が近づいている ～ing
        ↓
センサー値が得られる
        ↓
「検知あり」
        ↓
OPEN判定
```

Under the provisional definition:

```text
～ed₀ = センサー値
～ed₁ = 「検知あり」
～ed₂ = OPEN指示
```

Each of these can be treated as a local establishment because it has become usable by subsequent processing.

Even `sensor = 0` / `no detection` can be a valid `～ed` if it is used to maintain CLOSE.

Therefore:

> `～ed` is not equivalent to “important event.”

It is simply something that has become locally usable by the Operator/system at that point.

---

## 6. Ball Recognition Example

A simplified recognition chain:

```text
何かある
↓
動いている
↓
近づいている
↓
ボールだ
↓
危ない
```

Potential local establishments:

```text
～ed₀ = 「何かある」
～ed₁ = 「動いている」
～ed₂ = 「近づいている」
～ed₃ = 「ボールだ」
```

Each can be used by later processing.

However, the human case is likely to contain many more small and overlapping local establishments than the simplified diagram shows.

The current hypothesis is not “human recognition is fundamentally different because it is complex,” but rather:

> many small local establishments may occur at very short intervals and in overlapping processing chains.

---

## 7. ～ing and ～ed Are Not Alternating Global States

An earlier simple model would be:

```text
～ing → ～ed → ～ing → ～ed
```

The current view is closer to:

```text
～ing ───────────────────────────────→
        ↓      ↓      ↓      ↓
      ～ed₀  ～ed₁  ～ed₂  ～ed₃
```

That is:

> the larger ongoing flow continues, while local `～ed` states are established within it.

This is considered a more natural model for both automatic-door processing and ball recognition.

---

## 8. Retroactive Access / 遡り

The sequence is not necessarily forward-only.

A later state may refer back to earlier local establishments:

```text
～ed₀   ～ed₁   ～ed₂   ～ed₃
   \      |      |      /
      retroactive PULL
             ↓
      new local establishment
```

`遡り` does not mean returning physically or logically to the past state itself.

It means:

> from the current position, earlier local establishments can be handled again if they remain accessible or reconstructable.

---

## 9. Two Different Types of Retroactive Case

Two cases must be separated.

### Case A: A new ～ed is established only after retroactive handling

Example:

```text
点₀
↓
点₁
↓
点₂
```

At these earlier points, the relation:

```text
「近づいている」
```

may not yet have existed as a local establishment.

Later, by handling the earlier sequence together:

```text
点₀ + 点₁ + 点₂
        ↓
「大きくなっている」
        ↓
「近づいている」
```

A **new current ～ed** is established.

Thus:

> the later `～ed` is not necessarily something that had been hidden in the past waiting to be found.

It may be newly established in the present through retroactive handling of earlier local establishments.

---

### Case B: A past ～ed existed, but is no longer currently usable

Example:

```text
時点 t0
「青いボールだ」
    ～ed
```

This may have been locally usable at `t0`.

Later, the system may no longer be able to access it.

Therefore:

```text
成立した
≠
保持された
≠
後から遡れる
```

This distinction is important.

An `～ed` may have existed at one time without being permanently retained or recoverable.

---

## 10. Example: “ずっとOPENだった”

Automatic-door history:

```text
OPEN₀ → OPEN₁ → OPEN₂ → OPEN₃
```

Each `OPENₙ` may be a separate local establishment.

Later, by handling them together:

```text
OPEN₀
OPEN₁
OPEN₂
OPEN₃
  ↑
retroactive handling
  ↓
「ずっとOPENだった」
```

`「ずっとOPENだった」` does not need to have been stored previously as a single `～ed`.

It may be a newly established current result derived from the relation among multiple earlier local establishments.

The same applies to:

```text
「近づいている」
「繰り返している」
「以前と違う」
```

These may depend on relations among multiple local establishments rather than a single point.

---

## 11. Time Order vs Establishment Order

The current discussion is not making a physical claim that meaningful time delays must exist.

The distinction is primarily structural:

```text
成立順:
～ed₀
↓
～ed₁
↓
～ed₂
↓
遡り
↓
関係を見る
↓
新しい～ed
```

These stages may occur within an extremely short real-time interval.

So, from an external perspective, they may appear almost simultaneous and continuous.

This is why:

```text
ボールを見る
↓
「あ、ボールがこっちに飛んできている」
```

can look like one continuous real-time event even if many local establishments and retroactive references are structurally involved.

---

## 12. Retention Is Separate from ～ed

One of the important corrections is:

> local establishment and retention must not be conflated.

For example, in an automatic door:

```text
10:00:01 sensor=0 → ～ed
10:00:02 sensor=0 → ～ed
10:00:03 sensor=1 → ～ed
```

If no log is kept, the earlier values may no longer be available later.

Thus:

```text
～ed成立
   ↓
┌───────────────┐
│ immediately used │
│ retained          │
│ discarded / lost  │
└───────────────┘
```

The retention path is a separate issue.

---

## 13. Current Minimal Image

```text
             ～ing
────────────────────────────────────────→
      ↓         ↓         ↓         ↓
    ～ed₀     ～ed₁     ～ed₂     ～ed₃
      │         │         │         │
      └─────────┴─────────┴─────────┘
                        ↑
                 retroactive handling
                        ↓
                new local establishment
                        ↓
                  Operator update
                        ↓
                  next processing...
```

The larger `～ing` continues throughout this process.

Local establishments may be created, used, retained, lost, or later re-used.

---

## 14. What Is Still Unfixed

The following remain intentionally open:

- whether `～ed` and `局所的成立` are ultimately identical terms
- whether PULL always occurs before or after `～ed`, or whether both patterns exist
- what determines the granularity of `～ed`
- what or who makes something become `～ed`
- whether retroactive access is continuous or only occasional
- whether earlier `～ed` values are stored, reconstructed, or both
- how Operator orientation should be represented
- where “information” itself should be placed in this process
- whether `～ing / ～ed` terminology should later be replaced with neutral symbols
- how this model differs from or overlaps with existing theories such as state estimation, smoothing, active inference, phenomenology of retention, and process/event models

---

## 15. Immediate Test Questions

The next stage should actively try to break the provisional definition of `～ed`.

### Test 1

Can there be something that appears locally established but is not usable by any subsequent processing?

### Test 2

Can a process continue without any identifiable `～ed` being established?

### Test 3

Can two Operators derive contradictory `～ed` values from the same ongoing `～ing`?

### Test 4

Can a later `～ed` be established only through retroactive handling of multiple earlier `～ed` values?

### Test 5

Can a past `～ed` have existed but become permanently inaccessible later?

### Test 6

What is the smallest set of conditions under which `～ed` can be said to have been established without relying on vague terms such as “importance,” “purpose,” or “threshold”?

---

## 16. Working Definition for Review

For this review cycle, use the following as the primary provisional definition:

> **～ed = Operatorが、その時点で後続の処理から扱える形になった局所的成立。実際に後続処理で使われる必要はなく、永続的に保持される必要もない。**

This definition should be treated as provisional and should be challenged rather than protected.

---

## 17. Review Request

Please review this note with particular attention to:

1. logical contradictions
2. ambiguity in the provisional definition of `～ed`
3. examples where the definition fails
4. cases where retroactive handling cannot be explained naturally
5. hidden assumptions about retention or memory
6. over-generalization from automatic-door and ball-recognition examples
7. overlap with existing theories
8. what should remain unfixed for now
9. what single issue should be tested next

Do not assume the model is correct. Prefer counterexamples and boundary cases over supportive reinterpretation.
