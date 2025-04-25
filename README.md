# MP Religion & Assisted Dying Dashboard

This dashboard presents insights into the religious affiliations and Assisted Dying voting patterns of UK Members of Parliament (MPs).

## 📊 What is this dashboard?

This dashboard presents insights into the religious affiliations and Assisted Dying voting patterns of UK Members of Parliament. It combines publicly available data to support transparency and understanding of Parliament's composition.

## 📂 Where does the data come from?

The data is compiled from publicly available parliamentary records and voting data. You can download it directly from the link in the header or view it in the **Raw Data** tab of the dashboard.

## 🙏 How is religion determined?

There are three steps to determining religion. An MP is classified as having a religion based on the following criteria:

1. If the MP is a member of a religiously based group, they are classified as a member of that religion.
2. If a member has publicly spoken about their religion, they are classified as a member of that religion.
3. Finally, the text an MP swore in on is used to help infer their religion.

These sources are used in order of priority. For example, Tim Farron is a member of Christians in Parliament and has spoken about his religious views. However, he did not take the oath on the Bible, but made a solemn affirmation on no text. Regardless, he is still classed as Christian.

## 🧾 Variable Reference

**What do those variable names mean?**

- **Member ID** – *member_id* – A unique numeric identifier for each MP provided by Parliament.
- **Name** – *display_as* – The full display name of the MP.
- **Gender** – *gender* – The MP's gender.
- **Party** – *party* – The full political party name.
- **Party (Simplified)** – *party_simple* – A shortened or cleaned version of the party name.
- **Religion** – *mp_final_relig* – The MP’s classified religion based on multiple criteria outlined above.
- **AD: 2nd Reading Vote** – *ass_suicide_2nd* – The MP's vote (Yes, No, Abstain) on the Assisted Dying Bill 2nd Reading.
- **AD: 3rd Reading Vote** – *ass_suicide_3rd* – The MP's vote (Yes, No, Abstain) on the Assisted Dying Bill 3rd Reading.
- **LGBT Status** – *lgbt* – Whether the MP is publicly identified as LGBT ([LGBT.MP](https://www.lgbt.mp/)).
- **Ethnic Minority** – *ethnic_mp* – Whether the MP identifies as an ethnic minority.
- **Religious Group: Christian** – *relig_christian* – MP belongs to a Christian group (1 = Yes).
- **Religious Group: Muslim** – *relig_muslim* – MP belongs to a Muslim group (1 = Yes).
- **Religious Group: Jewish** – *relig_jewish* – MP belongs to a Jewish group (1 = Yes).
- **Religious Group: Sikh** – *relig_sikh* – MP belongs to a Sikh group (1 = Yes).
- **Oath Taken** – *mp_swear* – Whether the MP took the Oath or made an Affirmation.
- **Oath Book** – *mp_swear_book* – The specific religious text (e.g., Bible, Quran) used when swearing in.
- **Inferred Religion** – *mp_inferred_relig* – The religion inferred from the swearing-in text.
- **Election Outcome** – *elected* – Whether the MP was re-elected in the most recent election.
- **Majority** – *majority* – The MP’s vote share margin.
- **Constituency Type** – *constituency_type* – Type: Borough or County.
- **Claimant Rate** – *cen_claimant* – % of constituents claiming unemployment benefits.
- **% White (Census)** – *cen_eth_white* – Proportion of white ethnicity in the constituency.
- **% Christian** – *cen_rel_christian* – Constituency Christian population from the Census.
- **% Buddhist** – *cen_rel_buddhist* – Constituency Buddhist population.
- **% Hindu** – *cen_rel_hindu* – Constituency Hindu population.
- **% Jewish** – *cen_rel_jewish* – Constituency Jewish population.
- **% Muslim** – *cen_rel_muslim* – Constituency Muslim population.
- **% Sikh** – *cen_rel_sikh* – Constituency Sikh population.
- **% No Religion** – *cen_rel_no religion* – Constituents identifying as non-religious.
- **% No Qualifications** – *cen_qual_none* – Constituents with no formal qualifications.
- **% Graduates** – *cen_qual_grad* – Constituents with degree-level education.
- **% Some Disability** – *cen_disab_some* – Constituents reporting a form of disability.

## ✝️ Why are Catholics separate from Christians?

Don't worry, I'm not suggesting we bring back the Test Acts. The logic here is that **more granular data is better**.

When swearing in, there are versions of the Bible specific to Catholics — typically the New Jerusalem Bible or the Douay–Rheims Bible — whereas if someone just asks for "the Bible", they are given the King James Version and could be from any Christian denomination.

It would be a shame to lose that detail, so I provide the option to break out Catholic MPs separately.

## 📚 Where can I find more information about swearing in and the parliamentary oath?

The Parliament website has a great guide:  
👉 [https://www.parliament.uk/about/how/elections-and-voting/swearingin/](https://www.parliament.uk/about/how/elections-and-voting/swearingin/)

## 👤 Who created this dashboard?

This dashboard was created by **Dr David Jeffery**, University of Liverpool.  
Follow me on [Twitter/X](https://twitter.com/DrDavidJeffery) or [Bluesky](https://drdavidjeffery.bsky.social).

## ❓ Why did you create this dashboard?

I needed to know MPs' religion, and the text MPs used to swear in seemed like a valid proxy. This information was held by Humanists UK and when I asked for it, they said no.

So I did what any time-starved academic would do: I collected the data myself, by hand, and decided to make it public.

---
