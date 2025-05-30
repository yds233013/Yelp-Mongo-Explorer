# Yelp-Mongo-Explorer
This project explores how MongoDB, a NoSQL database, handles semi-structured JSON data using the Yelp Academic Dataset. The project involves querying and analyzing business, user, and review data to understand the capabilities and tradeoffs of document-based data models compared to relational databases.

## 🚀 Project Summary

- Uses **MongoDB** to store and query Yelp's business, user, and review data
- Accesses MongoDB via **PyMongo** in a Python Jupyter Notebook
- Investigates:
  - Document structure and indexing
  - MongoDB query language
  - Differences between MongoDB and relational databases
- Includes free-response insights and autograded code questions

## 🧠 Learning Objectives

- Understand document-oriented data storage
- Practice querying and updating MongoDB collections
- Compare MongoDB performance and flexibility with SQL-based systems
- Work with real-world data in a semi-structured format

## 📁 Dataset

- Yelp Academic Dataset (truncated):
  - `business.json` (full)
  - `review.json` (7,500 reviews)
  - `user.json` (1,000 users)

## 🛠️ Technologies Used

- Python
- PyMongo
- Jupyter Notebook
- MongoDB

## 📷 Example

```python
# Find top-rated restaurants in Las Vegas
business.find({
    "city": "Las Vegas",
    "stars": {"$gte": 4.5}
})
