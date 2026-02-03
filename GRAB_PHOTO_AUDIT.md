# Pinky's Kitchen - Grab Photo Audit Report 🐷

**Generated:** February 3, 2026  
**Status:** ⚠️ PARTIAL - Grab menu inaccessible via desktop

---

## ⚠️ Important Limitation

**The Grab link cannot be accessed via desktop browser:**
- URL: `https://r.grab.com/g/6-20260203_220915_...`
- This is a mobile deep link designed to open the Grab app
- When accessed via browser, it redirects to generic GrabFood marketing page
- The food.grab.com restaurant pages require mobile access or location data

**Action Required:** Someone needs to manually check the Grab app on their phone to compare photos.

---

## Website Image Inventory

### Current Photos (dish1-8.jpg)

| File | Description | Currently Used For | Suitable For |
|------|-------------|-------------------|--------------|
| **dish1.jpg** | Two wooden boxes with BBQ pork + rice on cutting board, "Have a nice day" utensils | Pinky's Box for 2 | ✅ Perfect - shows 2 portions |
| **dish2.jpg** | Black bowl, pork slices, rice mound, cucumber, marble background, chopsticks | Juicy BBQ Pork Bowl 200g (main) | ✅ Great bowl presentation |
| **dish3.jpg** | Black bowl, pork around rice, cucumber, dark counter, wooden board visible | Juicy BBQ Pork Bowl 150g (main) | ✅ Good bowl variation |
| **dish4.jpg** | Black plate, sliced BBQ pork, cucumber, NO rice, wooden board | Juicy BBQ Pork 150g | ✅ Correct - pork only |
| **dish5.jpg** | Close-up thick sliced pork on wooden board, no rice/sides | Juicy BBQ Pork 200g | ✅ Correct - pork only, larger portion visible |
| **dish6.jpg** | Black bowl, large portion pork with rice, no cucumber visible | Coming Soon - Chicken Thigh | ⚠️ ISSUE - This is pork, not chicken! |
| **dish7.jpg** | Black bowl, BBQ pork + rice, chopsticks, wooden board | Coming Soon - Chicken Bowl | ⚠️ ISSUE - This is pork, not chicken! |
| **dish8.jpg** | Rustic wooden board, pork + rice + cucumber, palm leaf background | Garden Grill Board | ✅ Perfect - matches "garden/rustic" description |

### Image Assignments in Code

```javascript
// Current menu item → images mapping:
"Juicy BBQ Pork Bowl 200g"   → [dish2, dish3, dish6] 
"Juicy BBQ Pork Bowl 150g"   → [dish3, dish2, dish8]
"Juicy BBQ Pork 200g"        → [dish5, dish4]
"Juicy BBQ Pork 150g"        → [dish4, dish5]
"Garden Grill Board"         → [dish8, dish2]
"Pinky's Box for 2"          → [dish1, dish2, dish3]

// Coming Soon (problematic):
"Juicy BBQ Chicken Thigh"    → [dish6]  ⚠️ Shows pork!
"Juicy BBQ Chicken Bowl"     → [dish7]  ⚠️ Shows pork!
```

---

## Photo Analysis Summary

### ✅ Items That Look Correct

| Menu Item | Image Match |
|-----------|-------------|
| Juicy BBQ Pork Bowl 200g | dish2.jpg - Full bowl with generous pork portion |
| Juicy BBQ Pork Bowl 150g | dish3.jpg - Slightly smaller appearance |
| Juicy BBQ Pork 200g | dish5.jpg - Large pork-only portion |
| Juicy BBQ Pork 150g | dish4.jpg - Medium pork-only with cucumber |
| Garden Grill Board | dish8.jpg - Rustic outdoor presentation |
| Pinky's Box for 2 | dish1.jpg - Clearly shows two portions |

### ⚠️ Potential Issues

1. **Coming Soon Chicken Items**
   - dish6.jpg and dish7.jpg clearly show **pork**, not chicken
   - These are placeholder images for unreleased chicken items
   - **Recommendation:** Either mark more clearly as "illustration" or wait for real chicken photos

2. **Photo Reuse**
   - dish2.jpg and dish3.jpg are used across multiple items
   - This is normal for similar items but may confuse customers
   - **Recommendation:** Consider unique hero shots for each main item

3. **200g vs 150g Differentiation**
   - Hard to visually distinguish portion sizes in photos
   - **Recommendation:** Add visual scale reference (plate size, rice amount)

---

## What's Needed for Grab Verification

To complete this audit, please manually check these items on the Grab app:

### Checklist for Grab App Verification

- [ ] **Menu Categories** - What categories exist on Grab?
- [ ] **Item Names** - Do they match website exactly?
- [ ] **Prices** - Are all prices current?
- [ ] **Photos** - Which items have photos on Grab?
- [ ] **Photo Quality** - Are Grab photos same as website?
- [ ] **Missing Items** - Any items on Grab not on website?
- [ ] **Item Descriptions** - Do descriptions match?

### How to Check

1. Open Grab app on phone
2. Go to GrabFood section
3. Search "Pinky's Kitchen" or use the link from the website
4. Screenshot each menu item
5. Compare with website at https://warwideweb.github.io/pinkys/

---

## Recommendations

### Immediate Actions

1. **Get Real Chicken Photos** 🐣
   - When chicken items launch, photograph them properly
   - Don't use pork photos for chicken products

2. **Verify Grab Photos Match Website** 📱
   - Someone with Grab app needs to compare
   - Ensure uploaded photos match current website images

3. **Consider Photo Upgrades** 📸
   - Current photos are good quality but similar angles
   - Lifestyle shots, hand-held, steam/sizzle effects could help

### Future Enhancements

- **Photo CDN:** Consider using Grab's actual CDN URLs for consistency
- **A/B Testing:** Test which photos perform better on each platform
- **Seasonal Updates:** Refresh photos periodically to keep content fresh

---

## Current Menu Structure

### Website Menu (from index.html)

**Signature Bowls:**
| Item | Thai Name | Price |
|------|-----------|-------|
| Juicy BBQ Pork Bowl 200g | ข้าวบาบีคิวคอหมูย่างนุ่มฉ่ำ | ฿279 |
| Juicy BBQ Pork Bowl 150g | ข้าวบาบีคิวคอหมูย่างนุ่มฉ่ำ | ฿239 |
| Juicy BBQ Pork 200g | บาบีคิวคอหมูย่างนุ่มฉ่ำ | ฿269 |
| Juicy BBQ Pork 150g | บาบีคิวคอหมูย่างนุ่มฉ่ำ | ฿229 |
| Garden Grill Board | หมูย่างสไตล์สวน | ฿249 |
| Pinky's Box for 2 | เซ็ทคู่สุดคุ้ม | ฿459 |

**Coming Soon:**
| Item | Thai Name | Price |
|------|-----------|-------|
| Juicy BBQ Chicken Thigh | สะโพกไก่ย่างบาบีคิวนุ่มฉ่ำ | ฿189 |
| Juicy BBQ Chicken Thigh Bowl | ข้าวบาบีคิวสะโพกไก่ย่างนุ่มฉ่ำ | ฿199 |

**Drinks:**
| Item | Thai Name | Price |
|------|-----------|-------|
| Coke Zero | โค้กซีโร่ | ฿40 |
| Aura Water 500ml | น้ำออร่า | ฿30 |

---

## Files Reference

```
/projects/pinkys/images/
├── dish1.jpg     (162KB) - Box for 2
├── dish2.jpg     (136KB) - 200g Bowl (hero)
├── dish3.jpg     (144KB) - 150g Bowl (hero)
├── dish4.jpg     (174KB) - 150g Pork only
├── dish5.jpg     (186KB) - 200g Pork only
├── dish6.jpg     (129KB) - ⚠️ Pork (used for chicken)
├── dish7.jpg     (170KB) - ⚠️ Pork (used for chicken)
├── dish8.jpg     (190KB) - Garden Grill Board
├── logo.png      (359KB) - Main logo
├── pig-regular.png    - Mascot
├── pig-showercap.png  - Loading mascot
├── grab-icon.png      - Grab button
└── line-icon.png      - LINE button
```

---

## Summary

| Status | Count |
|--------|-------|
| ✅ Photos Match Intent | 6 items |
| ⚠️ Placeholder/Wrong | 2 items (chicken coming soon) |
| ❓ Needs Grab Verification | All items |

**Next Step:** Manual verification via Grab app required to complete audit.

---

*Report generated by OpenClaw AI - February 3, 2026* 🐷💕
