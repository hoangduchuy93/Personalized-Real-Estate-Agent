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

Note: it is important to notice that the ChromaDB only works with version **0.3.29**. Unless this version, you can not persist the embeddings. Please install ChromaDB with **%pip install chromadb==0.3.29**

4. Run the notebook
```
jupyter notebook
```

## IV. Chatbot Real Estate Consultant
Below are some examples from chatbot to consult the customers

Example 1:
```
- Question A comfortable three-bedroom house with a spacious kitchen and a cozy living room.
- Answer: Based on your preferences for a comfortable three-bedroom house with a spacious kitchen and a cozy living room, I have found the perfect property for you. This stunning home features a gourmet kitchen with stainless steel appliances, perfect for whipping up delicious meals for your family and friends. The open-concept living area is ideal for relaxing or entertaining, with a cozy fireplace to create a warm and inviting atmosphere.

The spacious master suite offers a private retreat with a luxurious en-suite bathroom and walk-in closet, providing you with the perfect sanctuary to unwind after a long day. Additionally, the master suite also boasts a jetted tub, perfect for relaxing and rejuvenating.

Furthermore, the updated kitchen includes modern appliances and a breakfast nook, making it the perfect space to start your day with a cup of coffee. The master suite also offers a private balcony, where you can enjoy your morning coffee or relax in the evening with a glass of wine while taking in the beautiful views.

Overall, this property not only meets your criteria for a comfortable three-bedroom house with a spacious kitchen and cozy living room, but it also exceeds your expectations with its luxurious features and amenities. I believe this property is the perfect fit for you and I highly recommend you schedule a viewing to experience it for yourself.
Sources: ['2', '4', '5']
```

Example 2:
```
- Question: A quiet neighborhood, good local schools, and convenient shopping options.
- Answer: This charming family home in the desirable Suburban Meadows neighborhood is the perfect fit for you! The quiet neighborhood offers a peaceful retreat from the hustle and bustle of city life, while the top-rated local schools provide excellent education options for your family. With convenient shopping options just a short drive away, running errands will be a breeze.

This 4-bedroom, 3-bathroom home is ideal for entertaining guests or simply relaxing with your loved ones. The spacious backyard with a deck is perfect for outdoor gatherings, while the open-concept living area features a cozy fireplace for those chilly evenings. The gourmet kitchen with stainless steel appliances is a chef's dream, making meal preparation a joy.

The master suite is a true sanctuary, offering a jetted tub for ultimate relaxation and a walk-in closet for all your storage needs. With a modern kitchen perfect for entertaining, and the convenience of living within walking distance to top restaurants, shops, and entertainment venues, this home truly has it all. Don't miss out on the opportunity to make this your dream home!
Sources: ['1', '2', '4']
```
