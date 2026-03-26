# MVP User Testing

## 1. Sample Description

A focus group of **10 users** was recruited for testing.

The sample included:

- **3 students** (ages 20–23) interested in design and visual AI tools
- **2 beginner interior designers**
- **1 IT specialist** actively using AI services
- **4 non-professional users** interested in home renovation and furnishing

### Why the project was relevant to them

- fast visualization of interior ideas
- interest in generative AI
- inspiration for renovation or home design
- professional curiosity from designers

## 2. Testing Format

Testing was conducted as **individual interviews with hands-on product use**.

Each participant:

1. received access to the **first version of the website**
2. was given a short instruction:  
   *“Try generating an interior you would like to see.”*
3. interacted with the interface independently
4. was observed by the moderator, who recorded:
   - difficulties
   - behavior
   - comments
5. answered follow-up questions after use

### First Version Limitation

The first MVP included **only one UI element**: a text input field for the prompt.

This helped test:

- whether text-only control was enough
- what expectations users had from the service

## 3. Example Interview Questions

Users were asked questions such as:

- Was it clear how to use the service?
- Were you satisfied with the generated result?
- Is text input alone enough to control the result?
- Would you like more control? If yes, how?
- Which parameters would you want to set explicitly?
- What did you dislike or find difficult?
- What would you add to the service?
- Would you use this in real life?

## 4. Survey Results

### Users satisfied with the MVP — ~30%

**3 users**

Typical feedback:

- “Overall, it’s clear and convenient.”
- “Text description is enough for me.”
- “The result is good; I would use it.”

However, even they noted that it can be hard to describe exactly what they want.

### Users who wanted more control — ~60%

**6 users**

Their feedback directly pointed to the main product improvements.

#### Style selection

- “I want to choose a style instead of typing it every time.”
- “Sometimes I write ‘Scandinavian,’ but the result doesn’t really match.”
- “There should be ready-made options like loft or minimalism.”

#### Room size

- “It’s unclear what kind of room the model is generating unless I specify it in the prompt.”
- “I want to indicate whether it’s a small bedroom or a large living room.”

#### Lighting

- “Lighting has a huge impact, but it’s hard to describe in words.”
- “I want to choose something like evening light or daylight.”

#### Main issue

- “Too much depends on how the text is written.”
- “I want more control through the interface, not only through text.”

### Users interested in photo upload — ~10%

**1 user** (with partial support from another)

Typical feedback:

- “It would be great to upload a photo of my own room and get a redesign.”
- “I don’t want an abstract interior; I want to redesign my actual space.”

This feature was not included in the current MVP, but it was recorded as a promising next step.

## 5. Quantitative Summary

- **30% (3 users)** — fully satisfied with the MVP
- **60% (6 users)** — wanted more control over style, size, and lighting
- **10% (1 user)** — wanted photo upload functionality

## 6. Key Findings

The testing revealed several important insights:

1. **Text-only control is not enough**  
   Many users struggle to write precise prompts.

2. **Users want structured control**  
   The most requested parameters were:
   - style
   - room size
   - lighting

3. **The interface should reduce the need for prompt-engineering skills**  
   Users expect guidance, not just a text box.

4. **There is demand for personalization through photos**  
   This is outside the MVP scope but relevant for future development.

## 7. Outcome

The testing confirmed that:

- the product idea is relevant
- the core scenario works
- the main improvement area is **adding controllable parameters to the interface**

Based on this feedback, the following features were added:

- style selection
- room size selection
- lighting selection
- extended backend request structure

These changes made the system:

- easier to understand
- more controllable
- closer to user expectations