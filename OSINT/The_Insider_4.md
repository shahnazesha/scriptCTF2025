# The Insider 4 | NoobMaster — Write-up

**Description:**  
Good luck! *Max flag limit is 6 for a reason — you shouldn’t need that many. If you do, open a ticket.*  
Flag is case-insensitive.

---

## Walkthrough

While checking the GitHub repo for **The Insider 3**, I noticed a folder for **The Insider 4** containing two images and a short note. The note mentioned checking the comments, which turned out to be the key hint.

[Repository link](https://github.com/scriptCTF/scriptCTF26/tree/main/OSINT/.insider-4/attachments)

One of the image comments read:

> **“Great fireworks! Thanks to the Wendell family for organizing these!”**

This pointed straight toward identifying the fireworks event. After some OSINT digging in Instagram, I learned that **Wendell Family Fireworks** is a long-running **Rockport, Texas 4th of July tradition**.  
That lined up perfectly with the hotel window view in the second attachment.

---

## Identifying the Hotel

Comparing the second image with hotels around **Rockport Bay** and **Little Bay**, one building matched perfectly:

**Holiday Inn Express & Suites Rockport – Bay View**  
**Address:** *901 Hwy 35 N, Rockport, TX 78382, United States*

[Street View confirmation](https://www.google.com/maps/@28.0314711,-97.0462465,3a,75y,272.48h,93.11t/data=!3m7!1e1!3m5!1s9mUXvoqzyZ7wHwmb9J5Ohw!2e0!6shttps:%2F%2Fstreetviewpixels-pa.googleapis.com%2Fv1%2Fthumbnail%3Fcb_client%3Dmaps_sv.tactile%26w%3D900%26h%3D600%26pitch%3D-3.1068241845318028%26panoid%3D9mUXvoqzyZ7wHwmb9J5Ohw%26yaw%3D272.4844775718037!7i16384!8i8192)

The building structure, window layout, and bay orientation all aligned with the challenge image.

---

## Finding the Room Number

Using Google Maps photography and publicly available hotel images, I confirmed that rooms facing the pool and Little Bay are numbered around **115–117** on one end of the wing.

By matching the challenge image’s angle, distance from the corner, and the alignment with nearby buildings, I back-counted the rooms along the same corridor.

After testing a small handful of possible room numbers, the correct one emerged:

**Room 111**

---

## Final Flag
scriptCTF{901_Hwy_35_N_111}

