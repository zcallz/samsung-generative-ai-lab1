# Lab 3: Comparing Responses With and Without Document Context (RAG Concept)

## Step 1: Ask Questions Without Documents (Baseline)
* **Question Asked:** "What are the specific renewable energy subsidy allocation rules for G7 countries under the new 2026 Global Climate Finance Framework?"
* **AI Response (Baseline):** The AI provided a generic overview, mentioning common practices like tax credits, feed-in tariffs, and general green energy funds.
* **Observation:** The response lacked any specific 2026 data, exact budget caps, or specific policy clauses. It relied on its pre-trained general knowledge, which is insufficient for rigorous macroeconomic planning.

## Step 2: Ask the Same Questions With Documents Provided
* **Document Provided:** A mock 20-page internal policy document titled "2026 G7 Climate Finance & Econometric Assessment Guidelines".
* **AI Response (Grounded):** The AI stated explicitly that under Article 4 of the provided document, G7 countries must allocate 40% of their climate budget to offshore wind and green hydrogen, capped at $450 Billion, with compliance modeled via CS-ARDL methodologies.
* **Observation:** The answer was highly specific, citing exact figures, policies, and econometric requirements directly from the text.

## Step 3: Compare the Two Results
Comparing the baseline vs. document-grounded responses based on strict evaluation criteria:

1. **Accuracy:** The RAG (Step 2) response is factually correct based on the provided enterprise context, whereas the Step 1 response was merely a plausible guess.
2. **Specificity:** Step 2 provided concrete details (40% allocation, $450 Billion cap, Article 4). Step 1 provided none.
3. **Grounding:** The Step 2 answer was clearly grounded, explicitly referencing the provided framework document.
4. **Hallucination Risk:** Step 1 carried a massive hallucination risk, as the AI attempted to invent a summary for a highly specific 2026 policy it hadn't been trained on. Step 2 eliminated this risk.
5. **Trustworthiness:** In a real business or policy context, only the Step 2 (RAG) response can be trusted for making financial or econometric modeling decisions.
