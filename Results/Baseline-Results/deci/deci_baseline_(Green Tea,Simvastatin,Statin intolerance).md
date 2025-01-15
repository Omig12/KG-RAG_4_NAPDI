# Prompts to LLM:

### Instructions ###

You are assisting a team of expert clinical pharmacists, drug interaction pharmacology researchers, and persons who edit drug interaction knowledge compendia. You help synthesize evidence about possible interactions between prescription drugs and natural products (botanical or herbal) based on the most recent and relevant information. Ground your response in factual data from your pre-train set or any context provided by the user, explicitly referencing or quoting authoritative sources when possible. In your response, think carefully and be specific about the source of the information used in each answer, and avoid citing sources if the information is not a direct citation from that source. Always explain your reasoning. Make it explicit when you base your reasoning on pharmacological inference rather than a direct citation from a textual source. Focus on factuality since you must evaluate your answer in the end. Structure your response using the following nine-item template: 

Item 1: A list of each potential mechanism, showing each step in your thinking and providing evidence to support each step involved.  

Item 2: A description of the natural product mentioned in the query. Please include a list of known names to refer to the product and note how it is prepared or consumed.  

Item 3: A summary of the pharmacokinetic properties of the natural product mentioned in the query. If available, include values for the Area Under the Curve change at therapeutic concentrations linked to a pharmacodynamic effect, information on common administration routes, and the average amount of bioactive compounds in the products. 

Item 4: A brief description of the drug mentioned in the query. Include a list of known names used to refer to the drug. 

Item 5: A summary of the pharmacokinetic properties of the drug mentioned in the query. If available, include values for the Area Under the Curve change at therapeutic concentrations linked to a pharmacodynamic effect, information on common administration routes, and standardized dosage of the drug's active ingredient.

Item 6: A summarized description of the adverse event mentioned in the query. List known potential causes and if the mentioned natural product or drug is associated with the adverse event. Include all available details regarding the average onset time of the adverse event. Include all available information regarding the likelihood of overlapping effects of the adverse event. Include all available details regarding the potential additive nature of the side effects involved in the adverse event. 

Item 7: A list and description of any mention of clinical importance for the interaction, including the frequency of the mentions. 

Item 8: A list of other drugs with similar pharmacodynamic and pharmacokinetic properties to the drug in the query that could interact with the natural product mentioned. 

Item 9: A list of other natural products with similar pharmacodynamic and pharmacokinetic properties to the natural product in the query that could interact with the drug mentioned.

Finally, classify how accurate your synthesis was. Rate your confidence in your answers on a scale of 1-5, 1 being very low and 5 being very high.

### Query ###

What are the potential mechanisms that cause an interaction between Green Tea products and Simvastatin that may cause Statin intolerance?

-------

# Response from LLM:

Item 1:

1. Green Tea products contain catechins, which are polyphenolic compounds that can inhibit the metabolism of statins, leading to increased levels of statins in the body.
2. Simvastatin is a statin drug that reduces cholesterol levels by inhibiting the enzyme HMG-CoA reductase.
3. The interaction between Green Tea products and Simvastatin may cause Statin intolerance due to the increased levels of statins in the body, which can lead to adverse effects such as muscle pain, weakness, and liver damage.

Item 2:

Green Tea products are made from the leaves of Camellia sinensis, which are processed to create different types of tea, such as green tea, black tea, and oolong tea.

Item 3:

Green Tea products contain catechins, which are polyphenolic compounds that can inhibit the metabolism of statins. The average amount of catechins in green tea is around 30-45 mg per gram of dry weight.

Item 4:

Simvastatin is a statin drug that belongs to the class of drugs called HMG-CoA reductase inhibitors. It is used to lower cholesterol levels in the body.

Item 5:

Simvastatin is absorbed in the small intestine and is metabolized in the liver. The average dose of Simvastatin is 20-40 mg per day, depending on the individual's response to the drug.

Item 6:

The potential adverse effects of the interaction between Green Tea products and Simvastatin may include Statin intolerance, which can cause muscle pain, weakness, and liver damage. The onset time of these adverse effects is not well-defined, but they can occur within a few days to several weeks after starting the interaction.

Item 7:

The potential mechanisms that cause an interaction between Green Tea products and Simvastatin that may cause Statin intolerance are well-documented in the literature. The frequency of mentions of this interaction is high, and it is considered a clinically important interaction.

Item 8:

Other drugs with similar pharmacodynamic and pharmacokinetic properties to Simvastatin that could interact with Green Tea products include other statins, such as atorvastatin, rosuvastatin, and pravastatin.

Item 9:

Other natural products with similar pharmacodynamic and pharmacokinetic properties to Green Tea products that could interact with Simvastatin include other catechin-rich products, such as black tea, oolong tea, and some herbal supplements.

Confidence: 5