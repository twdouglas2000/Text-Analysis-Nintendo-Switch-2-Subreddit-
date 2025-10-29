_Nintendo Switch 2 Subreddit Text Analysis_

**Project Overview**

This project is a Natural Language Processing (NLP) pipeline designed to extract, analyze, and quantify public sentiment toward the anticipated Nintendo Switch 2 console based on posts from a

The following is a GitHub README section generated for your Nintendo Switch 2 Subreddit Text Analysis project, incorporating the data analysis steps and key findings from your provided notebook and resume summary.

**Nintendo Switch 2 Subreddit Text Analysis**

Sentiment and topic modeling analysis on fan discussions to extract actionable business insights.

**Project Overview**

This project implements a complete Natural Language Processing (NLP) pipeline to analyze and interpret public sentiment toward the Nintendo Switch 2 on a dedicated Reddit community. The goal was to identify the key drivers of fan discussion—both positive and negative—to provide data-driven recommendations for marketing, sales, and customer service strategies.

**Key Technologies**

The analysis was performed entirely in Python, utilizing the following libraries:

Data Collection: PRAW (Python Reddit API Wrapper), requests, BeautifulSoup

Preprocessing/NLP: NLTK (Natural Language Toolkit)

Sentiment Analysis: VADER (Valence Aware Dictionary and sEntiment Reasoner)

Topic Modeling: NMF (Non-Negative Matrix Factorization)

**Methodology**
1. Data Extraction

Extracted and analyzed 100 recent subreddit posts using the Reddit API (via PRAW) to build the core dataset.

2. Text Preprocessing

Preprocessed text by implementing a rigorous cleaning pipeline.

Steps included removing special characters and stop words, tokenization, POS tagging, and lemmatization (using WordNetLemmatizer) to standardize vocabulary.

3. Sentiment Analysis (VADER)

Applied the VADER sentiment tool, chosen for its effectiveness with social media and slang, to classify posts as Positive (compound score ≥0.05), Neutral (−0.05<compound score<0.05), or Negative (compound score ≤−0.05).

4. Topic Modeling (NMF)

Performed NMF topic modeling (Non-Negative Matrix Factorization) separately on the positive and negative post subsets. NMF was selected for its fast, interpretable output, which is ideal for shorter social media text.

**Key Findings & Results**:Overall Sentiment Distribution**


Positive (54%)

Neutral (26%)

Negative (20%)

The analysis revealed that the majority of recent posts on the subreddit expressed positive sentiment.

Positive Sentiment Drivers (Top 3 NMF Topics)

The primary topics driving positive discussion focused on peripherals, online play, and corporate announcements:

Grippy Case and Pro Controllers (10 posts).

Online Multiplayer (9 posts).

Nintendo Direct System Releases (9 posts).

**Negative Sentiment Drivers (Key NMF Topics)**

Negative sentiment, while a minority, concentrated on pain points related to the product and purchasing experience:

Purchasing Switch 2 and Games (10 posts): Concerns often revolve around limited stock, game availability (digital vs. physical), or difficulty of purchase.

Screen Protector (5 posts): Implies a perception of device fragility or a perceived mandatory expense beyond the console's price.

Screen and Video Settings (5 posts): Indicates mixed feelings about the hardware's display capabilities (e.g., HDR/TV output issues).

**Business Recommendations**

The findings were translated into actionable business recommendations:

Department	Recommendation	Justification
Marketing	Highlight comfort-focused peripheral design (grips/controllers) and the social/multiplayer experience in campaigns.	These topics are strong positive sentiment drivers.
Sales/Product	Address stock and purchasing difficulties directly, and consider providing an enhanced screen protector or more durable screen in future revisions.	Concentrated negative topics point to friction in the purchasing/user experience that can lead to customer dissatisfaction.
Customer Service	Prioritize support documentation and troubleshooting guides for screen/video output settings to mitigate confusion and user frustration.	The presence of screen settings in a negative topic suggests troubleshooting issues exist.
