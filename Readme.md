<!-- FEATURES -->
1--User-Friendly Interface: The web app has a clean and responsive interface built with React and styled using Bootstrap/Tailwind CSS.

2--CRUD Operations for Flashcards: Create, Read, Update, and Delete flashcards.

3--Leitner System Implementation: The app uses the Leitner system to review flashcards. Based on user responses (correct/incorrect), flashcards are reviewed at spaced intervals to improve memory retention.

4--Progress Tracking: The system tracks which flashcards need to be reviewed and at what frequency.

5--how Answer Feature: Users can click a button to reveal the answer to each flashcard during review.



<!-- Backend Setup -->
 
1--Install backend dependencies:
     cd backend
     npm install

2--Create a .env file in the backend 
    MONGO_URI
    PORT=5000

3--Start the backend server:
    npm run dev or nodemon server.js


<!-- Frontend Setup -->

1--Navigate to the frontend directory:
    cd frontend
    
2--Install frontend dependencies:
    npm install

3--Start the frontend server:
    npm start



<!-- Thought Process Behind the Leitner System -->
The Leitner System is a method for using spaced repetition to improve the effectiveness of learning. 
It works by sorting flashcards into different boxes based on how well the user knows each flashcard.
 Flashcards that are easy are reviewed less often, while harder cards are reviewed more frequently.

a--Flashcards are grouped into boxes. Initially, all flashcards are in Box 1.

b--When the user answers a flashcard correctly, it moves to the next box (i.e., from Box 1 to Box 2), indicating the flashcard is easier to recall.
c--If the user answers a flashcard incorrectly, it moves back to Box 1, meaning the card will be reviewed sooner.

d--The flashcards in each box are reviewed at different frequencies. Flashcards in higher-numbered boxes (Box 3, Box 4) are reviewed less frequently than those in Box 1.
 
 