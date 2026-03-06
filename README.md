# NurturInk Seed Data

This repository contains the platform template seed data for the NurturInk application.

## Structure

Each file contains `categories` and `templates` arrays for a specific industry:

- `universal.json` — Loaded for all users regardless of industry
- `insurance.json` — Insurance industry templates
- `real_estate.json` — Real estate industry templates  
- `mortgage.json` — Mortgage industry templates

## Adding a New Industry

1. Create a new `{industry_key}.json` file following the same schema
2. The seeder will automatically pick it up — no code changes needed

## Schema

### Category
```json
{
  "name": "Thank You",
  "slug": "thank-you",
  "description": "Express gratitude to clients",
  "subcategory": "Milestones",
  "sortOrder": 1
}
```

### Template
```json
{
  "name": "Template Name",
  "content": "Message content here...",
  "categorySlugs": ["thank-you"]
}
```
