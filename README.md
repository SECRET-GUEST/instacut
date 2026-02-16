
```
██╗███╗   ██╗███████╗████████╗ █████╗  ██████╗██╗   ██╗████████╗
██║████╗  ██║██╔════╝╚══██╔══╝██╔══██╗██╔════╝██║   ██║╚══██╔══╝
██║██╔██╗ ██║███████╗   ██║   ███████║██║     ██║   ██║   ██║   
██║██║╚██╗██║╚════██║   ██║   ██╔══██║██║     ██║   ██║   ██║   
██║██║ ╚████║███████║   ██║   ██║  ██║╚██████╗╚██████╔╝   ██║   
╚═╝╚═╝  ╚═══╝╚══════╝   ╚═╝   ╚═╝  ╚═╝ ╚═════╝ ╚═════╝    ╚═╝   
```
![Javascript](https://img.shields.io/badge/JAVASCRIPT-yellow)

# INSTACUT 🧩

### Instagram 3-Post Grid Splitter (4:5 Safe)

INSTACUT is a lightweight browser tool that splits a single image into **three aligned Instagram posts (1080×1350, 4:5)** while preserving grid continuity.

It compensates for Instagram’s default square preview behavior to avoid visible misalignment in profile grids.

Live version:
[https://secret-guest.github.io/instacut/](https://secret-guest.github.io/instacut/)

## 📸 Why This Exists

Instagram posts are uploaded in **4:5 (1080×1350)**.

However, the profile grid preview crops them closer to **3:4 portrait**, which can break alignment across multi-post layouts.

If you split an image naively into three equal 1080px columns, the grid will not look seamless.

INSTACUT corrects this.

<img width="1866" height="947" alt="image" src="https://github.com/user-attachments/assets/9bc2350f-4ced-4889-944a-d8cc58080658" />


## ⚙️ How It Works

1. The image is loaded into a canvas.
2. A continuous **master canvas** is created based on the visible grid ratio (~3:4).
3. A safe “bleed” area is calculated to compensate for grid cropping.
4. Three 1080×1350 tiles are generated:

   * The visible area is centered.
   * Side pixels are extended using real image data (no 1px stretching).
5. Files are exported as PNG.
6. Optional ZIP download is generated using JSZip.

Everything runs **fully client-side**.
No uploads. No server. No storage.

## 📐 Instagram Sizes Reference

| Context              | Size (px) | Ratio |
| -------------------- | --------- | ----- |
| Post (Portrait)      | 1080×1350 | 4:5   |
| Profile Grid Preview | ~3:4 crop | ~0.75 |

Important:
Instagram defaults to square preview during posting.
Tap **⤢ Expand** before publishing.

## 🚀 Usage

1. Drag & drop an image.
2. Preview appears automatically.
3. Download individual tiles or the ZIP file.
4. Post each image as **4:5 (1080×1350)**.
5. Expand before publishing.

## 📜 License

MIT License.

## ❓ Support

If you encounter issues or have feature suggestions:

* Open an issue
* Start a discussion

## 💎 Recommendations  

In your quest for more tools to enhance your desktop productivity, these additional repositories are worth a look:

- [Barcraft](https://github.com/SECRET-GUEST/barcraft) : Create barcodes/QRCodes using an application free from malware, sourced directly from GitHub.

Looking for more? Discover user-friendly, GUI-free script here: 
- [Tiny Scripts](https://github.com/SECRET-GUEST/tiny-scripts)

If you're a 3D animator, consider:
- [Animation](https://github.com/SECRET-GUEST/animation)



```
     _ ._  _ , _ ._            _ ._  _ , _ ._    _ ._  _ , _ ._      _ ._  _ , _ .__  _ , _ ._   ._  _ , _ ._   _ , _ ._   .---.  _ ._   _ , _ .__  _ , _ ._   ._  _ , _ ._      _ ._  _ , _ .__  _ , _ . .---<__. \ _
   (_ ' ( `  )_  .__)        (_ ' ( `  )_  .__ (_ ' ( `  )_  .__)  (_ '    ___   ._( `  )_  .__)  ( `  )_  .__)   )_  .__)/     \(_ ' (    )_  ._( `  )_  .__)  ( `  )_  .__)  (_ ' ( `  )_  ._( `` )_  . `---._  \ \ \
 ( (  (    )   `)  ) _)    ( (  (    )   `)  ) (  (    )   `)  ) _ (  (   (o o) )     )   `)  ) _    )   `)  ) _    `)  ) \.@-@./(  (    )   `)     )   `)  ) _    )   `)  ) _ (  (    )   `)         `) ` ),----`- `.))  
(__ (_   (_ . _) _) ,__)  (__ (_   (_ . _) _) _ (_   (_ . _) _) ,__ (_   (  V  ) _) (_ . _) _) ,_  (_ . _) _) ,_ . _) _) ,/`\_/`\ (_   (  . _) _) (_ . _) _) ,_  (_ . _) _) ,__ (_   (_ . _) _) (__. _) _)/ ,--.   )  |
    `~~`\ ' . /`~~`           `~~`\ ' . /`~~`   `~~`\ ' . /`~~`     `~~`/--m-m- ~~`\ ' . /`~~`   `\ ' . /`~~`  `\ ' . /  //  _  \\ ``\ '  . /`~~`\ ' . /`~~`   `\ ' . /`~~`     `~~`\ ' . /`~~`\ ' . /`~~/_/    >     |
         ;   ;                     ;   ;             ;   ;               ;   ;      ;   ;          ;   ;         ;   ;  | \     )|_   ;    ;      ;   ;          ;   ;               ;   ;      ;   ;    |,\__-'      |
         /   \                     /   \             /   \               /   \      /   \          /   \         /   \ /`\_`>  <_/ \  /    \      /   \          /   \               /   \      /   \     \__         \
________/_ __ \___________________/_ __ \___________/_ __ \______ __ ___/_ __ \____/_ __ \________/_ __ \_______/_ __ \\__/'---'\__/_/_  __ \____/_ __ \________/_ __ \_____ _______/_ __ \____/_ __ \____ __\___      )
```
