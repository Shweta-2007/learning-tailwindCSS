# LEARNING TAILWIND CSS

# Icons:

- HeroIcons => paste the svg link of the icon in the folder and change the classes according to requirement.

# Google Fonts

- Add import links in index.css and apply font-family to the components.

# To add custom colors, fonts or whatever you want:

- Write inside extend in the tailwind.config.js

extend: {
colors: {
primary: "#FF6363",
secondary: {
100: "#E2E2D5",
200: "#888883",
},
},
fontFamily: {
body: ["Nunito,"],
},
},

# If there are same no of classes repeating in many components then you can make a reusable class:

- .badge {
  @apply bg-secondary-100 text-secondary-200 text-xs font-bold rounded-full p-2 absolute top-0 ml-2 mt-2;
  }

Now give this badge class to the component.

<div className="badge">
