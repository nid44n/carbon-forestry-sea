# To what extent does Land Use Change from Deforestation contribute to CO₂ emissions across SEA countries? 🌳
Hi there! I am Nidaan, this is my portfolio to apply for ESG Data Analyst (and related roles)! 🙌🏻 I used data from [The World Bank](https://databank.worldbank.org/) and am currently practising my data analysis skills. I'd love to hear any feedback. Thank you and hope you find this insightful!<br /><br />
To answer this, we divide into several questions! <br /> <br />

## 1️⃣ How does forest loss, weighted by forest area, influence CO₂ emissions from land-use change across Southeast Asian countries?
First, I cleaned data I extracted from the World Bank using MySQL. After finishing the preprocessing step, I transformed data into Jupyter Notebook to later be processed by Python. Using Random Forest algorithm, I discovered that the feature importance score for the following factors are as follows: <br />

**Tree Cover Loss (hectares) : 91.1%** <br />
**Forest Area (%) : 8.9%** <br />

Notice that tree cover loss has a strong influence in carbon emissions from Land Use Change and Forestry (LUCF) across SEA countries. This could indicate that changes in tree cover, such as deforestration, is the primary cause of carbon emissions in LUCF. However, we need to keep in mind that Tree cover loss is an absolute value whilst forest area is the relative value. One interesting insight we can draw from this is: <br /> 

💡In densely forested countries, small changes in forest area can mean hundreds or thousands of hectares forest lost, resulting in massive carbon emission. For instance, 1% change in Indonesian forest area results in +500 Mt CO₂/year emissions whilst 1% reduction in Singapore's forest area only results in +0.4 Mt CO₂/year. Therefore, we need to be careful when we want to use forest area data to capture better understanding of the overall context. <br />

## 2️⃣ Which country have the highest CO₂ emissions from deforestation?
Moving on, now we discuss which countries experience rising CO₂ emissions due to deforestation. Using the same dataset, we now obtain the following graph. 

![Random Forest Results](https://github.com/user-attachments/assets/0d5b68ce-f13b-4c73-8765-ec1b851daa06)

I did this simple graph in Ms Excel and  some modifcations in Figma to get a more visually captivating graph. This figure shows SEA countries ranked by the highest R² using Random Forest depicting the contribution to their annual CO₂ emissions. However, for Singapore. The initial CO₂ emissions were in minus. Negative values in the dataset (provided by The World Bank) refers to carbon removals.
<br /> 
## 3️⃣ How does LUCF-based CO₂ emission compare to other sectors (industry, energy, transport, mining) in each country?
This question aims to investigae whether carbon emission from land use changes (especially from deforestation) dominate one country's total emissions. During the data cleaning process using MySQL, we exclude several countries where they consistently have 0 value for at least one sector. After discovering which countries meet the criteria, we can only include: Indonesia, Malaysia, Thailand, Philippines, Cambodia, Myanmar, and Vietnam. 
 <br /> pake stacked bar chart

## 📝Conclusions

## 🙋‍♀️Here's what I suggest
