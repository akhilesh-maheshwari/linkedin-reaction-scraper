# 👍 LinkedIn Post Reactions Scraper

Extract every person who reacted to any LinkedIn post, enriched with full profile data. Paste the post URL and get a clean, structured export of the whole reactor list with headline, location, follower count, work history, education, and skills attached to each row.

**Perfect for:**
- Warm outbound list building
- Competitor audience mining
- Launch and event follow-ups
- Social intent signal collection

> No login cookies required.

---

## ⚙️ How It Works

| Step | What Happens |
|------|-------------|
| **Input** | Submit one or more LinkedIn post URLs |
| **Collection** | Actor pulls the full list of reactors on the post |
| **Enrichment** | Each reactor is enriched with full profile-level data |
| **Output** | Clean JSON / CSV / Excel export |

Every row includes the reaction type left by that person, so you can segment by intent strength.

---

## 📌 Data Fields

| Field | Description |
|-------|-------------|
| `publicIdentifier` | Public LinkedIn profile slug |
| `linkedInIdentifier` | LinkedIn's internal profile identifier |
| `memberIdentifier` | Numeric LinkedIn member ID |
| `linkedInUrl` | Direct profile URL |
| `firstName` | First name |
| `lastName` | Last name |
| `headline` | Profile headline |
| `summary` | Profile about/summary section |
| `location` | Profile location |
| `followerCount` | Total followers |
| `premium` | Whether the member has LinkedIn Premium |
| `is_open_profile` | Whether the profile is an Open Profile |
| `is_creator` | Whether creator mode is enabled |
| `is_influencer` | Whether the member is a LinkedIn Influencer |
| `is_self` | Internal flag for the requesting account |
| `is_relationship` | Whether the member is a connection |
| `websites` | Websites listed on the profile |
| `connections_count` | Total connections |
| `birthdate` | Birthdate, if public |
| `positions` | Full work history (company, title, dates, description, company ID, LinkedIn URL, logo) |
| `schools` | Full education history (school, degree, grade, dates, school ID) |
| `skills` | Listed skills with endorsement counts and insights |
| `languages` | Languages listed on the profile |
| `recommendations` | Recommendations received |
| `volunteering_experience` | Volunteering history |
| `photoUrl` | Profile picture URL |
| `backgroundUrl` | Profile banner image URL |
| `request_type` | Type of request run |
| `reaction` | `TRUE` for everyone in this export |
| `reaction_type` | Reaction type: `LIKE`, `APPRECIATION`, `INTEREST`, `PRAISE`, `EMPATHY`, `ENTERTAINMENT` |
| `comment` | `TRUE` if the person also commented on the post |

---

## 📊 Sample Output

```json
{
  "publicIdentifier": "agile-practitioner-coach",
  "linkedInIdentifier": "ACoAAAVGw3IBQLa9gfnL2SZKaNbEyRPFzLlBtYg",
  "memberIdentifier": "88523634",
  "linkedInUrl": "https://www.linkedin.com/in/agile-practitioner-coach",
  "firstName": "Siddhesh",
  "lastName": "Dongare",
  "headline": "Decision Intelligence Architect | Product Leader at Mastercard Open Finance | AI Practitioner | Agile Coach of the Year 2024 | 2× Published Author",
  "location": "Thane, Maharashtra, India",
  "followerCount": "8983",
  "premium": "TRUE",
  "is_open_profile": "TRUE",
  "is_creator": "TRUE",
  "positions": {
    "positionsCount": 8,
    "positionHistory": [
      {
        "start": "2/1/2025",
        "end": null,
        "company": "Skill India Digital Hub",
        "location": "India",
        "skills": ["Leadership", "Life Coaching", "Coaching & Mentoring", "Mentor"]
      }
    ]
  },
  "schools": {
    "educationsCount": 3,
    "educationHistory": [
      {
        "start": "1/1/2008",
        "end": "1/1/2010",
        "school": "University of Mumbai",
        "degree": "Master's Degree, Information Technology",
        "grade": "Distinction",
        "school_id": "15093732"
      }
    ]
  },
  "skills": {
    "Skills": [
      { "name": "Product Management", "endorsement_count": 0 },
      { "name": "AI Practitioner", "endorsement_count": 0 }
    ]
  },
  "request_type": "Social Enrichment",
  "reaction": "TRUE",
  "reaction_type": "LIKE",
  "comment": "FALSE"
}
```

---

## 💰 Pricing

**$5.00 per 1,000 reactors**

One flat rate. Full profile enrichment is included by default with no add-on tiers.

---

## 📦 Estimated Delivery Time

| Volume | Delivery Time |
|--------|--------------|
| Up to 10,000 reactors | Within 3 hours |
| 10,000 to 50,000 reactors | 3 to 6 hours |
| 50,000+ reactors | 6 to 12 hours |

---

## 📁 How to Use

1. [Create a free Apify account](https://apify.com)
2. Open this actor and paste your LinkedIn post URL as input
3. Run the actor
4. Download your structured JSON, CSV, or Excel output

---

## ⚠️ Disclaimer

This actor is intended for legitimate business use cases such as market research, lead generation, and outreach. Use it in compliance with LinkedIn's Terms of Service and applicable data privacy regulations (GDPR, CCPA, etc.). The actor does not require or store any LinkedIn credentials.
