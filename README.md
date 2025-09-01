# Click ID Recovery by TAGGRS

**Recover and preserve lost click IDs (GCLID, GBRAID, WBRAID) in Google Ads tracking** using Google Tag Manager Server-Side.  
This template ensures that your conversions are tracked accurately, even with Safari ITP and other privacy restrictions.

---

## 🚀 Features
- ✅ Recovers **GCLID**, **GBRAID**, and **WBRAID** values  
- ✅ Works with **Google Ads Tracking Templates**  
- ✅ Compatible with **all server-side GTM containers**  
- ✅ Supports **Final URL suffix** when other tools use Tracking Templates  
- ✅ Quick installation via **template.tpl**  

---

## 📦 Installation

### 1. Download the Template
- Download the [`Click ID Recovery by TAGGRS.template.tpl`](./template.tpl) file from this repository.  

### 2. Import into sGTM
- Open your **Server-Side GTM container**  
- Go to **Templates → New → Import**  
- Upload the downloaded `.tpl` file  
- Save the template  

### 3. Configure the Tag
- Create a new tag using **Click ID Recovery by TAGGRS**  
- Enter your custom parameter names (e.g. `g_c_l_i_d`, `g_b_r_a_i_d`, `w_b_r_a_i_d`)  
- Enter your **server subdomain** (e.g. `sst.yourdomain.com`)  
- Set the trigger to **All Pages**  

### 4. Update Google Ads Tracking
In **Google Ads → Admin → Tracking**, configure the tracking template:

`{lpurl}?g_c_l_i_d={gclid}&g_b_r_a_i_d={gbraid}&w_b_r_a_i_d={wbraid}`

⚠️ Replace `g_c_l_i_d`, `g_b_r_a_i_d`, `w_b_r_a_i_d` with the names you set in Step 3.

### 5. If Another Tool Uses the Tracking Template
If another tool (e.g. **ClickPatrol**) already uses the Tracking Template,  
add the Click ID parameters to the **Final URL suffix**:

`g_c_l_i_d={gclid}&g_b_r_a_i_d={gbraid}&w_b_r_a_i_d={wbraid}`


### 6. Test & Publish
- In Google Ads, click **Test** to verify approval  
- Once validated, **publish your sGTM container**  

---

## 🧪 Example Setup

**Tracking template:**
`{lpurl}?g_c_l_i_d={gclid}&g_b_r_a_i_d={gbraid}&w_b_r_a_i_d={wbraid}`


**Final URL suffix (if needed):**
`g_c_l_i_d={gclid}&g_b_r_a_i_d={gbraid}&w_b_r_a_i_d={wbraid}`


---

## 🔧 Requirements
- Google Tag Manager **Server-Side container**  
- Google Ads account with **tracking templates enabled**  
- Subdomain for sGTM via TAGGRS (e.g. `sst.example.com`)  

---

## 🙌 Credits
Developed by **[TAGGRS](https://taggrs.io/)** – specialists in server-side tracking & privacy-proof marketing.


