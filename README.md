# LittleNorth.Igloo

This repository contains the **RCL (Razor Class Library) views** for **LittleNorth.Igloo**.

The purpose of this repo is to make it easy for consumers of the package to **inspect, copy, and override views** in their own Umbraco websites.

---

## What is this repo for?

When you install `LittleNorth.Igloo` via NuGet, the views are provided through an RCL.  
Umbraco allows you to override any RCL view by placing a file with the same path and name in your website’s `/Views` folder.

This repository exists so you can:

- See exactly which views are available
- Copy the view you want to customise

---

## How to override a view

1. Find the view you want to override in this repository
2. Copy the file (keeping the same folder structure)
3. Paste it into your Umbraco website under:

```
/Views
```
For example:
```
/Views/Partials/blockgrid/Components/textBlock.cshtml
```
Once the file exists in your site, Umbraco will automatically use it instead of the RCL version.

---

## Notes

- You only need to copy the views you want to change
- Unmodified views will continue to use the package defaults
- This repo is **not required** at runtime — it’s a reference and override helper
