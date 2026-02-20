# DATA SCIENCE - QUICK NOTES (THANGLISH)

---

## PART-A (2 MARKS)

### 1. Data Science Tools

**Popular Tools:**
- **Python:** Pandas, NumPy, Scikit-learn
- **R:** Statistical analysis
- **SQL:** Database queries
- **Tableau:** Visualization
- **Excel:** Basic analysis
- **Jupyter:** Notebook environment

---

### 2. Pareto Diagram

**Definition:** Bar chart + line graph showing 80-20 rule.

**Purpose:** Most significant factors identify panna.

**Example:** 80% problems 20% causes la irundhu varum.

---

### 3. Data Warehouse

**Definition:** Large storage system - multiple sources la irundhu data collect panni store panrum for analysis.

**Features:**
- Historical data store
- Integrated from multiple sources
- Query & analysis ku optimized

---

### 4. External Data

**Definition:** Organization-ku velila irundhu vara data.

**Examples:**
- Market research reports
- Government statistics
- Social media data
- Weather data
- Competitor information

---

### 5. Nominal & Ordinal Variables

| Type | Definition | Example |
|------|------------|---------|
| **Nominal** | Categories (no order) | Color, Gender, City |
| **Ordinal** | Categories (with order) | Ranks, Ratings, Education level |

---

### 6. Variability Example

**Definition:** Data points spread out aana level.

**Example:**
```
Class A scores: 70, 72, 71, 69, 73 (Low variability)
Class B scores: 50, 90, 60, 85, 40 (High variability)
```

**Measures:** Range, Variance, Standard Deviation

---

### 7. Types of Data

**1. Qualitative (Categorical):**
- Nominal: Gender, Color
- Ordinal: Rating, Grade

**2. Quantitative (Numerical):**
- Discrete: Count (students = 30)
- Continuous: Measurement (height = 5.7ft)

---

### 8. Data Table vs Graph

| Data Table | Graph |
|------------|-------|
| Numbers la display | Visual representation |
| Exact values | Patterns & trends |
| Detailed | Quick understanding |
| Example: Spreadsheet | Example: Bar chart, Pie chart |

---

### 9. Correlation

**Definition:** Two variables ku idaila relationship measure panradhu.

**Range:** -1 to +1
- **+1:** Perfect positive (one increase → other increase)
- **-1:** Perfect negative (one increase → other decrease)
- **0:** No relationship

---

### 10. Regression

**Definition:** Dependent variable predict panna independent variables use panra technique.

**Example:** House price (dependent) predict using size, location (independent).

**Formula:** y = mx + c

---

## PART-B (13 MARKS)

### 11A. Types of Data (Detailed)

#### **1. Qualitative Data (Categorical):**

**A. Nominal Data:**
- **Definition:** Categories without order
- **Properties:** Cannot add/subtract, only count
- **Examples:**
  - Gender: Male, Female, Other
  - Blood group: A, B, AB, O
  - City: Chennai, Mumbai, Delhi
  - Color: Red, Blue, Green

**Operations:** Frequency count, Mode

---

**B. Ordinal Data:**
- **Definition:** Categories with meaningful order
- **Properties:** Rank exist, but intervals not equal
- **Examples:**
  - Education: Primary < Secondary < Graduate < Post-graduate
  - Satisfaction: Very Dissatisfied < Dissatisfied < Neutral < Satisfied < Very Satisfied
  - Movie rating: 1 star < 2 star < 3 star < 4 star < 5 star
  - Economic status: Low < Middle < High

**Operations:** Median, Mode, Percentile

---

#### **2. Quantitative Data (Numerical):**

**A. Discrete Data:**
- **Definition:** Countable, whole numbers
- **Properties:** Gaps between values
- **Examples:**
  - Number of students: 25, 30, 35
  - Number of cars: 2, 3, 4
  - Dice roll: 1, 2, 3, 4, 5, 6
  - Items sold: 100, 150, 200

**Operations:** All statistics (mean, median, mode, SD)

---

**B. Continuous Data:**
- **Definition:** Measurable, any value possible
- **Properties:** No gaps, infinite precision
- **Examples:**
  - Height: 5.7ft, 5.75ft, 5.751ft
  - Weight: 60.5kg, 60.52kg
  - Temperature: 25.3°C, 25.35°C
  - Time: 10.5 seconds, 10.523 seconds

**Operations:** All statistics, graphs

---

#### **Comparison Table:**

| Type | Order | Math Ops | Example |
|------|-------|----------|---------|
| **Nominal** | No | Count only | Gender |
| **Ordinal** | Yes | Count, Rank | Rating |
| **Discrete** | Yes | All | Students count |
| **Continuous** | Yes | All | Height |

---

**Data Hierarchy:**
```
Nominal < Ordinal < Discrete < Continuous
(Less info)              (More info)
```

---

### 11B. Data Warehousing

#### **Definition:**
Central repository - multiple sources la irundhu data collect, store, analyze panna system.

---

#### **Architecture (3 Layers):**

**1. Bottom Layer (Data Sources):**
```
Operational DBs → ETL → Data Warehouse
External data   →     →
Legacy systems  →     →
```

**ETL Process:**
- **Extract:** Data sources la irundhu collect
- **Transform:** Clean, format, integrate
- **Load:** Warehouse-la store

---

**2. Middle Layer (Data Warehouse Server):**
- **OLAP Server:** Fast queries
- **Metadata:** Data about data
- **Data Mart:** Department-specific subset

---

**3. Top Layer (Frontend/Tools):**
- Query tools
- Reporting tools
- Analysis tools (OLAP)
- Data mining tools

---

#### **Components:**

**1. Data Warehouse Database:**
- Fact tables: Metrics store
- Dimension tables: Context (time, location)

**2. ETL Tools:**
- Informatica, Talend, SSIS

**3. Metadata:**
- Technical metadata: Table structure
- Business metadata: Definitions

**4. Query Tools:**
- SQL, MDX

**5. Data Marts:**
- Sales mart, Finance mart, HR mart

---

#### **Applications:**

**1. Business Intelligence:**
- Sales analysis: Trends, forecasts
- Customer segmentation
- Performance dashboards

**2. Decision Making:**
- Historical trend analysis
- What-if scenarios
- Predictive analytics

**3. Industry Examples:**
- **Retail:** Inventory optimization, customer behavior
- **Banking:** Fraud detection, risk analysis
- **Healthcare:** Patient records, treatment outcomes
- **Telecom:** Network performance, customer churn

---

### 12A. Data Mining Architecture

#### **Components:**

**1. Data Sources:**
```
Databases → Data Mining Engine
Files     →
Web data  →
```

---

**2. Data Warehouse Server:**
- Integrated data storage
- Pre-processed data
- Historical data

---

**3. Data Mining Engine:**
**Core Functions:**
- **Association:** Pattern discover (Market Basket Analysis)
- **Classification:** Category predict (Email spam/not spam)
- **Clustering:** Group similar items (Customer segments)
- **Regression:** Value predict (Sales forecast)

---

**4. Pattern Evaluation Module:**
- Interesting patterns filter
- Threshold apply
- Noise remove

---

**5. Graphical User Interface:**
- User queries
- Results visualization
- Interactive exploration

---

**6. Knowledge Base:**
- Domain knowledge
- Concept hierarchies
- Interestingness measures

---

#### **Process Flow:**
```
Data Sources → Data Warehouse → Data Cleaning → 
Data Mining Engine → Pattern Evaluation → Knowledge Base
```

---

**Example: Supermarket Data Mining**
```
Data: Customer purchases
Mining: "Bread buyers 70% buy milk"
Action: Place items together
Result: Increased sales
```

---

### 12B. Facets of Data

#### **1. Structured Data:**
**Definition:** Organized format (tables, rows, columns)

**Properties:**
- Well-defined schema
- Easy to search
- Relational database

**Examples:**
- Excel spreadsheets
- SQL databases
- CSV files

**Format:**
```
ID | Name | Age | City
1  | Ram  | 25  | Chennai
2  | Sita | 22  | Mumbai
```

---

#### **2. Unstructured Data:**
**Definition:** No predefined format

**Properties:**
- No schema
- Hard to search
- Requires preprocessing

**Examples:**
- Text documents
- Images, videos
- Social media posts
- Emails

**Challenge:** 80% of data unstructured

---

#### **3. Semi-Structured Data:**
**Definition:** Some organization but not full table format

**Examples:**
- JSON: `{"name": "Ram", "age": 25}`
- XML: `<person><name>Ram</name></person>`
- Logs files

---

#### **4. Metadata:**
**Definition:** Data about data

**Example:**
- Photo: Date taken, location, camera model
- Document: Author, creation date, file size

---

#### **5. Big Data Facets (5 V's):**

**Volume:** Large amount (TBs, PBs)

**Velocity:** Fast generation (social media posts per second)

**Variety:** Different types (structured, unstructured)

**Veracity:** Data quality, accuracy

**Value:** Useful insights extract pannalam

---

### 13A. Normal Curve & Z-Score

#### **Normal Distribution (Bell Curve):**

**Shape:**
```
         Peak (Mean)
          /\
         /  \
        /    \
       /      \
_____ /        \ _____
    μ
```

**Properties:**
- Symmetric around mean (μ)
- Mean = Median = Mode
- 68% data within 1 SD
- 95% data within 2 SD
- 99.7% data within 3 SD

---

#### **Z-Score:**

**Formula:**
```
Z = (X - μ) / σ

Where:
X = Data point
μ = Mean
σ = Standard Deviation
```

**Meaning:**
- Z = 0: Value at mean
- Z = +1: One SD above mean
- Z = -1: One SD below mean

---

**Example:**
```
Test scores: μ = 70, σ = 10
Student score: X = 85

Z = (85 - 70) / 10 = 1.5

Interpretation: 1.5 SD above average
```

---

**Applications:**
- Compare different distributions
- Find percentiles
- Identify outliers (|Z| > 3)

---

### 13B. Four Types of Descriptive Statistics

#### **1. Measures of Central Tendency:**

**A. Mean (Average):**
```
Mean = Sum of all values / Count

Example:
Scores: 70, 80, 90, 60, 75
Mean = (70+80+90+60+75)/5 = 75
```

**B. Median (Middle Value):**
```
Arrange in order, pick middle

Example:
60, 70, 75, 80, 90
Median = 75 (middle value)
```

**C. Mode (Most Frequent):**
```
Example:
Scores: 70, 80, 80, 90, 80
Mode = 80 (appears 3 times)
```

---

#### **2. Measures of Variability:**

**A. Range:**
```
Range = Maximum - Minimum

Example:
Scores: 60, 70, 80, 90
Range = 90 - 60 = 30
```

**B. Variance:**
```
Average of squared differences from mean

Example:
Scores: 10, 12, 14
Mean = 12
Variance = [(10-12)² + (12-12)² + (14-12)²]/3
         = [4 + 0 + 4]/3 = 2.67
```

**C. Standard Deviation:**
```
SD = √Variance = √2.67 = 1.63
```

---

#### **3. Measures of Position:**

**Percentiles:**
```
25th percentile (Q1): 25% below this
50th percentile (Q2): Median
75th percentile (Q3): 75% below this
```

**Example:** 90th percentile = score better than 90% students

---

#### **4. Measures of Shape:**

**Skewness:**
- **Positive skew:** Tail right side (Mean > Median)
- **Negative skew:** Tail left side (Mean < Median)
- **Symmetric:** Mean = Median

**Kurtosis:** Peak sharpness measure

---

### 14A. Types of Variables with Examples

#### **1. Independent Variable (Predictor):**
**Definition:** Variable we control/change

**Examples:**
- Study hours (to predict exam score)
- Advertising budget (to predict sales)
- Temperature (to predict ice cream sales)

**Symbol:** Usually X

---

#### **2. Dependent Variable (Response):**
**Definition:** Variable we measure/observe

**Examples:**
- Exam score (depends on study hours)
- Sales (depends on advertising)
- Ice cream sales (depends on temperature)

**Symbol:** Usually Y

---

#### **3. Categorical Variables:**

**A. Nominal:**
```
Example: Blood Type
Categories: A, B, AB, O
No order
```

**B. Ordinal:**
```
Example: Customer Satisfaction
Categories: Very Dissatisfied, Dissatisfied, Neutral, Satisfied, Very Satisfied
Order exists
```

---

#### **4. Numerical Variables:**

**A. Discrete:**
```
Example: Number of Children
Values: 0, 1, 2, 3, 4
Whole numbers only
```

**B. Continuous:**
```
Example: Height
Values: 165.5cm, 165.75cm, 165.752cm
Any value possible
```

---

#### **5. Confounding Variable:**
**Definition:** Affects both independent & dependent

**Example:**
- Study: Coffee → Better concentration
- Confounding: Sleep hours (affects both)

---

### 14B. Finding Z-Score

#### **Formula:**
```
Z = (X - μ) / σ
```

---

#### **Given Information:**
- X = Data point value
- μ (mu) = Mean
- σ (sigma) = Standard Deviation

---

#### **Step-by-Step Process:**

**Step 1:** Identify values
```
X = data point
μ = mean
σ = SD
```

**Step 2:** Subtract mean from X
```
Difference = X - μ
```

**Step 3:** Divide by SD
```
Z = Difference / σ
```

---

#### **Examples:**

**Example 1:**
```
Given:
Mean (μ) = 100
SD (σ) = 15
Find Z for X = 115

Solution:
Z = (115 - 100) / 15
Z = 15 / 15
Z = 1

Meaning: 1 SD above mean
```

---

**Example 2:**
```
Given:
Mean (μ) = 50
SD (σ) = 5
Find Z for X = 40

Solution:
Z = (40 - 50) / 5
Z = -10 / 5
Z = -2

Meaning: 2 SD below mean
```

---

**Example 3:**
```
Given:
Mean (μ) = 75
SD (σ) = 10
Find Z for X = 75

Solution:
Z = (75 - 75) / 10
Z = 0 / 10
Z = 0

Meaning: Exactly at mean
```

---

#### **Interpretation:**

| Z-Score | Meaning |
|---------|---------|
| 0 | At mean |
| +1 | 1 SD above |
| -1 | 1 SD below |
| +2 | 2 SD above |
| -2 | 2 SD below |
| > +3 | Outlier (very high) |
| < -3 | Outlier (very low) |

---

### 15A. i) Scatter Plot

#### **Definition:**
Graph showing relationship between two variables (X and Y axis la points).

---

#### **Components:**
- **X-axis:** Independent variable
- **Y-axis:** Dependent variable
- **Points:** Each data pair

---

#### **Types of Relationships:**

**1. Positive Correlation:**
```
   Y
   |     ●
   |   ●
   | ●
   |_______ X
   
X increase → Y increase
Example: Study hours vs Marks
```

---

**2. Negative Correlation:**
```
   Y
   | ●
   |   ●
   |     ●
   |_______ X
   
X increase → Y decrease
Example: Speed vs Time
```

---

**3. No Correlation:**
```
   Y
   | ● ●
   |  ●  ●
   | ●  ●
   |_______ X
   
Random pattern
Example: Shoe size vs IQ
```

---

#### **Uses:**
- Relationship identify
- Outliers spot
- Correlation strength visualize

---

### 15A. ii) Range & Variance

#### **Range:**

**Formula:**
```
Range = Maximum value - Minimum value
```

**Example:**
```
Data: 10, 15, 20, 25, 30

Range = 30 - 10 = 20
```

**Meaning:** Data spread out aana width.

**Limitation:** Outliers affect aggressively

---

#### **Variance:**

**Formula:**
```
σ² = Σ(X - μ)² / N

Where:
X = each value
μ = mean
N = count
```

---

**Calculation Steps:**

**Example:** Data: 4, 8, 6, 5, 7

**Step 1: Find Mean**
```
μ = (4+8+6+5+7)/5 = 30/5 = 6
```

**Step 2: Find Deviations**
```
4-6 = -2
8-6 = +2
6-6 = 0
5-6 = -1
7-6 = +1
```

**Step 3: Square Deviations**
```
(-2)² = 4
(+2)² = 4
(0)² = 0
(-1)² = 1
(+1)² = 1
```

**Step 4: Average**
```
Variance = (4+4+0+1+1)/5 = 10/5 = 2
```

---

**Meaning:** Average squared distance from mean.

**Standard Deviation = √Variance = √2 = 1.41**

---

### 15B. Correlation Calculation

#### **Given Data:**
```
X (Father): 66, 68, 68, 70, 71, 72, 72
Y (Son):    68, 70, 69, 72, 72, 72, 74
```

---

#### **Formula:**
```
r = [NΣxy - (Σx)(Σy)] / √[NΣx² - (Σx)²][NΣy² - (Σy)²]
```

---

#### **Step 1: Calculate Required Values**

| X | Y | XY | X² | Y² |
|---|---|----|----|-----|
| 66 | 68 | 4488 | 4356 | 4624 |
| 68 | 70 | 4760 | 4624 | 4900 |
| 68 | 69 | 4692 | 4624 | 4761 |
| 70 | 72 | 5040 | 4900 | 5184 |
| 71 | 72 | 5112 | 5041 | 5184 |
| 72 | 72 | 5184 | 5184 | 5184 |
| 72 | 74 | 5328 | 5184 | 5476 |

---

#### **Step 2: Find Sums**
```
N = 7
Σx = 487
Σy = 497
Σxy = 34604
Σx² = 33913
Σy² = 35313
```

---

#### **Step 3: Apply Formula**

**Numerator:**
```
NΣxy - (Σx)(Σy)
= 7(34604) - (487)(497)
= 242228 - 242039
= 189
```

**Denominator Part 1:**
```
NΣx² - (Σx)²
= 7(33913) - (487)²
= 237391 - 237169
= 222
```

**Denominator Part 2:**
```
NΣy² - (Σy)²
= 7(35313) - (497)²
= 247191 - 247009
= 182
```

**Denominator:**
```
√(222 × 182) = √40404 = 201
```

---

#### **Step 4: Final Answer**
```
r = 189 / 201
r = 0.94
```

---

#### **Interpretation:**
- **r = 0.94** (very strong positive correlation)
- Father tall → Son tall aagura high probability
- 94% relationship strength

---

## PART-C (15 MARKS)

### 16A. Types of Data & Variables - Complete Analysis

#### **SECTION 1: DATA TYPES**

**A. Qualitative Data:**

**1. Nominal:**
- No natural order
- **Examples:** Gender (Male, Female), Blood type (A, B, AB, O), Marital status, Nationality
- **Operations:** Frequency count, Mode
- **Cannot:** Add, subtract, rank

**2. Ordinal:**
- Order exist, intervals not equal
- **Examples:** Education level (HS < UG < PG), Customer rating (1-5 stars), Economic class (Low, Middle, High)
- **Operations:** Median, Percentile, Mode
- **Cannot:** Calculate mean meaningfully

---

**B. Quantitative Data:**

**1. Discrete:**
- Countable whole numbers
- **Examples:** Number of students (30, 31), Cars owned (0, 1, 2), Coin tosses (Heads count)
- **Operations:** All statistics (mean, median, mode, SD, variance)
- **Graph:** Bar chart, histogram

**2. Continuous:**
- Measurable, infinite precision possible
- **Examples:** Height (170.5cm), Weight (65.75kg), Temperature (37.2°C), Time (10.25 sec)
- **Operations:** All statistics, regression
- **Graph:** Line graph, histogram

---

#### **Comparison Table:**

| Feature | Nominal | Ordinal | Discrete | Continuous |
|---------|---------|---------|----------|------------|
| **Order** | No | Yes | Yes | Yes |
| **Equal Intervals** | No | No | Yes | Yes |
| **Mean** | No | No | Yes | Yes |
| **Median** | No | Yes | Yes | Yes |
| **Addition** | No | No | Yes | Yes |
| **Fractions** | No | No | No | Yes |

---

#### **SECTION 2: VARIABLES**

**A. Based on Role:**

**1. Independent Variable (X):**
- Manipulated/controlled variable
- Predictor
- **Examples:**
  - Study hours (predict marks)
  - Fertilizer amount (predict crop yield)
  - Price (predict demand)

**2. Dependent Variable (Y):**
- Measured outcome
- Response variable
- **Examples:**
  - Marks (based on study)
  - Crop yield (based on fertilizer)
  - Demand (based on price)

**3. Confounding Variable:**
- Affects both X and Y
- Hidden factor
- **Example:** Age affects both income and health

---

**B. Based on Data Type:**

**1. Categorical:**
- **Nominal:** Unordered (Color, Gender)
- **Ordinal:** Ordered (Rating, Grade)
- **Binary:** Two values only (Yes/No, Pass/Fail)

**2. Numerical:**
- **Discrete:** Count values
- **Continuous:** Measured values

---

**C. Special Variables:**

**1. Dummy Variable:**
- Convert categorical to numerical
- **Example:** Gender → Male=1, Female=0

**2. Latent Variable:**
- Cannot directly measure
- **Example:** Intelligence, Satisfaction (measure through tests/surveys)

---

#### **SECTION 3: STATISTICAL ANALYSIS BY TYPE**

**Nominal Data:**
- **Center:** Mode only
- **Spread:** Cannot measure
- **Test:** Chi-square test
- **Example:** Gender distribution (60% M, 40% F)

**Ordinal Data:**
- **Center:** Median, Mode
- **Spread:** Percentiles, IQR
- **Test:** Mann-Whitney U test
- **Example:** Survey ratings analysis

**Discrete Data:**
- **Center:** Mean, Median, Mode
- **Spread:** Range, SD, Variance
- **Test:** t-test, ANOVA
- **Example:** Students per class comparison

**Continuous Data:**
- **Center:** Mean (preferred), Median
- **Spread:** SD, Variance, Range
- **Test:** t-test, regression, correlation
- **Example:** Height analysis

---

#### **SECTION 4: PRACTICAL APPLICATIONS**

**Business:**
- Customer segmentation (Nominal)
- Satisfaction surveys (Ordinal)
- Sales figures (Continuous)
- Product count (Discrete)

**Healthcare:**
- Blood type (Nominal)
- Pain level (Ordinal)
- Blood pressure (Continuous)
- Hospital visits (Discrete)

**Education:**
- Major field (Nominal)
- Grade (Ordinal)
- Test score (Continuous)
- Number of courses (Discrete)

---

### 16B. Correlation - Complete Analysis

#### **SECTION 1: DEFINITION & CONCEPT**

**Correlation:**
Measure of relationship strength & direction between two variables.

**Symbol:** r (correlation coefficient)

**Range:** -1 ≤ r ≤ +1

**Formula:**
```
r = Σ[(X-X̄)(Y-Ȳ)] / √[Σ(X-X̄)²·Σ(Y-Ȳ)²]

Or:

r = [NΣxy - (Σx)(Σy)] / √[NΣx²-(Σx)²][NΣy²-(Σy)²]
```

---

#### **SECTION 2: TYPES OF CORRELATION**

**A. Based on Direction:**

**1. Positive Correlation (0 < r ≤ +1):**
```
Diagram:
  Y
  |       ●
  |     ●
  |   ●
  | ●
  |________ X

Both variables same direction move
X ↑ → Y ↑

Examples:
- Height & Weight (+0.7)
- Study hours & Marks (+0.8)
- Income & Spending (+0.6)
```

---

**2. Negative Correlation (-1 ≤ r < 0):**
```
Diagram:
  Y
  | ●
  |   ●
  |     ●
  |       ●
  |________ X

Variables opposite direction move
X ↑ → Y ↓

Examples:
- Speed & Travel time (-0.9)
- Price & Demand (-0.7)
- Age & Reaction time (-0.5)
```

---

**3. No Correlation (r ≈ 0):**
```
Diagram:
  Y
  | ● ●
  |  ● ●
  | ●  ●
  |________ X

Random scatter, no pattern
X change → Y no predictable change

Examples:
- Shoe size & IQ (0.02)
- Height & Salary (0.05)
```

---

**B. Based on Strength:**

| Strength | r value | Meaning |
|----------|---------|---------|
| **Perfect** | ±1.0 | Exact relationship |
| **Very Strong** | ±0.9 to ±0.99 | Almost perfect |
| **Strong** | ±0.7 to ±0.89 | Clear pattern |
| **Moderate** | ±0.4 to ±0.69 | Noticeable |
| **Weak** | ±0.2 to ±0.39 | Slight pattern |
| **Very Weak** | ±0.01 to ±0.19 | Almost none |
| **None** | 0 | No relationship |

---

**C. Based on Linearity:**

**1. Linear Correlation:**
```
Straight line relationship
Y = mX + c
Example: Distance & Time (constant speed)
```

**2. Non-linear Correlation:**
```
Curved relationship
Example: Population growth (exponential)
```

---

#### **SECTION 3: INTERPRETATION**

**Example Interpretations:**

**r = +0.95:**
- Very strong positive
- Father height 95% son height predict pannalam
- 95% variation explain

**r = -0.80:**
- Strong negative
- Price increase → Sales decrease strongly
- 80% variation explain

**r = 0.10:**
- Very weak/no relationship
- Practically no prediction possible

---

#### **SECTION 4: CALCULATION EXAMPLE**

**Problem:** Find correlation

```
X: 10, 20, 30, 40, 50
Y: 15, 25, 35, 45, 55
```

**Solution:**

| X | Y | XY | X² | Y² |
|---|---|----|----|-----|
| 10 | 15 | 150 | 100 | 225 |
| 20 | 25 | 500 | 400 | 625 |
| 30 | 35 | 1050 | 900 | 1225 |
| 40 | 45 | 1800 | 1600 | 2025 |
| 50 | 55 | 2750 | 2500 | 3025 |

```
N = 5
Σx = 150, Σy = 175
Σxy = 6250
Σx² = 5500, Σy² = 7125

r = [5(6250) - (150)(175)] / √[5(5500)-(150)²][5(7125)-(175)²]
r = [31250 - 26250] / √[27500-22500][35625-30625]
r = 5000 / √[5000][5000]
r = 5000 / 5000
r = 1.0 (Perfect positive)
```

---

#### **SECTION 5: IMPORTANT NOTES**

**1. Correlation ≠ Causation:**
- Ice cream sales & drowning both increase (summer)
- But ice cream doesn't cause drowning
- Common cause: Hot weather

**2. Outliers Effect:**
- Single extreme point r-a drastically change pannalam
- Always check scatter plot

**3. Range Restriction:**
- Limited range → correlation underestimated
- Example: Only study top students (restricted range)

**4. Non-linear Relationships:**
- r only linear measure
- Curved relationship-ku r close to 0 aagidum even if strong relationship

---

#### **SECTION 6: APPLICATIONS**

**Business:**
- Marketing spend vs Sales
- Customer satisfaction vs Retention
- Price vs Demand

**Medicine:**
- Smoking vs Lung disease
- Exercise vs Health
- Cholesterol vs Heart disease

**Education:**
- Study time vs Performance
- Attendance vs Grades
- Sleep vs Test scores

**Finance:**
- Risk vs Return
- Stock prices correlation
- Economic indicators

---

## QUICK REVISION

**Key Concepts:**
```
Data Types: Nominal, Ordinal, Discrete, Continuous
Variables: Independent (X), Dependent (Y)
Central Tendency: Mean, Median, Mode
Variability: Range, Variance, SD
Correlation: -1 to +1
Z-score: (X - μ) / σ
```

**Important Formulas:**
```
Mean = Σx / N
Variance = Σ(x-μ)² / N
SD = √Variance
Range = Max - Min
r = [NΣxy-(Σx)(Σy)] / √[NΣx²-(Σx)²][NΣy²-(Σy)²]
```

**Quick Tips:**
1. Nominal → Count only
2. Ordinal → Rank possible
3. Discrete → Whole numbers
4. Continuous → Decimals ok
5. |r| > 0.7 → Strong correlation
6. Correlation ≠ Causation

**Exam Strategy:**
1. Tables & diagrams mandatory
2. Show all calculation steps
3. Interpret results (meaning sollunga)
4. Real-world examples give
5. Keywords bold-a highlight

**All the best! 📊**
