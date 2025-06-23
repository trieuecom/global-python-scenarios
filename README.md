# 🌏 Global Programming Assignment: Japan, Australia & Morocco (Python)

## 🎯 Project Overview

This Python project includes three themed programming challenges simulating distinct real-world and fantasy scenarios:
- 🗾 **Japan**: Reforge an imperfect katana to match a master design
- 🦘 **Australia**: Relocate animals across states to avoid threats
- 🕌 **Morocco**: Strategically purchase spices under dynamic pricing

Each problem emphasizes **file I/O**, **object-oriented design**, and **recursive strategies**.

---

## 🇯🇵 Japan: Katana Reforging

Simulates a blacksmith evaluating and reforging a katana blade to meet a required **similarity score**.

### 🔧 Features
- Reads `.bp` files containing blueprint designs
- Compares blade segments using line-wise `#` count
- Prompts user to reforge by entering custom blade shapes
- Validates and rewrites the blueprint while preserving handle structure

### 🧪 Example

- Similarity score: 0.62
- Denied: You must reforge it.
- Line (1/5) [####]: 4
...
- Similarity score: 0.93
- Accepted: The blacksmith is satisfied.


---

## 🇦🇺 Australia: Animal Relocation

Simulates the **safe relocation** of animals across Australian states. Each animal has a **threat** and a **habitat**.

### 🦘 Constraints
- No two animals can share the same state
- Animals must not be adjacent to their threats (based on adjacency map)

### 📁 Input
CSV file: `animals.csv` with lines like:
Wombat,forest,Fox
Kangaroo,grassland,Dingo


### 🔧 Features
- Object-oriented animal representation
- Fixed relocation order: `NSW → QLD → VIC → TAS → SA → NT → WA`
- Automatically skips invalid placements

---

## 🇲🇦 Morocco: Spice Trade Strategy

Implements a **recursive algorithm** to find the cheapest order to buy 9 spices under a dynamic pricing model.

### 💸 Dynamic Pricing Model
Price depends on:
- The previously purchased spice
- The student ID's last digit
- Spice position in the order

### 🧠 Logic
- Validates 9-digit student ID
- Recursively tries all permutations of spice orders
- Returns the cheapest valid purchase order within budget

---

## 🧪 Sample Functions

- `calculate_spice_price(...)`: Computes adjusted price based on rules
- `purchase_spices(...)`: Recursive function to find optimal order
- `get_similarity_score(...)`: Computes average similarity between katanas
- `relocate_animals(...)`: Places animals respecting adjacency constraints

---

## 📂 Repository Structure

| File | Description |
|------|-------------|
| `Japan.zip` | `japan.py`, `my_katana.bp`, `perfect_katana.bp` | Katana blueprint reforging logic and blade similarity comparison |
| `Australia.zip` | `australia.py`, `animals.csv` | Fictional animal relocation logic with threat avoidance |
| `Morocco.zip` | `morocco.py`, `test_morocco.py`, `test_plan.md` | Spice purchase optimization with recursion, test cases, and test planning |


## 🛠️ Tools Used

- Python 3.10+
- Standard libraries only (`sys`, `os`, `math`)
- No external dependencies






