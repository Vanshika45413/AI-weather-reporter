# 🌤️ AI Weather Reporter

This project was built as part of the **AI Automation Project**.  
It collects user input, validates email, fetches live weather & air quality data, stores it, and sends a weather summary email – optionally enhanced with AI commentary.

---

📽️ Demo Video
🎥 Watch how it works from start to finish:
https://drive.google.com/file/d/1OhfaW5OnphfJnKhkUtURJTx1RkUWjZaE/view?usp=drive_link
---


## 🔗 Live Form

Submit your details here:(https://your-lovable-form-link.com)

---

## 🎯 Features

- 📥 User input via Lovable form (Name, Email, City)
- ✅ JavaScript email validation using regex
- 🌤️ Weather & AQI fetch from [WeatherAPI.com](https://www.weatherapi.com/)
- 🗃️ Data storage in [Supabase](https://supabase.io)
- 📧 Email sent with:
  - Temperature (°C)
  - Weather condition
  - AQI level
- 🧠 Optional: Smart weather commentary using OpenAI or Claude

---

## 🧰 Tech Stack

| Component      | Tool/Service        |
|----------------|---------------------|
| Form           | Lovable             |
| Automation     | Make.com / n8n      |
| Weather API    | WeatherAPI.com      |
| Database       | Supabase            |
| Email          | Gmail SMTP / Mailjet / Brevo |
| AI (Optional)  | OpenAI / Claude     |

---

## 🧪 Email Validation (JavaScript)

```js
function validateEmail(email) {
  const regex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
  return regex.test(email);
}
