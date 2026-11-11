
Readme · MD
# 🛰️ Habitat Layout Creator
 
**Team Orbitecture** · STARFORGE 24-Hour Hackathon, BMSIT&M · Problem **SW-4** · Software Track
 
Design the inside of a space habitat, check it against NASA-based rules, and fix every mistake in one click.
 
▶ **Demo video:** [Watch on Google Drive](https://drive.google.com/file/d/1WtVOYcYrcFb3MPiV2Yn8HzfsssDHFBBp/view?usp=drivesdk)
 
---
 
## 🚀 The problem
 
Planning where the beds, gym, kitchen, toilets and storage go in a spacecraft is slow and costly. Mistakes are often found late, for example:
 
- a noisy gym next to the beds
- a blocked exit
- not enough living space for the crew
These mistakes are expensive to fix after the design is done.
 
## 💡 Our solution
 
A web page where anyone can:
 
1. **Describe the mission**: crew size, number of days, habitat shape, size, deck height and decks.
2. **Paint the layout** on a 1 m grid: sleep, exercise, hygiene, food/galley, work, medical, storage, life support, hatches and corridors.
3. **Get a score out of 100** right away, with a clear reason and a NASA source for every problem.
4. **Click Auto-fix** to repair all the mistakes and reach 100.
---
 
## ✨ Features
 
| Feature | What it does |
|---|---|
| **Live score (0–100)** | 6 checks: volume per crew, zone sizes, neighbours, noise, emergency exits, space use |
| **Extra safety tests** | Radiation storm shelter and blocked-hatch escape (not part of the score) |
| **Load good example** | Builds a 100-score layout for your exact mission settings |
| **Load flawed example** | Builds the same layout with typical mistakes, to practise on |
| **✨ Auto-fix** | Fixes whatever is wrong, step by step, and shows a before/after |
| **Real spacecraft shapes** | ISS-style station, Starship, Skylab, Bigelow B330, plus rectangle, cylinder, dome, ring and L-shape |
| **Multiple decks** | Stack decks with ladders between them |
| **Views** | 2D grid, noise map, exit paths and a 3D view |
| **🚀 Which spacecraft fits?** | Tests 11 spacecraft options and picks the cheapest one that scores 100 |
| **🔗 Share link & 🔀 Merge deck** | Teamwork: each person designs a deck, shares a link, and the decks are merged into one habitat |
| **Save & compare** | Save layouts and compare them side by side |
| **Cost estimate** | Rough mass and launch cost of the habitat |
| **Export / Import JSON, 📄 PDF report** | Keep or share your work |
| **Undo, Help tour, works on phones** | Easy to use for beginners |
 
### Habitat shapes
 
- **ISS-style station:** joined modules (Unity, Destiny, Harmony, Columbus, Kibo, Tranquility, Quest), sizes 1–5
- **Starship-style:** 9 m wide, 1–3 stacked decks, and the nose narrows at the top
- **Skylab-style:** NASA 1973, 2 decks, 6.6 m × 14.6 m
- **Bigelow B330-style:** inflatable, 330 m³
- **Basic shapes:** rectangular module, cylinder, inflatable dome, torus/ring, L-shape
---
 
## 📏 How a layout is scored
 
The score is out of 100 and has six checks:
 
1. **Volume per crew:** enough living space for each person, based on mission length.
2. **Zone sizes:** each zone is big enough for the crew.
3. **Neighbours:** zones that belong together are close; zones that clash are apart.
4. **Noise:** loud zones (exercise) are kept away from quiet ones (sleep).
5. **Emergency exits:** enough hatches, and every box is close to one.
6. **Space use:** enough walkway, without wasting space.
There are also two **extra safety tests**, which are not part of the score:
 
- **Radiation storm shelter:** NASA asks for an extra 10 cm of water (≈ 10 g/cm²) around the crew during solar storms. A side of a bed is shielded when the supplies between the bed and the hull give ≥ 10 g/cm². We estimate 1 m of storage ≈ 25 and 1 m of life support ≈ 20. The test passes when 75% of beds have 2 or more shielded sides.
- **Blocked hatch:** if any one hatch is blocked, everyone can still escape.
---
 
## 🛠️ Tech used
 
- **HTML, CSS and JavaScript** in a single file (`index.html`)
- **No server, no install, no libraries.** It works offline in any modern browser, on a laptop or a phone.
- **2D grid and 3D view** drawn in the browser
- **Saved layouts** are kept in the browser's local storage
---
 
## ▶️ How to run
 
1. Download or clone this repository.
2. Open **`index.html`** in Chrome, Edge or Firefox.
That's it.
 
**Quick try:**
1. Pick a shape and crew size.
2. Click **Load flawed example**.
3. Click **✨ Auto-fix**, and the score goes to **100**.
---
 
## 📁 Files
 
| File | What it is |
|---|---|
| `index.html` | The full app |
| `Orbitecture_SW-4_Habitat_Layout_Creator.pptx` / `.pdf` | Pitch deck |
| `README.md` | This file |
 
---
 
## 📚 Main sources
 
- NASA-STD-3001 (crew health and habitability) and NASA habitable volume studies
- NASA-STD-3001 radiation technical brief (vehicle ≥ 20 g/cm², storm shelter + 10 cm water)
- NASA ECLSS (life support) fact sheet
- NASA ISS module fact sheets (Unity, Destiny, Harmony, Tranquility, Quest), plus ESA Columbus and JAXA Kibo
- NASA / Smithsonian: Skylab Orbital Workshop
- SpaceX Starship and Falcon Heavy published figures
- Bigelow Aerospace B330
*Some values (shielding per metre, costs) are estimates for design comparison, not flight data.*
 
---
 
## 👩‍💻 Built by
 
**Shravani VU** ([@shravanivu1207](https://github.com/shravanivu1207))
 
Team Orbitecture · Made for **STARFORGE 2026 · BMS Institute of Technology and Management**
 

