<h1 align="center">NGROK Setup</h1>

ngrok is a globally distributed reverse proxy that secures, protects and accelerates your applications and network services, no matter where you run them. You can think of ngrok as the front door to your applications.


Follow these steps to set up and use NGROK effectively.

---

## Step 1: Download NGROK

<img src="Reference Snaps/reference_image1.png">

1. Open the following link to download NGROK:  [NGROK Download Page](https://ngrok.com/download)
2. Select your operating system and click the **Download** button.

---

## Step 2: Install NGROK

### For Linux Users:
Install NGROK via Snap:  
```bash
snap install ngrok
```

### Extract if needed:
If you downloaded a zip file, extract it after downloading.

---

## Step 3: Add Authtoken

<img src="Reference Snaps/reference_image2.png">
<img src="Reference Snaps/reference_image3.png">

1. **Sign in** to your NGROK account.
2. On the left-hand side, find the **Authtoken** tab and click on it.
3. Copy your token from the top of the page.
4. Run the following command in your terminal to configure NGROK with your token:  
   ```bash
   ngrok config add-authtoken <token>
   ```

---

## Step 4: Set Up a Custom Domain

<img src="Reference Snaps/reference_image4.png">

<img src="Reference Snaps/reference_image5.png">

1. Navigate to the **Domains** section under the **Cloud Edge** tab on the NGROK website.
2. Select a domain and copy it.
3. Use the following command to start a server with your custom domain:

   
   ```bash
   ngrok http --domain=<your-custom-domain> 9080
   ```

## Step 5: Access Your Application

1. Once NGROK is online, you will see a **Forwarding** link.
2. Use the forwarding link to access your application. For example:  
  
   ```bash
   https://(your_domanin_name_here)/(service_name)
   ```


---

## Step 6: Monitor Requests

You can monitor all incoming requests directly on your terminal or NGROK dashboard.

---

You're all set to use NGROK with a custom domain!
