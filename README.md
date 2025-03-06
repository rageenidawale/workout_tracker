# 🏋️ Workout Tracker  

A Python-based **workout tracking app** that logs exercises automatically using **Nutritionix API** and stores data in **Google Sheets**.  

---

## ✨ Features  
- 🏃‍♂️ **Track exercises** by typing a natural-language query (e.g., "Ran 5km and did 30 push-ups").  
- 🔥 **Fetch workout details** like duration and calories burned via **Nutritionix API**.  
- 📊 **Log workouts automatically** in **Google Sheets**.  

---

## 🛠 Setup Instructions  

### 1️⃣ Install Dependencies  

Ensure Python is installed, then install the required library:  

```bash
pip install requests python-dotenv
```

---

### 2️⃣ Create API Keys  

- Sign up at **[Nutritionix](https://www.nutritionix.com/business/api)** and get your **APP ID** & **API Key**.  
- Create a **Google Sheet** and set up a **Sheety API** to connect it.  
- Store API credentials in a **.env file** (or set as environment variables).  

---

### 3️⃣ Configure Environment Variables  

Create a `.env` file and add:  

```ini
NT_APP_ID=your_nutritionix_app_id
NT_API_KEY=your_nutritionix_api_key
SHEET_ENDPOINT=your_google_sheets_api_endpoint
TOKEN=your_sheety_api_token
```

---

### 4️⃣ Run the Application  

Run the script and **input your exercise details**:  

```bash
python main.py
```

Example:  
```bash
Tell me which exercises you did: Ran 5km and did 30 push-ups
```

---

## 📜 How It Works  

1. **Takes a text input** (e.g., "I ran 3 miles and did 20 push-ups").  
2. **Fetches workout details** from **Nutritionix API**.  
3. **Logs the workout** in **Google Sheets** via **Sheety API**.  
