# FUTURE_DS_01
Online Retail Sales Performance Analysis Dashboard - Future Interns Data Science Task 1
## Project Files
- Excel File: [Click here to view](https://drive.google.com/file/d/1yWrYQh4Cj1n1wFkZY2fDo_rhsSJiVfoL/view?usp=sharing)
# 📊 Online Retail Sales Performance Analysis Dashboard

**Future Interns Data Science Internship — Task 1**

---

## 📌 Project Overview
An interactive Excel dashboard analyzing online retail sales performance, 
built to uncover key business insights including revenue trends, 
top-performing products, customer behavior, and regional sales distribution.

---

## 🎯 Objectives
- Analyze sales performance across products, regions, and time periods
- Identify top-selling products and highest-revenue categories
- Track monthly and yearly revenue trends
- Provide actionable insights through visual data storytelling

---

## 🛠️ Tools Used
- **Microsoft Excel** — Data cleaning, analysis & dashboard design
- **Pivot Tables & Charts** — Dynamic data summarization
- **Conditional Formatting** — Visual KPI highlighting

---

## 📂 How to Access the Dashboard

> ⚠️ The dashboard file exceeds GitHub's 25MB limit and has been split into 3 parts.
> Download all 3 parts and reassemble using PowerShell.

### Step 1: Download all 3 parts
| File | Size |
|------|------|
| dashboard_part0.zip | 25 MB |
| dashboard_part1.zip | 25 MB |
| dashboard_part2.zip | 10 MB |

### Step 2: Reassemble using PowerShell
```powershell
$parts = Get-ChildItem "dashboard_part*.zip" | Sort-Object Name
$out = [System.IO.File]::OpenWrite("dashboard_restored.xlsx")
foreach ($p in $parts) {
    $data = [System.IO.File]::ReadAllBytes($p.FullName)
    $out.Write($data, 0, $data.Length)
}
$out.Close()
```
### Step 3: Open dashboard_restored.xlsx in Microsoft Excel ✅

---

## 👨‍💻 Author
**Ambrose** — Future Interns Data Science Program
