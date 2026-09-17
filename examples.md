# Example texts for the De-Identification Checker

Copy and paste each example into the [De-Identification Checker](deid-checker.html) to see what it flags.

---

## Example 1 - Looks safe but isn't (Tier 4)

```
Weekly medical update from our team in El Fasher. This week we treated 3 children with severe acute malnutrition at the clinic in Kutum (13.6293, 25.3493). The Zaghawa community has been particularly affected. Patient Amina Ibrahim, aged 4, from the village of Fata Borno, was admitted on 12 March with complications. We also treated 2 women for injuries consistent with sexual assault. One gunshot wound patient was stabilized and transferred.
```

**Why this is Tier 4:** GPS coordinates of a health facility in active conflict. Named patient (Amina Ibrahim) with age, village, and admission date. Ethnic group named (Zaghawa). Sexual violence mentioned. Gunshot wound implies possible combatant. Small denominator (3 children) in a named location makes individuals identifiable.

---

## Example 2 - Partially de-identified but still risky (Tier 3, possibly Tier 4)

```
In the northern sector, our facility treated 147 cholera cases this month with a case fatality rate of 2.1%. Pediatric malnutrition admissions rose 40% compared to last quarter. We also saw 6 patients with blast injuries and 4 cases of measles in children under 5. The attack rate in the eastern camp remains above emergency threshold at 8.2 per 1000 per week.
```

**Why this is still risky:** No names or GPS, but "6 patients with blast injuries" is a small denominator in a single facility - potentially identifiable. "Northern sector" and "eastern camp" may narrow location enough for someone with local knowledge. Blast injuries imply conflict-related trauma. The combination of specific case counts, injury types, and location descriptors could enable a motivated intruder to identify individuals.

---

## Example 3 - Actually safe (Tier 0)

```
Overall cholera response across the region has reached 12,400 consultations this quarter. Oral rehydration points have been established in 23 locations. Vaccination coverage in accessible areas has reached 78%. The organization continues to advocate for unimpeded humanitarian access to all affected populations.
```

**Why this is safe:** Large aggregate numbers (12,400 consultations). No facility-level data. No individual counts small enough to enable re-identification. No geographic precision. No protected attributes. This text can be safely processed through any commercial LLM.
