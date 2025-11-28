# 🚗 AckoDrive New Car Scraper – Mahindra (Delhi)
A mini-project built as part of our internship to scrape Mahindra car details from the AckoDrive website.  
Since AckoDrive does not support used cars and the Mumbai location data was not available,  
we continued the project using the **Delhi location**, which successfully provided complete data.

---

## 📌 Project Overview
This project collects data of **15 Mahindra car models** from the AckoDrive website.  
As the site lists only **new cars**, attributes such as Year, KM Driven, and Owners were not available and were excluded.

We extracted:
- Car Name  
- Fuel Type  
- Transmission  
- Price Label  
- Price Range  
- Variants  

The scraped HTML was processed using **BeautifulSoup**, cleaned, structured into a DataFrame, and exported for analysis.

---

## 📁 Files in This Repository
- `TeamE_Minor_Project_IPYNB.ipynb` – Main project notebook  
- `raw_ackodrive.html` – Raw HTML extracted during scraping  
- `AckoDrive_Mahindra_Car.csv` – Mahindra Car CSV file
- `README.md` – Project documentation  

---

## 🧠 Technologies Used
- Python  
- BeautifulSoup (for parsing)  
- Requests (for fetching HTML)  
- Pandas (for cleaning & structuring data)  
- Jupyter Notebook  

---

## 🔍 Data Collected
| Attribute        | Description |
|------------------|-------------|
| Car Name         | Name of the Mahindra model |
| Fuel Type        | Petrol / Diesel |
| Transmission     | Manual / Automatic |
| Price Label      | Location-based pricing info |
| Price Range      | Minimum & maximum on-road price |
| Variants         | Total variants offered |

---

## ⚠️ Issues Faced
- **Mumbai location** data did not load on AckoDrive.  
  Even after selecting Mumbai on the site,  
  **URL did not change** and **class names remained the same**, so data stayed Delhi-based.

- AckoDrive shows only **new cars**, so used car fields like:
  - Year  
  - KM Driven  
  - Owners  
  were unavailable.

- Some class names were dynamic and required manual inspection.

Despite these, we extracted all 15 Mahindra cars available.

---

## ▶️ How to Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-repo-url
2. **Navigate to the project folder:**

  ```bash
  cd your-folder
```
3. **Open the notebook:**

```bash
  jupyter notebook
```
4.**Run all cells to scrape, clean, and export the dataset.**

---

## 👥 Team Members
Priyanshu Prakash Sharma

---
## 📄 License
This project is for educational and academic purposes only.
