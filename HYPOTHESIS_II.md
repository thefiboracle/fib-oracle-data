# PRE-REGISTERED HYPOTHESIS II

Committed 16 August 2026, at n=22 readings and zero price observations.

---

## Relationship to Hypothesis I

Hypothesis I is a real question with a published literature behind it
(Hart et al. 2013, Frontiers in Zoology).

**Hypothesis II is not.** There is no proposed mechanism. There is no prior
literature. We are aware of this.

They are kept in separate files for that reason. Nothing in this document
should be read as affecting the status of Hypothesis I.

---

## Claim under test

Subject 001's magnetic alignment predicts the direction of the Solana market.

---

## The weekly bearing vector

Individual bearings are too noisy to test anything. We aggregate weekly.

Take the **circular mean** of all bearings recorded in a calendar week
(Monday 00:00 to Sunday 23:59 AEST).

The circular mean is the correct method for averaging angles. The arithmetic
mean is wrong: the average of 350° and 010° is 0°, not 180°. We mention this
because it is the only part of this document with any methodological merit.

The resulting compass direction is the **WEEKLY BEARING VECTOR**.

The **magnitude** R runs from 0 to 1 and measures how concentrated the week's
bearings were. R near 0 means the readings were scattered and the subject held
no coherent position.

---

## Definitions

| Term | Definition |
|---|---|
| Week | Monday 00:00 to Sunday 23:59 AEST |
| Vector | Circular mean of all bearings recorded that week |
| Northward | Vector between 270° and 090° |
| Southward | Vector between 090° and 270° |
| Magnitude | R, from 0 (scattered) to 1 (perfectly aligned) |
| SOL close | Solana daily close, 00:00 UTC |
| Weekly return | Change in SOL close from Sunday to the following Sunday |

---

## Prediction

**Northward vector = SOL closes the FOLLOWING week higher.**
**Southward vector = SOL closes the FOLLOWING week lower.**

The vector is computed from a completed week and predicts the week after it.
It never predicts the week it was measured in. That would be postdiction and
it would not count.

---

## Minimum sample

A week with **fewer than four readings** is logged as INSUFFICIENT and excluded
from the analysis. A vector computed from two readings is not a vector, it is
two readings.

Excluded weeks are still recorded in the dataset. They are not deleted.

---

## What counts as a hit

- Vector northward and SOL up the following week — hit
- Vector southward and SOL down the following week — hit
- Anything else — miss

Chance is 50%.

---

## Reporting point

n = 100 readings, the same reporting point as Hypothesis I.

---

## What would refute this

Any hit rate at or near 50%.

We fully expect this to be refuted. We are running it because we said we would,
and because Hypothesis I is going the same way.

---

## Known problems

- There is no mechanism. None is proposed.
- One dog.
- Weekly returns on a single asset are extremely noisy. Even a real effect
  would be hard to detect at this sample size, and there is no real effect.
- The observer is not blind, is not disinterested, and holds SOL.
- Roughly fourteen weeks of data will exist at n=100. Fourteen coin flips.

---

## Data collection begins

**Today, 16 August 2026.** No backfill.

Historical SOL prices are public and backfilling would be legitimate, but
starting clean is simpler and there is nothing to argue about.

A `sol_close` column is added to readings.csv from this date. Rows before today
are left blank.

---

## Commitment

These definitions will not be changed after seeing the data.

Any change will be committed separately, dated, and announced in advance —
the same rule that applies to Hypothesis I.

We are treating a joke with the same procedure as the real question. That is
deliberate. If the procedure only applies when the answer matters, it is not
a procedure.


## AMENDMENT 1 — 16 August 2026

SOL close is taken from the Close column of CoinGecko's Solana historical data
page, which applies dates in UTC. Committed before any price observations were
recorded.
