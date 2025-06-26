# MERN Stack Project Setup - Batch No 6

# Step 1: Navigate to 'Code' folder (present in 'Batch No 6' directory)

cd Code

# Step 2: Create .env file inside the 'server' folder

cd server
touch .env
echo ".env file created in server folder"
echo "Now open 'envSetUp.txt' from the Code folder and copy its content into the .env file"
read -p "Press Enter after adding the environment variables..."

# Step 3: Install backend dependencies
npm install
echo "Backend dependencies installed"

# Step 4: Move to frontend folder
cd ../frontend

# Step 5: Install frontend dependencies
npm install
echo "Frontend dependencies installed"

# Step 6: Instructions to run the project
echo "To start the servers, open two terminals:"
echo "Terminal 1: cd Code/server && npm start"
echo "Terminal 2: cd Code/frontend && npm start"


# step 7: Wait for frontend to start
sleep 5

# step 8: Open User A (normal browser)
echo "Opening Chrome for User A (normal)..."
google-chrome "http://localhost:3000" &

# step 9: Wait a bit
sleep 2

# step 10: Open User B (incognito browser)
echo "Opening Chrome for User B (incognito)..."
google-chrome --incognito "http://localhost:3000" &

echo "Both instances running. Use different accounts to simulate chat."








