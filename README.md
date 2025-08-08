# To what extent does Land Use Change from Deforestation contribute to CO₂ emissions across SEA countries? 🌳
Hi there! I am Nidaan, this is my portfolio to apply for ESG Data Analyst (and related roles)! 🙌🏻 I used data from [The World Bank](https://databank.worldbank.org/) and am currently practising my data analysis skills. I'd love to hear any feedback. Thank you and hope you find this insightful!<br /><br />
To answer this, we divide into several questions! <br /> <br />

## 1️⃣ How does forest loss, weighted by forest area, influence CO₂ emissions from land-use change across Southeast Asian countries?
First, I cleaned data I extracted from the World Bank using MySQL. After finishing the preprocessing step, I loaded data into Jupyter Notebook. Using Random Forest algorithm, we discovered that the feature importance score for the following factors are as follows: <br />

**Tree Cover Loss (hectares) : 91.1%** <br />
**Forest Area (%) : 8.9%** <br />

Notice that tree cover loss has a strong influence on carbon emissions from Land Use Change and Forestry (LUCF) across SEA countries. This could indicate that changes in tree cover, such as deforestation, is the primary cause of carbon emissions in LUCF. However, we need to keep in mind that Tree cover loss is an absolute value whilst forest area is the relative value. One interesting insight we can draw from this is: <br /> 

💡In densely forested countries, small changes in forest area can mean hundreds or thousands of hectares forest lost, resulting in massive carbon emission. For instance, 1% change in Indonesian forest area results in +500 Mt CO₂/year emissions whilst 1% reduction in Singapore's forest area only results in +0.4 Mt CO₂/year. Therefore, we need to be careful when we want to use forest area data to capture better understanding of the overall context. <br />

## 2️⃣ Which country have the highest CO₂ emissions from deforestation?
Moving on, now we discuss which countries experience rising CO₂ emissions due to deforestation. Using the same dataset, we now obtain the following graph. 

![Random Forest Results](https://github.com/user-attachments/assets/0d5b68ce-f13b-4c73-8765-ec1b851daa06)

I did this simple graph in Ms Excel and some modifications in Figma to get a more visually captivating graph. This figure shows SEA countries ranked by the highest R² using Random Forest depicting the contribution to their annual CO₂ emissions. However, for Singapore, the initial CO₂ emissions were negative. Negative values in the dataset (provided by The World Bank) refer to carbon removals.
<br /> 
## 3️⃣ How does LUCF-based CO₂ emission compare to other sectors (industry, energy, transport, mining) in each country?
This question aims to investigate whether carbon emission from land use changes (especially from deforestation) dominate a country's total emissions. During the data cleaning process using MySQL, we excluded several countries that consistently have a 0 value for at least one sector. After discovering which countries meet the criteria, we can only include: Indonesia, Malaysia, Thailand, Philippines, Cambodia, Myanmar, and Vietnam.
 <br />
 
 <img width="5658" height="2892" alt="asean_emissions_by_sector" src="https://github.com/user-attachments/assets/3671fb79-555f-4a80-809e-bf47af1a9d9a" />
<br />
Based on this figure, we can draw insights that Indonesia is the largest CO₂ emitter in SEA with LUCF domination. If we correlate with the previous analysis, we can infer that deforestation is the highest CO₂ emission source in Indonesia, even compared to other countries. However, Cambodia and Myanmar also experience dominant CO₂ emission from LUCF. 

## 📝Conclusions
1. Tree Cover Loss is the prominent cause of CO₂ emissions from Land-Use Changes and Forestry in Southeast Asian Countries. Small feature importance of forest area reflects that relative value can't represent the CO₂ emissions.
2. Indonesia has the highest CO₂ emissions from deforestation followed by Brunei, Malaysia, and Thailand. As for Singapore, the initial CO₂ emission in 2008 - 2015 is negative, meaning carbon removals.
3. LUCF is the dominant source of CO₂ emissions in Indonesia, Cambodia, and Myanmar. Whilst in Malaysia, Thailand, Philippines, and Vietnam, the most dominant CO₂ emissions sourced from energy usage.
