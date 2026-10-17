# Ruchitha B M – MERN Stack Developer Portfolio

A responsive, high-performance portfolio highlighting full-stack engineering with the **MERN Stack** (MongoDB, Express.js, React.js, Node.js).

## Project Files
- `index.html` – Semantic HTML5 structure with modern metadata and accessibility.
- `style.css` – Dedicated Vanilla CSS stylesheet (MERN dark-mode theme, glassmorphism, responsive grids, keyframe animations).
- `script.js` – Interactive JavaScript logic (typewriter effect, MERN tier switcher, dynamic project filtering, scroll spy, toast notifications).
- `profile.jpg` – Profile photo.
- `Ruchitha_B_M_Resume.pdf` – Resume file linked to "Resume" and "Download Resume" buttons.
- `README.md` – Project documentation.

---

## 1. How to Update Your Resume (PDF)
If you have a new or updated resume PDF:
1. Name your new PDF file `Ruchitha_B_M_Resume.pdf`.
2. Copy and paste it into this `portfolio` folder (replace the existing `Ruchitha_B_M_Resume.pdf`).
3. If you want to use a different filename (e.g., `Ruchitha_MERN_Resume.pdf`), open `index.html` and update:
   - Line 101: `href="./Your_File_Name.pdf"`
   - Line 113: `href="./Your_File_Name.pdf" download="Your_File_Name.pdf"`

---

## 2. Why Resume Download Might Not Trigger Locally (`file:///`) & How to Fix
- **Direct file opening issue:** If you double-click `index.html` directly from Windows Explorer, your browser opens it with the `file:///` protocol. Modern browsers (Chrome, Edge, Brave) frequently block the HTML5 `download` attribute on local `file:///` URLs due to browser security sandbox rules.
- **Solution 1 (Live Server / Localhost):**
  - In VS Code, install the **Live Server** extension.
  - Right-click `index.html` and click **"Open with Live Server"**.
  - When served over `http://127.0.0.1:5500/index.html`, clicking "Download Resume" will immediately trigger the direct download to your Downloads folder!
- **Solution 2 (Direct New Tab Fallback):**
  - We added `target="_blank"` so even if the browser blocks automatic downloading under `file:///`, it immediately opens the PDF in a new tab where you can view, print, or click the download icon.

---

## 3. How to Deploy Live on GitHub Pages
1. Create a repository on GitHub (e.g. `ruchitha-portfolio`).
2. Upload `index.html`, `profile.jpg`, `Ruchitha_B_M_Resume.pdf`, and `README.md`.
3. Go to **Settings** > **Pages** > Select branch `main` / `root` and click **Save**.
4. Your site will be live at `https://<your-username>.github.io/<repo-name>/`, and the resume download button will work for all visitors across all devices.

