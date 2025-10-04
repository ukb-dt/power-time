# A
Locked to **scale-only**, rounded to **2×10^N** blocks. Units per your spec.

|  Code | Tier (who/what)        | Unit | Canon size (per **day**)     | Count relations (ballpark) |
| ----: | ---------------------- | ---- | ---------------------------- | -------------------------- |
| **P** | Person                 | kWh  | **2×10⁰ kWh**  ≈ **2 kWh**   | ~1/10 of H                 |
| **H** | Household              | kWh  | **2×10¹ kWh**  ≈ **20 kWh**  | ~10× P                     |
| **F** | Firm (SME block)       | MWh  | **2×10⁰ MWh**  ≈ **2 MWh**   | ~100× H                    |
| **C** | City / Gov block       | GWh  | **2×10⁰ GWh**  ≈ **2 GWh**   | **US = 1,000 × C**         |
| **S** | Hyperscalers (“super”) | GWh  | **2×10² GWh**  ≈ **200 GWh** | **S = 100 × C**            |
| **W** | World (electricity)    | TWh  | **2×10¹ TWh**  ≈ **20 TWh**  | ≈ 10–50 × US (scale-only)  |

Tiny legend: everything is snapped to **2×10^N** (so 30 → use **20**).
This keeps head math clean while preserving the staircase: **P→H→F→C→S→W**.

Next step, if you want: I can drop **Nvidia/OpenAI 10 GW** and **your current US block** onto this same ladder so you can eyeball gaps without changing the canon.

# B
Yebo. Dropping **Nvidia/OpenAI 10 GW** and the **US block** onto your canon, staying strict to your **2×10^N** ladder and daily units.

### Overlay (daily, rounded to 2×10^N where defined)

|            Code | Tier                       |                                Canon size | Relation in **C**-blocks | Relation to others                              |
| --------------: | -------------------------- | ----------------------------------------: | -----------------------: | ----------------------------------------------- |
|           **C** | City/Gov block             |                 **2×10⁰ GWh = 2 GWh/day** |                  **1 C** | —                                               |
|           **S** | Hyperscaler block          |               **2×10² GWh = 200 GWh/day** |                **100 C** | —                                               |
|          **US** | United States (by fiat)    | **2×10⁰ TWh = 2 TWh/day = 2,000 GWh/day** |              **1,000 C** | **US = 10 × S**                                 |
|           **W** | World (electricity)        |                **2×10¹ TWh = 20 TWh/day** |             **10,000 C** | **W = 10 × US**                                 |
| **10 GW fleet** | Nvidia/OpenAI (continuous) |                         **≈ 240 GWh/day** |              **≈ 120 C** | **≈ 1.2 × S**, **≈ 0.12 × US**, **≈ 0.012 × W** |

Quick reads:

* **10 GW ≈ 240 GWh/day** → basically **one S-block** with a 20% hat.
* **US = 2 TWh/day (canon)** → **≈ 10 hyperscalers** of this size.
* **World = 20 TWh/day (canon)** → **≈ 83 hyperscalers** or **10 US blocks**.

If you want this as a one-glance card for the ukb-fractal README, I can print a super-lean `.md` or `.html` snippet using only these numbers (no decimals, all 2×10^N).

# C
