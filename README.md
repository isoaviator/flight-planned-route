# flight-planned-route
A route generator im working on

A simple offline tool that generates random airline flight assignments based on the aircraft you choose.  
Runs locally on your computer — no internet or hosting required once set up.

---

## 🔧 Requirements

You only need:

- Python 3 installed on your computer  
  (Download from https://www.python.org if you don’t have it)

Nothing else.

---

## 🚀 How to Run the Program

### 1. Start the Backend (the engine)

1. Open the "backend" folder  
2. Right‑click → "Open in Terminal" (or Command Prompt)  
3. Run these commands:

pip install fastapi uvicorn
uvicorn main:app --reload

4. Leave this window open  
   You should see something like:

Running on http://127.0.0.1:8000

---

### 2. Open the Website (the interface)

1. Go to the "frontend" folder  
2. Double‑click "index.html"  
3. It will open in your browser  
4. The site will automatically connect to the backend you started

You can now:

- Select aircraft  
- Generate assignments  
- View airline, callsign, and route info  

---

## ❗ Troubleshooting

### Aircraft list is empty  
The backend is not running.  
Start it with:

uvicorn main:app --reload

### “No matching routes”  
The selected aircraft has no routes in the data files.

### Airport shows as “Unknown”  
The airport code is missing from airports.json.

---

## 🛠️ Customizing the Data (Optional)

You can edit the files in:

backend/data/

- airlines.json → Add/remove airlines  
- airports.json → Add more airports  
- routes.json → Add more routes  

Refresh the page to apply changes.

---

## ✔ You're Ready to Go

Once the backend is running and the HTML file is open, everything works locally with no extra setup.
