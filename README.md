# VibeBar

**VibeBar** is a lightweight macOS menu bar application that brings your Apple Music activity to your Discord Rich Presence.

No extra setup. No terminal scripts. Just launch, and your current track will appear in Discord.

---

###  Features

- Live Apple Music playback status in Discord  
- Clean and native macOS menu bar interface  
- Dynamic album covers (optional, powered by [loon](https://github.com/ungive/loon))  
- Customizable buttons (e.g. link to your track or profile)  
- Flexible behavior for paused/stopped states  
- Quick restart button for reloading settings

---

###  Preview

Here's how your presence will appear in Discord:

<!--![screenshot](https://github.com/user-attachments/assets/a6b260cb-be8c-4a59-ab63-1d61d0bfcb7a)-->

<img width="296" height="128" alt="VibeBar" src="https://github.com/user-attachments/assets/d7a92fe9-31ca-4c9e-b81d-f5afc6ec76a9" />


---

###  Requirements

- macOS 11.5+
- Apple Music app installed  
- Local Discord running (web version not supported)  

💡 *Full feature support (including all settings fields) requires macOS 13 or later. On macOS 12, only basic functionality and client ID editing are fully supported.*  

---

###  Installation

1. Download the latest `.dmg` file from [Releases](https://github.com/user1334/VibeBar/releases).
2. Move `VibeBar.app` to your `Applications` folder.
3. Launch it — and grant automation permissions when prompted.
4. That’s it. Your vibes are now live.

---

###  Permissions

macOS will prompt you to grant automation access so VibeBar can read playback info from Apple Music. This is required for real-time updates.  

---

### Dynamic Covers  

If you enable dynamic album covers, VibeBar will check for the [loon](https://github.com/ungive/loon) proxy.  
- If *loon* is not bundled, you’ll be prompted to install it.  
- Installation may require Homebrew or a direct Go-based build.  
- VibeBar itself does **not** ship loon — it only provides a helper script that builds loon directly from its [official repository](https://github.com/ungive/loon) by **ungive**.  

---

### Custom Presence  

VibeBar allows you to configure your own Discord Rich Presence details (images, hover texts, and buttons).  

Here’s an example for the **Listening** presence type:  

 <!--<img width="440" height="154" alt="Bildschirmfoto 2025-08-21 um 21 21 21" src="https://github.com/user-attachments/assets/e0781693-34b1-4c58-891c-210fcca402e2" />-->
 <!--<img width="441" height="150" alt="Bildschirmfoto 2025-08-21 um 21 33 00" src="https://github.com/user-attachments/assets/b846da15-df26-45a3-bf2a-32fcbab767c3" />-->
 <img width="443" height="155" alt="Bildschirmfoto 2025-08-21 um 21 40 07" src="https://github.com/user-attachments/assets/d507e4fc-3b55-4dc1-9fec-97525ccd0b7a" />




- **Large Image Key** → The main image shown (usually album art or custom asset).  
- **Large Image Text (Hover)** → Text shown when hovering over the large image. *(Note: not visible in all presence types)*  
- **Small Image Key** → A smaller image displayed on top of the large image.  
- **Small Image Text (Hover)** → Text shown when hovering over the small image.  
- **Buttons** → Add up to two buttons (e.g. "View Track" / "My Profile").  

 **Important:**  
- Some fields (like *Large Image Hover Text*) do not appear in certain presence types such as *Playing* or *Watching*.  
- Configured buttons are **only visible to other people**, not to yourself in your own Discord client.

---


###  Credits

Built with using SwiftUI and AppKit.
Special thanks to [ungive](https://github.com/ungive) for the original *loon* proxy. 
---
