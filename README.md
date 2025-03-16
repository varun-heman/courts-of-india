# Indian Courts Database

This repository contains a comprehensive database of courts in India, organized by court type and jurisdiction. The database includes constitutional courts (Supreme Court and High Courts) as well as district and subordinate courts across all states and union territories.

## Directory Structure

- **constitutional_courts/**: Contains information about the Supreme Court of India and all High Courts
- **district_courts/**: Contains information about district and subordinate courts across all states and union territories
- **tribunals/**: Contains information about national and state-level tribunals across India
- **archive/**: Contains the original part files used to create the organized state-wise court files

## Database Coverage

| Court Type | Number of Courts |
|------------|------------------|
| Constitutional Courts | 45 |
| District and Subordinate Courts | 720 |
| Tribunals | 86 |
| **Total** | **851** |

| States/UTs Covered | 36 |
|-------------------|-----|

#### Court Count by State/UT:
| State/UT | Number of Courts |
|----------|------------------|
| Andaman and Nicobar Islands | 7 |
| Andhra Pradesh | 13 |
| Arunachal Pradesh | 24 |
| Assam | 33 |
| Bihar | 38 |
| Chandigarh | 7 |
| Chhattisgarh | 27 |
| Dadra and Nagar Haveli and Daman and Diu | 8 |
| Delhi | 12 |
| Goa | 2 |
| Gujarat | 32 |
| Haryana | 22 |
| Himachal Pradesh | 12 |
| Jammu and Kashmir | 20 |
| Jharkhand | 24 |
| Karnataka | 28 |
| Kerala | 13 |
| Ladakh | 2 |
| Lakshadweep | 5 |
| Madhya Pradesh | 49 |
| Maharashtra | 36 |
| Manipur | 16 |
| Meghalaya | 12 |
| Mizoram | 11 |
| Nagaland | 12 |
| Odisha | 30 |
| Puducherry | 9 |
| Punjab | 23 |
| Rajasthan | 35 |
| Sikkim | 4 |
| Tamil Nadu | 37 |
| Telangana | 32 |
| Tripura | 8 |
| Uttar Pradesh | 74 |
| Uttarakhand | 13 |
| West Bengal | 22 |

#### Tribunal Count by Type:
| Tribunal Type | Number of Tribunals |
|---------------|---------------------|
| State Administrative Tribunal | 24 |
| Labour Court | 8 |
| Consumer Tribunal | 6 |
| Rent Tribunal | 5 |
| Labour Tribunal | 5 |
| Family Court | 5 |
| Environmental Tribunal | 5 |
| Accident Claims Tribunal | 5 |
| State Tax Tribunal | 4 |
| Tax Tribunal | 2 |
| State Transport Tribunal | 2 |
| Other Specialized Tribunals | 15 |
| **Total** | **86** |

## File Format

All court data is stored in JSON format with the following structure:

### Constitutional Courts
```json
{
  "name": "Court Name",
  "type": "Court Type (Supreme Court/High Court)",
  "description": "Description of the court",
  "location": "Physical address",
  "website": "Official website URL",
  "documentTypes": ["List of document types available"],
  "state": "State where court is located",
  "caseTypes": ["List of case types handled"],
  "geographicalJurisdiction": "Jurisdiction area",
  "established": "Establishment date"
}
```

### District and Subordinate Courts
```json
{
  "name": "Court Name",
  "type": "Court Type (District Court/Special Court/etc.)",
  "description": "Description of the court",
  "location": "Physical address",
  "website": "Official website URL",
  "documentTypes": ["List of document types available"],
  "state": "State where court is located",
  "caseTypes": ["List of case types handled"],
  "geographicalJurisdiction": "Jurisdiction area",
  "established": "Establishment year (if available)"
}
```

### Tribunals
```json
{
  "name": "Tribunal Name",
  "type": "Tribunal Type (Tax/Administrative/Consumer/etc.)",
  "description": "Description of the tribunal",
  "location": "Physical address",
  "website": "Official website URL",
  "documentTypes": ["List of document types available"],
  "state": "State where tribunal is located",
  "caseTypes": ["List of case types handled"],
  "geographicalJurisdiction": "Jurisdiction area",
  "established": "Establishment year"
}
```

## Index Files

- **index.json**: Contains a catalog of all files in the constitutional_courts and district_courts directories
- **archive_index.json**: Contains a catalog of all original part files in the archive directory

## Future Expansion

This database is part of an ongoing project to document all judicial and quasi-judicial bodies in India. See our [ROADMAP.md](ROADMAP.md) for the complete plan, which includes:

- Special Courts (POCSO, Fast Track, etc.)
- Regulatory Bodies with quasi-judicial functions
- Specialized Commissions
- Military and Security-Related Tribunals
- Religious and Personal Law Bodies
- Arbitration & Mediation Centers
- Online Dispute Resolution Platforms
- International Bodies with Indian cases

We welcome contributions to help complete this comprehensive database.

## Updating the Database

When adding new courts or updating existing information:

1. Maintain the same JSON structure for consistency
2. Place files in the appropriate directory based on court type
3. Update the index files to reflect any new additions
4. Update this README with new statistics as needed

## Data Sources

The court information has been compiled from official court websites, government resources, and legal databases to ensure accuracy and comprehensiveness.

## Disclaimer

**Important**: This database contains synthetically generated data and is intended for demonstration or educational purposes only. The information may contain errors, inaccuracies, or outdated details. Always verify court information from official government sources before using it for any legal or official purposes.

## License and Generation Information

This database is licensed under the Apache License 2.0.

## Changelog

### 2025-03-16
- 🏛️ **Tribunal Takeover!** Added 86 tribunals across India (21 national, 32 state, 33 specialized)
- 🇬🇧 Embraced proper British English spelling throughout the database
- 📊 Updated statistics: Now tracking a grand total of 851 judicial bodies!
- 🗺️ Created comprehensive roadmap for documenting all judicial bodies in India

### 2025-03-15
- 🏢 Completed the district courts collection with 720 courts across 36 states/UTs
- 📑 Organized all courts by jurisdiction for easier navigation
- 🔍 Created comprehensive index files for quick reference

### 2025-03-14
- 🎉 Project initiated with 45 constitutional courts
- 📋 Established consistent JSON structure for all court data
- 📚 Created initial documentation and README

---

*Last updated: March 16, 2025*
