# Target Audience Analysis and MVP Requirements

## 1. Context and Problem Statement

Users planning an interior update—renovation, furniture shopping, or decor changes—usually face two core problems:

- They struggle to clearly express their preferences and constraints. For example, “I want it cozy and modern” does not translate into specific design decisions.
- They find it hard to visualize the final result before taking action. This often leads to reference overload, long indecision, poor purchases, and repeated explanations to designers or store consultants.

The goal of the MVP is to shorten the path from a vague idea of the desired vibe to a practical output: a structured design brief and several visual concepts. The service acts as a bridge between inspiration and an actionable plan.

## 2. Product Goal and MVP Scope

**Product goal:** quickly turn a user’s text description into a structured design brief, 2–3 interior visual concepts in a chosen style, and recommendations for key furniture/decor categories and design principles.

**MVP format:** a web service focused on one main flow:

**description → brief → visualizations → recommendations**

### 2.1 What the MVP Includes

- text input plus clarifying parameters:
  - room type
  - style/vibe
  - palette/materials
  - constraints
  - budget level
- conversion into a structured design brief:
  - readable text
  - machine-readable JSON
- generation of 2–3 visual concepts based on the brief
- recommendations for furniture/decor categories and key design techniques, without linking to specific stores

### 2.2 What Is Not Included in the MVP

- exact floor planning with real dimensions
- engineering calculations or renovation cost estimates
- recognition of drawings/floor plans
- automatic ergonomic validation
- selection of specific products with live pricing and availability

### 2.3 Real Product Links

Product подбор with real links is considered a later-stage feature and could be implemented through:

- affiliate programs
- API integrations with marketplaces or stores
- curated collections by style, budget, and category

## 3. Segmentation Approach

For the MVP, it makes more sense to segment users by **usage context** rather than demographics. This better connects audience segments to product requirements, since each group differs in goals, barriers, and success criteria.

For the MVP, it is recommended to focus on **two main segments** and optionally validate **1–2 secondary ones**.

## 4. Target Audience Segments

### Segment A: DIY Users Updating Their Interior

These users want to improve their home on their own, fully or partially, but lack a clear visual language. They do not know how to move from a general feeling to specific choices in palette, materials, lighting, furniture, and decor.

**Typical triggers:**

- moving into a new or first apartment
- dissatisfaction with the current interior
- renovating one room rather than the whole home
- new constraints: child, pet, remote work, new hobby
- seasonal desire for a refresh

**Pain points:**

- “I don’t know the right design terms.”
- “There are too many options, I get stuck.”
- “I don’t want to waste money on furniture that won’t fit the style.”
- “I save ideas on Pinterest, but still can’t make it work.”
- “I want it to look good but also be practical.”

**What they value:**

- turning vague feelings into concrete choices
- reducing uncertainty with 2–3 good directions instead of endless references
- clear next steps

**Success criteria:**

- “This matches what I had in mind.”
- “I understand what to buy or change.”
- “This feels realistic for my home.”

**Barriers and fears:**

- “AI makes beautiful images, but my result won’t look like that.”
- fear of overly expensive concepts
- fear of generic advice
- insecurity about describing preferences “incorrectly”

**To satisfy this segment, the MVP should:**

- accept plain everyday language
- ask 3–5 optional follow-up questions or offer quick checkboxes
- generate a human-readable brief with palette, materials, lighting, furniture, and accents
- provide 2–3 visual options and explain the differences
- offer a simple action plan or shopping checklist by category

**Example Jobs To Be Done:**

- When I want to refresh a room, I want 2–3 clear concepts quickly so I can choose a direction without drowning in references.
- When I buy furniture or decor, I want to know what works together so I avoid mistakes.

---

### Segment B: Users Preparing a Brief for a Designer or Renovation Team

These users either already plan to hire a designer/contractor or are choosing one. They understand that without a clear brief, communication becomes slow, expensive, and frustrating. This segment values time and needs a result that can actually be shared with a professional.

**Typical triggers:**

- first consultation with a designer or contractor
- bad past experience: “they misunderstood me”
- growing project budget or scale
- need for alignment with partner, family, or office stakeholders
- tight move-in or completion deadlines

**Pain points:**

- “I can’t explain what I want clearly.”
- “We spend too much time on revisions.”
- “I need something concrete that can be approved and fixed.”
- “I want the interior to be beautiful and functional.”
- “I’m afraid the result will be too expensive, impractical, or unrealistic.”

**What they value:**

- turning taste and ideas into structured requirements
- documenting priorities and constraints
- reducing iterations and interpretation conflicts
- creating one document that can be shared with a designer or contractor

**Success criteria:**

- the brief looks professional and shareable
- it includes concrete details: palette, materials, lighting, furniture/zones, functional needs
- constraints and “red lines” are clearly stated
- the visuals match the written brief
- the result helps move the project forward faster

**Barriers and fears:**

- expecting architect-level technical documentation, which is outside MVP scope
- fear of unrealistic “Instagram-style” images
- concern that the brief will still be too generic
- safety/legal issues: the service should not provide instructions for electrical or structural work

**To satisfy this segment, the MVP should:**

- produce a result that can actually be sent to a contractor or designer
- collect not only style preferences but also functionality and constraints
- structure the request in a professional format
- keep text and visuals consistent
- provide 2–3 alternative concepts with clear comparison
- support iterative refinement of the brief

**Example Job To Be Done:**

- When I go to a designer, I want a structured brief and references so I am understood and we reduce unnecessary iterations.