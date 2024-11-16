+++
title = 'HugHugo Skeleton Theme Setup Guidee'
date = 2024-11-16T16:15:44-05:00
draft = false
+++

## Prerequisites

- Latest version of Hugo installed
- Visual Studio Code installed
- Basic command line knowledge

## Method 1: Creating a Project with Theme Directory

### Step 1: Create New Site

```bash
# Open PowerShell/Terminal in your desired directory
hugo new site skeleton
```

### Step 2: Create New Theme

```bash
# Navigate to your project directory
cd skeleton

# Create a new theme
hugo new theme my-theme
```

### Step 3: Configure Theme

1. Open `config.toml` (or `hugo.toml`)
2. Add the theme configuration:

```toml
theme = "my-theme"
```

### Step 4: Start Development Server

```bash
hugo server
```

- Click the provided localhost link to view your site

## Method 2: Creating a Project Without Theme Directory

### Step 1: Create Themeless Project

```bash
# Create a new skeleton project without separate theme directory
hugo new theme skeleton-no-theme --theme-dir .
```

- This command merges theme files directly into your project root

### Step 2: Project Structure

The resulting structure will have:

- Layouts directly in your project root
- No separate themes directory
- All necessary template files in the base project

### Step 3: Start Development Server

```bash
hugo server
```

## Important Notes

1. The skeleton theme provides:
   - Basic HTML structure
   - Head section with CSS/JS placeholders
   - Minimal default layout

2. Limitations:
   - Deliberately excludes intermediate and advanced features
   - Meant for basic testing and starting points
   - Advanced features need to be added manually

3. File Structure:
   - `/layouts`: Contains basic template files
   - `/content`: Where your content files go
   - `/static`: For static assets
   - `/archetypes`: Default content templates
