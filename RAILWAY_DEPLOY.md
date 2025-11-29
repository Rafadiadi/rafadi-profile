# 🚂 Deploy ke Railway - Rafadi Profile

Panduan lengkap untuk deploy personal website ke Railway.

## 📋 Prasyarat

1. Akun GitHub (untuk connect repository)
2. Akun Railway (gratis) - [Daftar di sini](https://railway.app/)

## 🚀 Cara Deploy

### Method 1: Deploy via GitHub (Recommended)

#### Step 1: Push ke GitHub
```bash
cd "/Users/crescendo/Documents/Personal Web"

# Initialize git repository
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit - Rafadi Profile"

# Create repository di GitHub dengan nama "rafadi-profile"
# Lalu jalankan:
git remote add origin https://github.com/YOUR_USERNAME/rafadi-profile.git
git branch -M main
git push -u origin main
```

#### Step 2: Deploy di Railway
1. Buka [railway.app](https://railway.app/)
2. Login dengan GitHub
3. Click **"New Project"**
4. Pilih **"Deploy from GitHub repo"**
5. Pilih repository **"rafadi-profile"**
6. Railway akan auto-detect dan deploy

#### Step 3: Konfigurasi Project
1. Setelah deploy, click project Anda
2. Click **"Settings"**
3. Ubah **Project Name** menjadi: **"Rafadi Profile"**
4. Di tab **"Networking"**, click **"Generate Domain"**
5. Custom domain akan dibuat: `rafadi-profile.up.railway.app`

### Method 2: Deploy via Railway CLI

```bash
# Install Railway CLI
npm i -g @railway/cli

# Login
railway login

# Initialize project
railway init

# Set project name
# Nama: Rafadi Profile

# Deploy
railway up
```

## 🔧 Konfigurasi Environment

Railway sudah dikonfigurasi dengan:
- **Builder:** Nixpacks (otomatis detect)
- **Start Command:** Python HTTP Server
- **Port:** 8080 (otomatis dari $PORT)
- **Runtime:** Python 3.9

## 📝 File Konfigurasi

File berikut sudah dibuat untuk Railway:
- ✅ `railway.json` - Railway configuration
- ✅ `nixpacks.toml` - Build configuration
- ✅ `Procfile` - Process configuration
- ✅ `runtime.txt` - Python version

## 🌐 Custom Domain

Setelah deploy, Anda bisa:
1. Gunakan domain Railway gratis: `*.up.railway.app`
2. Atau tambahkan custom domain sendiri di Settings > Networking

## 💰 Pricing

- **Free Tier:** $5 gratis setiap bulan (500 jam)
- Untuk static website seperti ini, biasanya cukup dengan free tier
- Auto-sleep setelah tidak ada traffic

## 🔄 Auto Deploy

Setiap kali Anda push ke GitHub:
- Railway akan otomatis detect changes
- Build ulang website
- Deploy versi terbaru

## 📊 Monitoring

Di Railway dashboard Anda bisa monitor:
- Deploy logs
- Build status
- Traffic analytics
- Resource usage

## 🛠️ Update Website

Untuk update website:
```bash
# Edit file yang diperlukan
# Lalu:
git add .
git commit -m "Update: deskripsi perubahan"
git push
```

Railway akan otomatis deploy versi terbaru!

## 🆘 Troubleshooting

### Website tidak loading?
- Check di Railway Logs apakah ada error
- Pastikan port 8080 digunakan
- Verify semua file sudah ter-push ke GitHub

### Build failed?
- Check railway.json configuration
- Verify Python version di runtime.txt
- Check Deployments logs untuk detail error

### Custom domain tidak work?
- Wait 24-48 jam untuk DNS propagation
- Verify DNS settings di domain provider
- Check Railway Networking settings

## 📞 Support

Jika ada masalah:
- Railway Docs: [docs.railway.app](https://docs.railway.app/)
- Railway Discord: [discord.gg/railway](https://discord.gg/railway)

---

**Nama Project:** Rafadi Profile  
**URL:** `https://rafadi-profile.up.railway.app` (setelah deploy)  
**Status:** Ready to Deploy! 🚀
