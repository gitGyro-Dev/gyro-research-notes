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

## 4. Provisional Definition of ～ed / 局所的成立

For the next stage of examination, `～ed` and `局所的成立` are treated as the same provisional concept.

> **～ed / 局所的成立 = Operatorが、その時点で後続の処理から参照可能・利用可能な形になった局所的成立。**

Important clarifications:

- `～ed` does not mean that the whole ongoing flow has ended.
- `～ed` does not have to be important.
- `～ed` does not have to be actually used later.
- `～ed` only needs to have become available to subsequent processing at that time.
- `～ed` does not imply permanent retention.
- availability at the time of establishment and actual later use are separate matters.

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

Each can be treated as a local establishment if it has become available to subsequent processing.

Even `sensor = 0` / `no detection` may be a valid `～ed` if it is available to the control process, whether or not it causes an observable state change.

Therefore:

> `～ed` is not equivalent to “important event” or “state change.”

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

Each may become available to later processing.

However, the human case is likely to contain many more small and overlapping local establishments than the simplified diagram shows.

This should not be used as an escape from falsification. The granularity of `～ed` remains unresolved and is now the primary test target.

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

---

## 8. Retroactive Access / 遡り

The sequence is not necessarily forward-only.

A later process may refer back to earlier local establishments if some form of access remains possible:

```text
～ed₀   ～ed₁   ～ed₂   ～ed₃
   \      |      |      /
      retroactive handling
             ↓
      new local establishment
```

`遡り` does not mean returning physically or logically to the past state itself.

It means:

> from the current position, earlier local establishments can be handled again if they remain accessible or can be reconstructed.

The mechanism of access, retention, or reconstruction is not yet fixed.

---

## 9. Two Different Types of Retroactive Case

### Case A: A new ～ed is established only after retroactive handling

```text
点₀
↓
点₁
↓
点₂
```

At these earlier points, the relation `「近づいている」` may not yet have existed as a local establishment.

Later, by handling the earlier sequence together:

```text
点₀ + 点₁ + 点₂
        ↓
「大きくなっている」
        ↓
「近づいている」
```

A **new current ～ed** may be established.

This does not require the later result to have existed previously as a hidden stored item.

### Case B: A past ～ed existed, but is no longer currently usable

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

---

## 10. Example: “ずっとOPENだった”

Automatic-door history:

```text
OPEN₀ → OPEN₁ → OPEN₂ → OPEN₃
```

Each `OPENₙ` may be a separate local establishment.

Later, if the earlier states remain accessible or reconstructable, handling them together may establish:

```text
「ずっとOPENだった」
```

This result need not have existed previously as a single stored `～ed`.

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

These stages may occur within an extremely short real-time interval and appear externally as one continuous process.

---

## 12. Retention Is Separate from ～ed

Local establishment and retention are separate questions.

An `～ed` may have been available at one time and later become inaccessible.

Retroactive handling therefore requires some form of current access to earlier establishments, but this access might arise from direct retention, compressed residue, reconstruction, or another mechanism not yet fixed.

For now:

```text
成立した
≠
保持された
≠
現在アクセス可能
≠
後から再構成可能
```

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

This is still a descriptive image, not a formal model.

---

## 14. Claude Review: Accepted Corrections

The following corrections from external review are accepted for the next test cycle:

1. `扱える` must mean **available / usable in principle by subsequent processing**, not necessarily actually used.
2. actual use and local establishment must be separated.
3. `～ed` and `局所的成立` will be treated as the same provisional concept for now.
4. Test 1 in the previous version was effectively tautological under the definition and is removed as a primary falsification test.
5. retroactive handling implicitly requires some form of access to earlier establishments; this dependency must be explicit.
6. human complexity or overlap must not be used as a catch-all explanation when the granularity criterion is unclear.

---

# 15. Test 6 — Minimal Conditions for ～ed / 局所的成立

This section is the only active focus for the next discussion cycle.

The aim is not to define a threshold, purpose, importance, or full Operator architecture.

The question is:

> **What is the smallest set of conditions under which something can be said to have become a local establishment (`～ed`) for an Operator?**

The current candidate set is intentionally minimal and provisional.

## Candidate C1 — Something is available to the Operator/system

There must be something that can enter or participate in the Operator's processing.

This does **not** yet require:

- importance
- novelty
- explicit purpose
- conscious attention
- a state change

Question:

> Can `～ed` exist if nothing is available to the Operator at all?

If the answer is no, C1 may be necessary.

---

## Candidate C2 — It becomes distinguishable in processing

The candidate must become distinguishable enough that subsequent processing could treat it as this rather than an entirely undifferentiated continuation.

Examples:

```text
sensor=0
sensor=1
```

or

```text
何かある
何か動いている
```

This does not mean that the Operator needs a linguistic label or conscious recognition.

Question:

> Is distinguishability really necessary, or is availability alone sufficient?

This is deliberately unresolved.

---

## Candidate C3 — It is available to subsequent processing

The candidate must have become usable or referable by some subsequent processing path at that time.

Actual use is not required.

```text
～ed成立
   ↓
後続処理Aから使われる
後続処理Bからは使われない
どこからも実際には使われない
```

All three may still satisfy C3 if the result was available to at least one possible subsequent processing path at the time of establishment.

Question:

> Is “availability to at least one subsequent processing path” sufficient, or does this merely restate the current definition?

This is a central risk of circularity.

---

# 16. Minimal Test Matrix

The next wall-bouncing session should test only C1–C3.

| Case | C1 Available | C2 Distinguishable | C3 Available to later processing | Candidate ～ed? | Why? |
|---|---:|---:|---:|---|---|
| Automatic door: sensor=0 sampled normally | Yes | Yes | Yes | likely Yes | control path can reference it |
| Automatic door: analog voltage changes but is never sampled | ? | ? | No | unclear / likely No | ongoing flow may never become locally usable |
| Automatic door: sampled value immediately corrupted before any downstream access | Yes? | Yes? | No? | boundary case | tests whether establishment precedes downstream accessibility |
| Ball: color becomes available but is never used for avoidance | Yes | Yes | Yes? | likely Yes | actual use is unnecessary |
| Ball: visual variation exists but never becomes distinguishable to processing | Yes? | No | No? | unclear | tests necessity of distinguishability |
| Repeated identical sensor=0 values | Yes | Yes? | Yes | unclear | tests whether change/novelty is required |

The table is intentionally unresolved. The purpose is to expose which candidate conditions do real work.

---

# 17. Specific Questions for the Next Discussion

Do not add new concepts before testing these questions.

1. **Is C1 necessary?**  
   Can there be local establishment without anything being available to the Operator/system?

2. **Is C2 necessary?**  
   If something participates in processing but never becomes distinguishable from the ongoing continuation, can it still count as `～ed`?

3. **Is C3 independent of C1/C2?**  
   Or does “available to subsequent processing” merely repeat what `～ed` means?

4. **Is change required?**  
   Can `sensor=0` followed by another `sensor=0` produce separate `～ed₀` and `～ed₁` without any value change?

5. **Is novelty required?**  
   If the same local result occurs repeatedly, does each occurrence remain a local establishment?

6. **Can an ～ed exist with no observable consequence?**  
   If it becomes available but no downstream path actually consumes it, does the definition still hold?

7. **Where exactly does the corrupted-sample case fail?**  
   If a value is formed but destroyed before any downstream path can access it, was there an `～ed` for an instant, or not?

These questions should be tested first with the automatic-door case, then with ball recognition only if the same distinction remains meaningful.

---

## 18. What Remains Explicitly Out of Scope for Test 6

Do not settle these during the Test 6 cycle unless strictly necessary:

- full definition of Operator
- physical mechanism of sensing
- exact granularity or threshold
- purpose / attention / priority
- PULL ordering
- retention architecture
- retroactive reconstruction mechanism
- information definition
- Gyro mapping
- formal mathematical notation
- replacement of `～ing / ～ed` terminology

The purpose of Test 6 is narrower:

> **reduce the establishment condition as far as possible without making it circular or vacuous.**

---

## 19. Review Request for Test 6

Please challenge only the proposed minimal conditions C1–C3.

Focus on:

1. whether any condition is redundant
2. whether any condition is circular
3. a counterexample where C1–C3 all appear satisfied but `～ed` should still not be said to exist
4. a counterexample where one of C1–C3 fails but `～ed` still appears to exist
5. whether repeated identical inputs can generate distinct local establishments without introducing an explicit threshold or clock
6. whether the corrupted-sample case exposes a missing distinction
7. the smallest revision that would make the candidate conditions more testable

Do not broaden the review into a general theory of information, cognition, memory, or Gyro unless a direct contradiction requires it.
