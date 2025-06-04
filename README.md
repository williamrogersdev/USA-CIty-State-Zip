# USA States, Cities, and ZIP Codes Dataset

This repository contains comprehensive JSON datasets for United States geographical data, including states, cities, and ZIP codes with their associated information.

## 📁 Files Overview

### 1. `all_city_state.json`

**Format:** Object with state names as keys and arrays of cities as values

```json
{
  "Alabama": ["ABBEVILLE", "ADAMSVILLE", "ADDISON", ...],
  "Alaska": ["ADAK", "AKIACHAK", "AKIAK", ...],
  ...
}
```

- **Purpose:** Complete listing of cities organized by state
- **City Format:** All uppercase
- **Coverage:** All 50 US states plus territories
- **Use Cases:** State-to-cities mapping, dropdown menus, validation

### 2. `states_abbr.json`

**Format:** Object with state abbreviations as keys and full state names as values

```json
{
  "AL": "Alabama",
  "AK": "Alaska",
  "AZ": "Arizona",
  ...
}
```

- **Purpose:** Mapping between 2-letter state codes and full state names
- **Coverage:** All 50 states plus territories and federal districts
- **Use Cases:** Address formatting, state code conversion, form validation

### 3. `states_titlecase.json`

**Format:** Array of objects with state information

```json
[
  {
    "name": "Alabama",
    "abbreviation": "AL"
  },
  {
    "name": "Alaska",
    "abbreviation": "AK"
  },
  ...
]
```

- **Purpose:** Structured state data with proper title case formatting
- **Coverage:** All US states and territories
- **Use Cases:** Select dropdowns, state listings, structured data needs

### 4. `usa-zipcodes.json`

**Format:** Array of objects with comprehensive ZIP code information

```json
[
  {
    "zip_code": 501,
    "latitude": 40.922326,
    "longitude": -72.637078,
    "city": "Holtsville",
    "state": "NY",
    "county": "Suffolk"
  },
  ...
]
```

- **Purpose:** Complete ZIP code database with geographical coordinates
- **Fields:**
  - `zip_code`: 5-digit ZIP code (number)
  - `latitude`: Geographic latitude (decimal degrees)
  - `longitude`: Geographic longitude (decimal degrees)
  - `city`: City name
  - `state`: 2-letter state abbreviation
  - `county`: County name
- **Coverage:** ~340,000+ ZIP codes across the United States
- **Use Cases:** Address validation, location services, shipping calculations, mapping applications
