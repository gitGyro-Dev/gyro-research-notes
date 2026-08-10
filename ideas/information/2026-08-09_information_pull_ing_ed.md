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

The earlier definition focused on downstream usability:

> `～ed / 局所的成立 = Operatorが、その時点で後続の処理から参照可能・利用可能な形になった局所的成立。`

Multi-AI review exposed a circularity risk in that wording. The active question is therefore shifted one step earlier.

For the next test cycle, do **not** treat downstream usability as the defining condition.

Instead, investigate the following weaker working image:

> **A local establishment (`～ed`) is something the Operator treats, or can treat, as one unit within an ongoing `～ing`.**

Important cautions:

- `～ed` does not mean that the whole ongoing flow has ended.
- `～ed` does not have to be important.
- `～ed` does not require an observable state change.
- `～ed` does not have to be actually used later.
- `～ed` does not imply permanent retention.
- the boundary of an `～ed` is not assumed to exist independently on the target side.
- the Operator-side way of treating something as one unit is now the primary test target.

This is still provisional and intentionally incomplete.

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

Earlier versions treated each of the following as candidate local establishments:

```text
～ed₀ = センサー値
～ed₁ = 「検知あり」
～ed₂ = OPEN指示
```

The new question is not merely whether each result is usable later.

It is:

> **What makes the Operator/system treat each of these as one unit rather than as an undifferentiated continuation of the larger flow?**

This becomes especially important for repeated identical values.

```text
sensor=0
sensor=0
sensor=0
sensor=0
```

Possible interpretations include:

```text
Operator A:
0 | 0 | 0 | 0
→ four local units

Operator B:
0000
→ one continuous state until change

Operator C:
00 | 00
→ two local units
```

The same target-side continuation may therefore permit different unitizations depending on the Operator-side processing structure.

This is now treated as a central test case rather than a defect to be hidden by a threshold assumption.

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

The current question is not whether these are all valid because later processing can use them.

Instead:

> **How does the Operator come to treat “何かある”, “動いている”, “近づいている”, or “ボールだ” as one unit at each stage?**

The human case may contain many overlapping processes, but complexity must not be used as an escape from this question.

---

## 7. ～ing and ～ed Are Not Alternating Global States

An earlier simple model would be:

```text
～ing → ～ed → ～ing → ～ed
```

The current view remains closer to:

```text
～ing ───────────────────────────────→
        ↓      ↓      ↓      ↓
      ～ed₀  ～ed₁  ～ed₂  ～ed₃
```

That is:

> the larger ongoing flow continues, while the Operator may treat some portions/results within it as local units.

The flow does not have to stop for a local establishment to occur.

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

Each `OPENₙ` may or may not have been treated as a separate local unit at the time.

Later, if earlier states remain accessible or reconstructable, the Operator may treat the sequence together and establish:

```text
「ずっとOPENだった」
```

This result need not have existed previously as a single stored `～ed`.

The example also shows that unitization can occur at more than one scale:

```text
OPEN₀, OPEN₁, OPEN₂, OPEN₃
```

and later:

```text
「ずっとOPENだった」
```

can both become units for different processing contexts.

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

Local establishment and retention remain separate questions.

An `～ed` may have been treated as one unit at one time and later become inaccessible.

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

The diagram remains descriptive, but the active interpretation has changed:

> `～ed` should not be imagined as a boundary that necessarily emerges by itself on the target side. The current question is how the Operator-side processing treats something within the ongoing flow as one unit.

---

## 14. Multi-AI Review: Accepted Corrections

The following corrections are accepted for the next test cycle:

1. actual downstream use and local establishment must be separated.
2. `～ed` and `局所的成立` are treated as the same provisional concept for now.
3. the earlier C1/C3 availability conditions were substantially redundant and risked circular definition.
4. “distinguishable” must not be silently equated with observable value change.
5. repeated identical values are a primary boundary case, not a trivial example.
6. the existence and count of local establishments may depend on Operator-side processing structure rather than target-side variation alone.
7. retroactive handling implicitly requires some form of access to earlier establishments; this dependency remains explicit.
8. human complexity or overlap must not be used as a catch-all explanation when unitization is unclear.

---

# 15. Test 6 — Operator-side Unitization / 区切り方

This section is the only active focus for the next discussion cycle.

The earlier question was:

> What is the smallest set of conditions under which something can be said to have become a local establishment (`～ed`)?

That framing tended to treat the local establishment as if it formed by itself and encouraged circular conditions such as “it is established when it is usable.”

The question is now revised to:

> **Within a continuous `～ing`, how does an Operator treat some portion, result, or relation as one local unit (`～ed`)?**

A stronger Japanese working formulation is:

> **連続する ～ing の中で、Operatorはどこまでを「一つとして扱える／一つとして扱ってよい」とするのか？**

This wording intentionally avoids claiming that a local establishment spontaneously “groups itself.”

---

## 15.1 Current working distinction

Do not assume:

```text
～ing
↓
自然にまとまる
↓
～ed
```

Instead test:

```text
～ing ─────────────────────→
        ↓
Operator-side handling
        ↓
「ここまでを一つとして扱う」
        ↓
～ed / 局所的成立
```

The exact mechanism of that handling remains open.

Terms such as `decision`, `judgment`, `threshold`, `sampling`, `boundary`, or `attention` should not yet be treated as universal explanations.

---

## 15.2 Why “まとめる” is still provisional

`まとめる` may sound too active or intentional.

An automatic door does not consciously decide:

> “I will group these 100 ms into one unit.”

Yet its processing structure may still treat a certain range/input/result as one unit.

Therefore the preferred wording for now is:

> **一つとして扱う / 一つとして扱える**

rather than:

> **意識的にまとめる / 判断してまとめる**

The word `judgment` should be used cautiously because it may import human-level cognition unnecessarily.

---

# 16. Unitization Test Matrix

The next wall-bouncing session should test Operator-side unitization directly.

| Same / similar target-side flow | Operator-side treatment | Candidate local units | Main question |
|---|---|---|---|
| `sensor=0` repeated | sample every cycle | `～ed₀, ～ed₁, ～ed₂...` | why does each cycle count as one unit? |
| `sensor=0` repeated | react only on value change | one continuing state until change | is there no new local unit during repetition? |
| `sensor=0` repeated | aggregate a fixed window | grouped units | what makes the window one unit? |
| analog voltage continuously changes | process snapshots | multiple local units | is unitization created by the processing structure? |
| analog voltage continuously changes | process only a relation/pattern | one higher-level unit | can a relation become the first relevant local unit? |
| ball approaching | successive local handling | `something → moving → approaching → ball` | what causes each step to be treated as one unit? |
| `OPEN₀ → OPEN₁ → OPEN₂ → OPEN₃` | later handled together | `ずっとOPENだった` | how can multiple earlier units become one new unit? |

The goal is not to select a universal clock or threshold.

The goal is to determine whether local establishment is better characterized by **Operator-side unitization** than by target-side state change or generic downstream availability.

---

# 17. Specific Questions for the Next Discussion

Do not broaden the discussion before testing these questions.

1. **Does a local unit require target-side change?**  
   Can repeated identical values become separate local establishments solely because the Operator treats them as separate processing units?

2. **Can target-side change occur without a new local unit?**  
   If the Operator treats several changing values together, can they form one `～ed`?

3. **Can the same ongoing flow support different unitizations for different Operators?**  
   If yes, does this threaten the concept or clarify it?

4. **Can the same Operator use different unitizations at different times?**  
   For example, detailed sampling first and later aggregation into `ずっとOPENだった`.

5. **Is “一つとして扱う” enough, or is it still circular?**  
   What observable or structural consequence would show that something was treated as one unit?

6. **Does unitization require explicit retention?**  
   Or can something be treated as one unit and then immediately disappear?

7. **Does a local establishment need a downstream consumer?**  
   Or is being formed as one unit sufficient even if no later processing uses it?

8. **Can unitization itself be revised retroactively?**  
   Can earlier events that were once treated separately later be re-treated as one unit without implying that the earlier unitization was wrong?

These questions should be tested first with the automatic-door case, then with ball recognition only if the same distinction remains meaningful.

---

## 18. What Remains Explicitly Out of Scope for Test 6

Do not settle these during the current cycle unless strictly necessary:

- full definition of Operator
- physical mechanism of sensing
- universal clock or threshold
- purpose / attention / priority
- PULL ordering
- retention architecture
- retroactive reconstruction mechanism
- information definition
- Gyro mapping
- formal mathematical notation
- replacement of `～ing / ～ed` terminology

The purpose of Test 6 is now narrower:

> **clarify how an Operator treats part of an ongoing flow as one local unit without assuming that the unit exists independently or forms itself.**

---

## 19. Review Request for Test 6 — Operator-side Unitization

Please challenge only the revised focus on Operator-side unitization.

Focus on:

1. whether `一つとして扱う / treat as one unit` is still circular or vacuous
2. whether a local unit can exist without target-side change
3. whether target-side change can occur without a new local unit
4. whether repeated identical inputs can legitimately produce multiple local establishments
5. whether the same `～ing` can support different local-unit structures for different Operators
6. whether the same Operator can revise unitization over time or retroactively
7. what structural evidence would distinguish “treated as one unit” from “merely passed through”
8. the smallest revision that would make Operator-side unitization testable without prematurely introducing a universal threshold, clock, purpose, or cognitive judgment

Do not broaden the review into a general theory of information, cognition, memory, or Gyro unless a direct contradiction requires it.
