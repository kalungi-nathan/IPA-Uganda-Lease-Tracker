# IPA Laptop & PDA Lease Tracker

A web-based inventory lease management system for Innovations for Poverty Action – Uganda Operations.

## Features

- **Role-Based Access Control**: Administrator, Finance, Project Manager, Field Manager, Research Associate
- **Inventory Management**: Track PDAs/Tablets and Laptops with depreciation
- **Lease Requests**: Submit and manage lease requests with automatic billing
- **Smart Billing**: Charges only Monday–Friday, excluding Uganda public holidays (2025–2026)
- **Bulk Upload/Delete**: Import inventory via CSV, bulk-delete assets
- **Reports & Export**: 8 report types, CSV and print export
- **Dashboard**: Real-time KPIs, status charts, activity feed
- **Mobile Responsive**: Works on desktop, tablet, and mobile

## Demo Accounts

| Role | Username | Password |
|---|---|---|
| Administrator | `admin` | `admin123` |
| Finance | `finance` | `finance123` |
| Project Manager | `pm` | `pm123` |
| Field Manager | `fm` | `fm123` |

## Deploy to GitHub Pages

1. Fork or clone this repository
2. Go to **Settings → Pages**
3. Under **Source**, select `Deploy from a branch`
4. Select `main` branch and `/ (root)` folder
5. Click **Save**
6. Your app will be live at `https://<username>.github.io/<repo-name>/`

No build step required. Pure HTML/CSS/JS — deploys instantly.

## Data Storage

Data is stored in the browser's `localStorage`. Each user's data is private to their browser. For production use with shared data, integrate a backend (Firebase, Supabase, or similar).

## CSV Bulk Upload Format

```
assetId,serial,model,category,purchaseDate,purchaseCost,status
PDA-010,SN100010,Samsung Galaxy Tab A9,PDA,2024-01-01,1200000,Available
LAP-010,SN200010,Dell Latitude 3540,Laptop,2024-01-01,3500000,Available
```

## Uganda Public Holidays (2026)

Billing automatically excludes:
- Jan 1 – New Year's Day
- Jan 26 – Liberation Day  
- Feb 16 – Archbishop Janan Luwum Day
- Mar 8 – International Women's Day
- Mar 20 – Eid al-Fitr
- Apr 3 – Good Friday
- Apr 6 – Easter Monday
- May 1 – Labour Day
- May 27 – Eid al-Adha
- Jun 3 – Martyr's Day
- Jun 9 – National Heroes Day
- Oct 9 – Independence Day
- Dec 25 – Christmas Day
- Dec 26 – Boxing Day

## License

Innovations for Poverty Action – Internal Use
