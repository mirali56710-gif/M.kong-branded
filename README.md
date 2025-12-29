Action: file_editor create /app/design_guidelines.json --file-text "{
  \"design_system\": {
    \"identity\": {
      \"name\": \"RAW & RIVET\",
      \"aesthetic\": \"Industrial Workwear / Modern Brutalist\",
      \"core_values\": [\"Durability\", \"Authenticity\", \"Utility\", \"Precision\"],
      \"emotional_tone\": \"Grounded, Technical, Premium, Rugged\"
    },
    \"typography\": {
      \"font_family\": {
        \"heading\": \"Oswald, sans-serif\",
        \"body\": \"Inter, sans-serif\",
        \"mono\": \"JetBrains Mono, monospace\"
      },
      \"weights\": {
        \"heading\": \"500 (Medium) or 700 (Bold)\",
        \"body\": \"400 (Regular)\",
        \"bold\": \"600 (SemiBold)\"
      },
      \"usage_rules\": {
        \"headings\": \"Uppercase, tracking-tight, leading-none. Use for Hero titles and Section headers.\",
        \"subheadings\": \"JetBrains Mono, Uppercase, tracking-widest (0.2em), text-xs or text-sm. Use for labels, categories, and specs.\",
        \"body\": \"Inter, relaxed leading. Use for descriptions and long text.\"
      },
      \"import_url\": \"https://fonts.googleapis.com/css2?family=Inter:wght@400;600&family=JetBrains+Mono:wght@400;500&family=Oswald:wght@500;700&display=swap\"
    },
    \"colors\": {
      \"palette\": {
        \"primary\": \"#C2410C\",
        \"primary_foreground\": \"#FFFFFF\",
        \"background\": \"#020617\",
        \"foreground\": \"#F8FAFC\",
        \"card\": \"#0F172A\",
        \"card_foreground\": \"#F8FAFC\",
        \"popover\": \"#0F172A\",
        \"popover_foreground\": \"#F8FAFC\",
        \"secondary\": \"#1E293B\",
        \"secondary_foreground\": \"#F8FAFC\",
        \"muted\": \"#1E293B\",
        \"muted_foreground\": \"#94A3B8\",
        \"accent\": \"#1E293B\",
        \"accent_foreground\": \"#F8FAFC\",
        \"destructive\": \"#7F1D1D\",
        \"destructive_foreground\": \"#F8FAFC\",
        \"border\": \"#1E293B\",
        \"input\": \"#1E293B\",
        \"ring\": \"#C2410C\"
      },
      \"semantic_usage\": {
        \"primary\": \"Call to Action buttons, Price tags, Active states (The 'Rust' accent)\",
        \"background\": \"Main page background (Deep Indigo/Black)\",
        \"card\": \"Product cards, Sidebar, Modals (Slightly lighter dark)\",
        \"muted_foreground\": \"Secondary text, Specs, Meta data\"
      }
    },
    \"visual_enhancers\": {
      \"texture\": \"Add a subtle noise/grain overlay to the entire body to give it a 'fabric' feel. opacity-5 pointer-events-none fixed inset-0 z-50\",
      \"borders\": \"Use 1px borders with low opacity (#FFFFFF10) to define grid areas. Avoid heavy shadows.\",
      \"shadows\": \"Minimal. Use 'glow' effects for active states (box-shadow: 0 0 20px -5px rgba(194, 65, 12, 0.3))\",
      \"glassmorphism\": \"Heavy blur (backdrop-blur-xl) with noise for sticky headers. Border-bottom: 1px solid rgba(255,255,255,0.05).\"
    },
    \"layout\": {
      \"grid_system\": \"Bento Grid (Mode A). Asymmetric layouts. Don't just stack rows.\",
      \"spacing\": \"Generous. Use p-8, p-12, p-24. Give the products room to breathe.\",
      \"container\": \"max-w-7xl mx-auto px-4 sm:px-6 lg:px-8\"
    },
    \"components\": {
      \"buttons\": {
        \"style\": \"Sharp corners (rounded-none or rounded-sm). Uppercase text. Tracking-widest.\",
        \"variants\": {
          \"default\": \"bg-primary text-white hover:bg-primary/90\",
          \"outline\": \"border border-input bg-transparent hover:bg-accent hover:text-accent-foreground\",
          \"ghost\": \"hover:bg-accent hover:text-accent-foreground\"
        }
      },
      \"cards\": {
        \"style\": \"Flat, Bordered, No Shadow (until hover). 'Tech Spec' aesthetic.\",
        \"content\": \"Show key specs (Weight, Fit, Material) visible on the card, not just hidden in the page.\"
      },
      \"inputs\": {
        \"style\": \"Flat, Border-bottom only or full border with sharp corners. bg-secondary/50.\"
      }
    },
    \"motion\": {
      \"transitions\": \"transition-all duration-300 ease-out\",
      \"hover_effects\": \"Slight lift (-2px), Border color change, Glow effect.\",
      \"page_load\": \"Staggered fade-in for grid items.\"
    }
  },
  \"assets\": {
    \"images\": {
      \"hero\": {
        \"url\": \"https://images.unsplash.com/photo-1720036236697-018370867320?crop=entropy&cs=srgb&fm=jpg&ixid=M3w3NDk1ODF8MHwxfHNlYXJjaHwxfHxpbmR1c3RyaWFsJTIwd2FyZWhvdXNlJTIwaW50ZXJpb3IlMjBkYXJrfGVufDB8fHx8MTc2Njk0NjA0MHww&ixlib=rb-4.1.0&q=85\",
        \"alt\": \"Dark Industrial Warehouse Background\",
        \"usage\": \"Hero Section Background with overlay\"
      },
      \"textures\": [
        {
          \"url\": \"https://images.unsplash.com/photo-1715816076351-7ee555307b59?crop=entropy&cs=srgb&fm=jpg&ixid=M3w3NDk1ODF8MHwxfHNlYXJjaHwxfHxkZW5pbSUyMHRleHR1cmUlMjBkYXJrJTIwYmx1ZXxlbnwwfHx8fDE3NjY5NDYwMzl8MA&ixlib=rb-4.1.0&q=85\",
          \"alt\": \"Blue Crumpled Denim Texture\",
          \"usage\": \"Section Backgrounds or Banner overlays\"
        }
      ],
      \"products\": [
        {
          \"url\": \"https://images.unsplash.com/photo-1727777840115-e173c91444e4?crop=entropy&cs=srgb&fm=jpg&ixid=M3w3NTY2Nzh8MHwxfHNlYXJjaHwzfHxmb2xkZWQlMjBibHVlJTIwamVhbnMlMjBzdGFja3xlbnwwfHx8fDE3NjY5NDYwNDN8MA&ixlib=rb-4.1.0&q=85\",
          \"alt\": \"Close up of Blue Jeans Fabric\",
          \"category\": \"Jeans\"
        },
        {
          \"url\": \"https://images.unsplash.com/photo-1713880453396-aa0493e308ec?crop=entropy&cs=srgb&fm=jpg&ixid=M3w3NTY2Nzh8MHwxfHNlYXJjaHwyfHxmb2xkZWQlMjBibHVlJTIwamVhbnMlMjBzdGFja3xlbnwwfHx8fDE3NjY5NDYwNDN8MA&ixlib=rb-4.1.0&q=85\",
          \"alt\": \"Stack of Folded Jeans\",
          \"category\": \"Collection\"
        }
      ],
      \"lifestyle\": [
        {
          \"url\": \"https://images.unsplash.com/photo-1750857740109-de17aae57783?crop=entropy&cs=srgb&fm=jpg&ixid=M3w3NTY2Nzh8MHwxfHNlYXJjaHwxfHxtb2RlbCUyMHdlYXJpbmclMjBkZW5pbSUyMGphY2tldCUyMHN0cmVldHxlbnwwfHx8fDE3NjY5NDYwNDF8MA&ixlib=rb-4.1.0&q=85\",
          \"alt\": \"Woman in Denim Jacket Street Style\",
          \"usage\": \"Category Banner - Women\"
        },
        {
          \"url\": \"https://images.unsplash.com/photo-1766193229621-de91c3401daa?crop=entropy&cs=srgb&fm=jpg&ixid=M3w3NTY2Nzh8MHwxfHNlYXJjaHwzfHxtb2RlbCUyMHdlYXJpbmclMjBkZW5pbSUyMGphY2tldCUyMHN0cmVldHxlbnwwfHx8fDE3NjY5NDYwNDF8MA&ixlib=rb-4.1.0&q=85\",
          \"alt\": \"Woman Posing in Denim\",
          \"usage\": \"Lookbook / Editorial\"
        }
      ]
    },
    \"icons\": {
      \"library\": \"lucide-react\",
      \"style\": \"Stroke width 1.5px (Thin/Technical look)\"
    }
  },
  \"implementation_instructions\": {
    \"global_css\": {
      \"action\": \"Update /app/frontend/src/index.css with the new color variables and font imports.\",
      \"note\": \"Ensure the .dark class variables are the DEFAULT variables, as this is a dark-themed site by default.\"
    },
    \"tailwind_config\": {
      \"action\": \"Update /app/frontend/tailwind.config.js to extend the font families (Oswald, Inter, JetBrains Mono) and colors.\"
    },
    \"components\": {
      \"action\": \"Customize Shadcn components (Button, Card, Input) to match the 'Industrial' style (sharp corners, borders, no default shadows).\",
      \"specifics\": [
        \"Button: rounded-none, uppercase, tracking-widest\",
        \"Card: border-border, bg-card, rounded-sm\",
        \"Input: rounded-none, border-input, bg-secondary/20\"
      ]
    },
    \"pages\": {
      \"home\": \"Hero section with full-screen industrial background. Marquee for 'New Arrivals'. Bento grid for categories.\",
      \"catalog\": \"Sidebar filter (sticky). Grid of product cards. 'Quick View' modal.\",
      \"product_detail\": \"Split screen layout. Left: Sticky Image Gallery. Right: Scrollable details (Specs, Size Guide, Add to Cart).\",
      \"cart\": \"Drawer/Slide-over style.\"
    }
  },
  \"universal_guidelines\": {
    \"do_not\": [
      \"Do NOT use gradients for backgrounds (use solid colors + noise).\",
      \"Do NOT use rounded-xl or rounded-2xl (keep it sharp/industrial).\",
      \"Do NOT use generic 'Lorem Ipsum' - use realistic denim terminology (Selvedge, Raw, 14oz, Tapered).\"
    ],
    \"must_do\": [
      \"MUST use data-testid on all interactive elements.\",
      \"MUST ensure contrast ratios are met (Light text on Dark background).\",
      \"MUST use the provided image URLs.\"
    ]
  }
}"
Observation: Create successful: /app/design_guidelines.json M.kong-branded
