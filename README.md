# WHO Infodemic data

The WHO Social Listening Infodemic Platform shows real-time information about how people are talking about COVID-19 online, so we can better manage as the infodemic and pandemic evolve.

More information about the initiative and an exploration of the data can be found at [WHOinfodemic.citibeats.com](http://whoinfodemic.citibeats.com/).

More information about the methodology, data and definitions can be found at [WHOinfodemic.citibeats.com/methodology](http://whoinfodemic.citibeats.com/methodology).

The platform is powered by Citibeats, a text analytics platform specialized in social understanding. More information can be on the methodology page, or found at [www.citibeats.com](http://www.citibeats.com/).

## Intended use

Listening to people&#39;s questions and concerns is an important way for health authorities to learn about what matters to communities in response to COVID-19. This social listening platform aims to show real-time information about how people are talking about COVID-19 online, so we can better manage as the COVID-19 infodemic and pandemic evolve.

While the Social Listening Infodemic Platform website facilitates ready made visualizations for easy exploration of the data, the aggregated and anonymized data is made available for anyone wishing to integrate the data into their own research, or integrate the data into their existing workflows.

This is available via the public API as well as this GitHub repository.

Any use of the data should use the citation &#39;World Health Organization, Social Listening Infodemic Platform&#39;.

We welcome you sharing with us [how you are using the data](http://whoinfodemic.citibeats.com/share-use-case), as well as feedback on how to [improve the platform for your needs](https://whoinfodemic.citibeats.com/feedback).

## Origin of the data

The data has been obtained from public posts related to COVID-19, using the Twitter API and data aggregators of public sources such as forums, message boards, blogs and comments in news. Please keep in mind that this is only a sample of all COVID-19 conversations.

The data is updated each day with new posts.

_NOTE: all data is subject to quality, technical, and ethical requirements before being added to the system._

More information about the data can be read [here](http://whoinfodemic.citibeats.com/methodology).

## How to interpret the data

Since the civic situation is constantly evolving and social needs are wide-ranging, there is a need for real-time data to serve the decisions of key actors. At the same time, this data must be treated carefully, as the data query and categories are subject to change along with the conversation. This repository will be kept up-to-date with revised data, and changes noted here. Note that, as new sources are added to the system, records from earlier dates could change.

Every analysis based on Internet data has to deal with representativity. Not everyone is connected to the Internet, and not everyone shares their opinion.

Further information on the methodology, data and definitions can be read [here](http://whoinfodemic.citibeats.com/methodology.).

CSV columns:

- `id`: code of the country as defined by [ISO 3166-1 alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3#Officially_assigned_code_elements)
- `date`: day in which the raw data was published in YYYY-MM-DD format (UTC timezone)
- `name`: name of the country in English
- `docs-N`: number of documents for the category N on a given day
- `docs-delta-percent-N`: variation of documents (%) for the category N respect the previous day
- `docs-percent-N`: percent of documents in the category N respect all the other categories in that day
- `docs-female-N`: number of documents for the category N on a given day, which are estimated to be from females
- `docs-male-N`: number of documents for the category N on a given day, which are estimated to be from males
- `docs-questions-N`: number of documents for the category N on a given day, which were questions
- `docs-complaints-N`: number of documents for the category N on a given day, which were complaints

NOTE: each row in the CSV corresponds to one day of data for a specific country.

## Category definitions

<table>
	<thead>
		<tr>
			<th>Level 1</th>
			<th>Level 2</th>
			<th>Definition</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td rowspan="3">
        <p><b>The cause</b></p>
        <p><em>How did the virus emerge and how is it spreading?</em></p>
      </td>
			<td><b>The cause of the virus</b></td>
			<td>Where do people think it comes from: lab derived, wild animal markets, animals, place where the virus comes from, imported food, etc.</td>
		</tr>
		<tr>
			<td><b>Stigma about the spread</b></td>
			<td>Stigma on people who are thought of spreading the virus: racist expressions, attribution to poor people or immigrants,</td>
		</tr>
		<tr>
			<td><b>Stigma about or by infected people</b></td>
			<td>Stigma expressed about or by infected people or have been infected</td>
		</tr>
		<tr>
			<td rowspan="9">
        <p><b>The illness</b></p>
        <p>What are the symptoms and how is it transmitted?</p>
      </td>
			<td><b>Confirmed symptoms</b></td>
			<td>Confirmed symptoms as defined by WHO, including long-term symptoms</td>
		</tr>
		<tr>
			<td><b>Other discussed symptoms</b></td>
			<td>Other discussed symptoms that have not yet been confirmed by WHO</td>
		</tr>
		<tr>
			<td><b>Asymptomatic transmission</b></td>
			<td>Comments on transmission from asymptomatic people, about asymptomatic people, or personal experience of asymptomatic people</td>
		</tr>
		<tr>
			<td><b>Pre-symptomatic transmission</b></td>
			<td>Comments on transmission from pre-symptomatic people, about pre-symptomatic people, or personal experience of pre-symptomatic people</td>
		</tr>
		<tr>
			<td><b>Modes of transmission</b></td>
			<td>Modes of transmission confirmed and unconfirmed by WHO</td>
		</tr>
		<tr>
			<td><b>Protection from transmission</b></td>
			<td>Actions that individuals take to protect themselves – discussion of recommended or also other types of actions that individuals should take to protect themselves</td>
		</tr>
		<tr>
			<td><b>Transmission settings</b></td>
			<td>Narratives about settings where transmission can be amplified: closed and semi-closed settings</td>
		</tr>
		<tr>
			<td><b>Demographic vulnerability & risks</b></td>
			<td>
        Vulnerable and risk groups:
        <ul>
          <li>elderly</li>
          <li>individuals with health conditions like lung or heart disease, diabetes or conditions that affect their immune system</li>
          <li>pregnant women</li>
      </td>
		</tr>
		<tr>
			<td><b>Impact on mental health</b></td>
			<td>Anxiety, depression and other affections derived from the pandemic situation</td>
		</tr>
		<tr>
			<td rowspan="6">
        <p><b>The treatment</b></p>
        <p>How can it be treated or cured?</p>
      </td>
			<td><b>Current treatment</b></td>
			<td>Medical treatment as per WHO treatment recommendations</td>
		</tr>
		<tr>
			<td><b>COVID-19 vaccine</b></td>
			<td>Narratives about the vaccine itself (side effects, safety, etc)</td>
		</tr>
		<tr>
			<td><b>Health care workers (HCW) and vaccine</b></td>
			<td>Narratives by and about health care workers and vaccine</td>
		</tr>
		<tr>
			<td><b>General vaccine discussion</b></td>
			<td>Narratives about vaccines in general, including discussion about others or communities that have different opinions about vaccines; can include any vaccine concerns, not just COVID-19</td>
		</tr>
		<tr>
			<td><b>Science and R&D</b></td>
			<td>Comments on new treatment and vaccines from research and development and evidence and scientific processes</td>
		</tr>
		<tr>
			<td><b>Non proven treatments</b></td>
			<td>Discussion about treatments that are not proven to be effective (examples: sunlight, nutrition, herbal remedies, etc)</td>
		</tr>
		<tr>
			<td><b>Myths</b></td>
			<td>Specific myths that WHO and partners have reacted to taken steps to debunk reference</td>
		</tr>
		<tr>
			<td rowspan="18">
        <p><b>The interventions</b></p>
        <p>What is being done by government and health authorities and societal institutions?</p>
      </td>
			<td><b>Testing</b></td>
			<td>Any discussion about tests – everything from reliability, to access to tests, types of tests, requirement to have tests, etc.</td>
		</tr>
		<tr>
			<td><b>Contact tracing</b></td>
			<td>Any discussion about the process, requirements and steps involved in contact tracing, use of technology</td>
		</tr>
		<tr>
			<td><b>Supportive care</b></td>
			<td>Care given to patients in hospitals by medical personnel</td>
		</tr>
		<tr>
			<td><b>Vaccine distribution and policies on access</b></td>
			<td>Narratives about distribution, equity, access to COVID-19 vaccine</td>
		</tr>
		<tr>
			<td><b>Personal measures</b></td>
			<td>Individual protection measures recommended by governments/OMS such as wearing masks, handwashing, social distance, isolation when ill...</td>
		</tr>
		<tr>
			<td><b>Measures in public settings</b></td>
			<td>Measures implemented by governments in public settings: schools, workplaces, public transport...</td>
		</tr>
		<tr>
			<td><b>Travel measures</b></td>
			<td>Measures implemented or suggested by governments/OMS/population/private companies on travel: immunity passports, negative PCR or negative rapid test to enter a country, mandatory quarantine</td>
		</tr>
		<tr>
			<td><b>Reduction of movement</b></td>
			<td>Measures implemented by governments related to movement reduction: lock-down at home, territory lock-down, etc.</td>
		</tr>
		<tr>
			<td><b>Protection: medical equipment</b></td>
			<td>Equipment for health workers</td>
		</tr>
		<tr>
			<td><b>Health Technology</b></td>
			<td>Health technology used to treat patients: <span style="color: #333333; background: white;">medicines, medical devices, vaccines, procedures and systems </span>
			</td>
		</tr>
		<tr>
			<td><b>Digital health technology</b></td>
			<td>Discussions about digital technology used to respond to pandemic: electronic data exchange, electronic notices of passenger lists to health authorities, biometric data coming from wearables, proximity apps (App Covid). Includes people’s attitudes to data privacy, or for modelling and predictive analytics.</td>
		</tr>
		<tr>
			<td><b>Pandemic Fatigue</b></td>
			<td>Fatigue from interventions (lock-down, movement restrictions, masks…)</td>
		</tr>
		<tr>
			<td><b>Faith</b></td>
			<td>Narratives about faith and religion and COVID-19 (these narratives are recurring, usually around the time of religious holidays and outbreaks in faith based settings)</td>
		</tr>
		<tr>
			<td><b>Industry</b></td>
			<td>Narratives about industry, unions and COVID-19</td>
		</tr>
		<tr>
			<td><b>Environment</b></td>
			<td>Narratives about the environment and COVID-19 – some examples: shading in environment, waste water, air pollution as a secondary byproduct of lockdowns</td>
		</tr>
		<tr>
			<td><b>Inequalities</b></td>
			<td>Narratives about social inequalities and relation to COVID-19</td>
		</tr>
		<tr>
			<td><b>Civil Unrest</b></td>
			<td>Narratives about civil unrest and COVID-19</td>
		</tr>
		<tr>
			<td><b>Youth</b></td>
			<td>Narratives about youth, effects of pandemic on them, or actions youth is taking</td>
		</tr>
		<tr>
			<td rowspan="5">
        <p><b>Type of information</b></p>
        <p>What types of information are most engaging?</p>
      </td>
			<td><b>Statistics & data</b></td>
			<td>Conversations about facts, official statistics and data</td>
		</tr>
		<tr>
			<td><b>Misinformation</b></td>
			<td>Conversations about misinformation</td>
		</tr>
		<tr>
			<td><b>Mis- and Disinformation</b></td>
			<td>Conversations about mis- and disinformation</td>
		</tr>
		<tr>
			<td><b>Sources & influencers</b></td>
			<td>Conversations about where people look for information</td>
		</tr>
	</tbody>
</table>

## Contact

infodemicmanagement@who.int
