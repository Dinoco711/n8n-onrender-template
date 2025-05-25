# 🚀 Deploy n8n on Render (Free Tier)

This guide will help you deploy the powerful **n8n workflow automation tool** on [Render](https://render.com) using their free instance.

---

## 🧩 Steps to Deploy

### ✅ Step 1: Create a Render Account
- Go to [render.com](https://render.com) and **sign up** or **log in**.

### ✅ Step 2: Create a New Web Service
- Navigate to **Dashboard → New → Web Service**.

### ✅ Step 3: Use Docker Image for Deployment
- Choose the option: **"Deploy an existing image"**.
- Use this image URL: [docker.n8n.io/n8nio/n8n:latest](docker.n8n.io/n8nio/n8n:latest)


### ✅ Step 4: Configure the Service
- **Name your service** something unique, for example:  
`n8n-onrender-a2`
- Select **Free Instance Type (Hobby Tier)** for cost-free deployment.

### ✅ Step 5: Deploy the Service
- Click **Create Web Service** to deploy.
- Wait for the deployment to complete.

---

## 🔐 Set Environment Variables

After deployment, go to your service settings and add the following environment variables:

| Variable               | Example                                                                 |
|------------------------|-------------------------------------------------------------------------|
| `N8N_EDITOR_BASE_URL`  | `https://n8n-onrender-a2.onrender.com`                                  |
| `N8N_HOST`             | `n8n-onrender-a2.onrender.com`                                          |
| `N8N_PORT`             | `5678`                                                                  |
| `N8N_PROTOCOL`         | `https`                                                                 |
| `N8N_RUNNERS_ENABLED`  | `true`                                                                  |
| `PORT`                 | `5678`                                                                  |
| `WEBHOOK_URL`          | `https://n8n-onrender-a2.onrender.com`                                  |

> 💡 Replace `n8n-onrender-a2` with your actual service name.

---

## ✅ You're Done!

Your n8n instance should now be live at: [https://<your-service-name>.onrender.com](https://<your-service-name>.onrender.com)

---

## 📘 Useful Links

- 🔗 [n8n Documentation](https://docs.n8n.io)
- 🔗 [Render Docs](https://render.com/docs)

---
