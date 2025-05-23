 #  Virtual Pet - React Application

##  How to Install and Run the Application

1. Clone the repository:
   git clone <your-classroom-repo-url>
   cd virtual-pet

2. Install dependencies:
   npm install

3. Run the development server:
   npm run dev

4. Open your browser:
   Visit http://localhost:5173 to view and interact with your virtual pet.

## Features Implemented

 Pet Visualization
- Pet is displayed using emojis to reflect growth stages:
  🥚 Egg (0–5 days), 🐣 Chick (6–10 days), 🐥 Teen (11–20 days), 🐤 Adult (21+ days)
- Activity overlays (🍽️ eating, ⚽ playing, 🛁 cleaning, 💤 sleeping)

 Status Management
- Tracked stats: Hunger, Energy, Happiness, Health, Cleanliness, Bond
- Stats decay over time at different rates
- Visual status bars show rounded values with color coding

 User Interactions
- Feed: Increases hunger, energy, health, bond
- Play: Increases happiness, bond; decreases hunger and energy
- Clean: Resets cleanliness, improves health
- Sleep: Gradually restores energy and health
- Each interaction disables during sleep and shows visual animation

 Time and Aging System
- One real-world minute = one pet day
- Pet age updates continuously; growth stage changes automatically
- Displays current pet age in days

Data Persistence
- Entire pet state saved to localStorage on each change
- On reload, loads state and calculates time passed
- Applies stat decay and ages pet accordingly

Achievements System
- 8 achievements:
  - First feed
  - 5 cleans
  - 5 plays
  - Reach 100 bond
  - Happiness 100
  - Health 100
  - Reach adult stage
  - Clean pet for 3 days (bonus)
- Unlocked achievements shown in panel
- Locked achievements shown faded with description
- Green notification banner on unlock
- Progress saved in localStorage

📱 Responsive Design
- Works on mobile and desktop
- Layout uses flex/grid with adaptive spacing and scaling

##  Bonus Features Added

- Bond stat and interaction logic
- Custom hooks: usePet, useTimePassage, useLocalStorage, useAchievements
- Animated activity states and overlays
- Notification system for live achievement feedback
- Clean visual achievements panel with locked/unlocked styles

## Screenshots 



(image.png)![alt text](<Screenshot 2025-05-14 at 1.42.48 AM.png>) ![alt text](<Screenshot 2025-05-23 at 2.34.18 AM-1.png>) ![alt text](<Screenshot 2025-05-23 at 2.34.05 AM-1.png>) ![alt text](<Screenshot 2025-05-23 at 2.33.43 AM-1.png>)