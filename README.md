# Personalized Real Estate Agent

## I. Project scope
Imagine you're a skilled developer at "Future Homes Realty," an innovative real estate company. In an industry where personalization is crucial for customer satisfaction, your company aims to transform how clients engage with property listings. The objective is to create a customized experience for each buyer, making the property search more interactive and aligned with their unique preferences.

## II. Core Components of "HomeMatch"
### 1. Understanding Buyer Preferences:
- Buyers will enter their preferences, including location, property type, budget, amenities, and lifestyle choices.
- The app leverages LLMs to process these inputs in natural language, grasping detailed requests beyond simple filters.

### 2. Integrating with a Vector Database:
- Integrate "HomeMatch" with a vector database housing all property listings.
- Use vector embeddings to match properties to buyer preferences, including neighborhood vibes, architectural styles, and proximity to amenities.

### 3. Personalized Listing Description Generation:
- For each matching listing, use an LLM to rewrite the description to emphasize features most relevant to the buyer's preferences.
- Make sure the personalization highlights aspects that appeal to the buyer while keeping all factual property details unchanged.

### 4. Listing Presentation:
- Output the personalized listing(s) as a text description of the listing.

## III. Install and execute
1. Clone the repo
```
https://github.com/hoangduchuy93/Personalized-Real-Estate-Agent.git
```

2. Create the environemt
```
cd Personalized-Real-Estate-Agent
python3 -m venv .venv
source .venv/bin/activate
```

3. Install the libraries
```
pip install -r requirements.txt
```

Note: it is important to notice that the ChromaDB only works with version **0.3.29**. Unless this version, you can not persist the embeddings
